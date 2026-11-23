# MVP functional spec

Platform: Android (Galaxy S24, 6.2", portrait). Offline. Single user. Local storage only.

## Screens

| # | Screen | Purpose |
|---|---|---|
| S1 | **Home** | Mascot, level & XP bar, streak, "Daily Mix" big button, skill tiles, Nightmare Trial tile (when ready) |
| S2 | **Skill detail** | Levels with mastery state, best times, start Sprint / Set / Practice, open trick lesson |
| S3 | **Quiz** | Question, answer field, custom numpad, timer/progress, combo meter, instant feedback |
| S4 | **Results** | Score, accuracy, median time, XP gained, slowest items, "retry misses" |
| S5 | **Insights** | Mistakes chart (top patterns), slowest facts heatmap (e.g. ×-table grid), trend over 14 days |
| S6 | **Nightmare Trial** | Intro (which patterns it targets) → boss quiz → result (patterns weakened) |
| S7 | **Trick lesson** | Step-by-step animated example → 3 guided items → drill |
| S8 | **Settings** | Haptics, sound, timer on/off, theme, data export (CSV) |

## Quiz modes

| Mode | Rule |
|---|---|
| **Sprint** | 60 s, as many as possible; score = correct × speed bonus |
| **Set of 20** | 20 items; tracks time per item |
| **Practice** | Untimed, unlimited, hints allowed, no XP penalty |
| **Daily Mix** | ~3 min interleaved queue from the spaced-repetition scheduler |
| **Nightmare Trial** | 15–25 items generated from top error patterns, 3 lives |

## Input

- Custom numpad (0–9, ⌫, −, ., /, ✓). Auto-submit when the typed answer has the
  correct number of digits *and* is correct; otherwise ✓ to submit (prevents "typing
  until right" gaming: first wrong submission counts as a miss).
- Large tap targets (≥ 56 dp), haptic tick on key, strong haptic on miss.
- Yes/No questions (e.g. "Is 91 prime?") use two big buttons.

## Gamification (MVP)

- **XP**: +10 correct, + speed bonus (up to +5 when under target time), ×combo
  multiplier (1.0 → 2.0 at 10 in a row). Practice mode gives 50 % XP.
- **Player level**: XP curve `xp_for_level(n) = 100 · n^1.5` (rounded).
- **Streak**: days with ≥ 1 completed session; 1 "freeze" earned per 7-day streak.
- **Skill mastery stars**: 0–3 per level (accuracy, speed, consistency).
- **Trophies**: bronze/silver/gold per skill (like the reference screenshot's tiles).
- **Nightmare Trial**: unlocks when the mistake engine finds ≥ 1 pattern with ≥ 5
  errors; beating it gives a badge and big XP.

## Mistake engine (summary – full detail in ADAPTIVE.md)

Every attempt logs: skill, level, operands, expected, given, correct?, time ms,
timestamp, mode. A rule-based classifier tags misses, e.g.:
`carry_missed`, `borrow_missed`, `off_by_one`, `table_fact:7x8`, `digit_swap`,
`place_value_shift` (×10 error), `sign_error`, `slow_fact` (correct but > 2× target).
Insights chart groups by tag; Nightmare Trial samples generators that trigger the
top tags.

## Data model (sketch)

```
Attempt(id, ts, skill, level, mode, prompt, operands[], expected, given,
        correct, timeMs, tags[])
ItemState(itemKey, stability, difficulty, due, lapses, reps)   // scheduler
SkillProgress(skill, level, stars, bestSprint, mastered)
Profile(xp, level, streak, freezes, lastActiveDate, settings)
```

## Out of scope for MVP

Accounts, sync, leaderboards, notifications beyond one daily reminder, iOS.
