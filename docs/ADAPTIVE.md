# Adaptive engine, mistake patterns, Nightmare Trial

## 1. Item scheduler (spaced repetition)

- An **item** = a concrete fact or a generator bucket (e.g. `mul:7x8`, `add:2d+2d:carry`).
- MVP: a simple FSRS-style model per item (stability, difficulty, due date). Candidate
  small borrowing: the open-source FSRS algorithm (MIT) — only the scheduling formula.
- Grade from the attempt: miss → Again; correct but slow (> target) → Hard;
  correct ≤ target → Good; correct ≤ 0.5 × target → Easy.
- **Daily Mix** = due items (oldest first) + 20 % new items from the current level,
  interleaved across skills, capped at ~3 min.

## 2. Difficulty within a session

Target success ≈ 85 %. Rolling window of 10: > 95 % → step up a sub-level,
< 70 % → step down. Accuracy is checked before speed.

## 3. Mistake classifier (rule-based, MVP)

Run on each miss (and on slow corrects). Tags:

| Tag | Rule (example) |
|---|---|
| `fact:a×b` / `fact:a+b` | single-digit fact wrong |
| `carry_missed` | addition answer = true − 10ᵏ for a carry column |
| `borrow_missed` | subtraction answer differs by 10ᵏ at a borrow column |
| `off_by_one` | \|given − expected\| = 1 |
| `off_by_operand` | given = expected ± one operand (counting/adding one too many groups) |
| `place_value_shift` | given = expected × 10^±k |
| `digit_swap` | same digits, two transposed |
| `sign_error` | given = −expected |
| `wrong_operation` | given = result of a different operation on the same operands |
| `table_neighbour` | given is a neighbouring table value (7×8 → 54 or 63) |
| `fraction_inverse` | gave b/a for a/b, or 1/x confusion |
| `percent_base` | used wrong base in % change |
| `slow_fact` | correct but > 2 × target time |
| `unknown` | none matched |

Each tag also records the **context** (skill, level, digits involved), so patterns like
"carry errors only when the tens column sums to ≥ 15" can surface.

## 4. Pattern detection

- Score per tag = recency-weighted count (half-life 7 days) × error rate in its context.
- A **pattern** = tag + context with score above threshold and ≥ 5 occurrences.
- Insights chart shows the top 5 patterns, plus a facts heatmap (e.g. the 12 × 12
  multiplication grid coloured by error rate / median time).

## 5. Nightmare Trial

1. Pick the top 1–3 patterns.
2. For each, a **targeted generator** creates items that provoke it (e.g.
   `carry_missed` → 2d+2d with a carry in the tens column; `fact:7×8` → 7×8, 8×7, 56÷7,
   70×80, 7×18).
3. Mix 70 % targeted / 30 % lure items, 3 lives, no hints, 15–25 items.
4. Result screen: before/after error rate for each pattern; beating the trial marks
   the pattern "weakened" and pushes its items to the front of the scheduler.
5. Sandbox mode: replay any pattern untimed with step-by-step solution hints.
