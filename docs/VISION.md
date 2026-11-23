# Vision

## Goal (one paragraph)

Build a personal, offline Android app (Samsung Galaxy S24) that makes me **fast and
accurate at the math that algebra and geometry are built on**. It trains only skills
with research evidence of payoff, uses spaced, interleaved retrieval practice, learns
the *patterns* in my mistakes and turns them into a targeted **Nightmare Trial**, and
wraps everything in a short-session game loop (levels, XP, streaks) so I actually open
it every day. Long term it grows from arithmetic fluency into Algebra 1 & 2 and geometry.

## Who it's for

One user (me), adult, wants speed for school/test/quant-style math. Not a kids' app,
not a social app. Personal use first; publishing is a later, optional decision.

## Success criteria (measurable)

| Metric | MVP target |
|---|---|
| Median response time on single-digit facts (+ − × ÷) | < 1.5 s at ≥ 95 % accuracy |
| 2-digit × 1-digit, 2-digit ± 2-digit | < 4 s at ≥ 90 % |
| Squares 1–30, roots of perfect squares to 900 | < 2 s at ≥ 95 % |
| Fraction ↔ decimal ↔ percent (common set) | < 3 s at ≥ 90 % |
| Daily habit | Session ≤ 5 min; ≥ 5 days/week for 4 weeks |
| Mistake engine | Each Nightmare Trial targets a detected pattern; that pattern's error rate falls over the next 2 weeks |

## Principles

1. **Evidence first.** Every drill has an entry in `RESEARCH.md`. No evidence → not in MVP.
2. **Fluency frees the mind.** Automatic facts leave working memory for the real problem.
3. **Retrieval > re-reading, spaced > massed, mixed > blocked.**
4. **Short and daily.** A 2–5 minute session is a complete win.
5. **Mistakes are data.** Every answer is logged with time and error type.
6. **Offline, private, no ads, no account.**
7. **Small, cheap codebase.** Template scaffold + small licensed borrowings only.

## Non-goals (for MVP)

- Multiplayer, leaderboards, accounts, cloud sync
- Generic "IQ" brain games without math transfer (chess, Queens-type puzzles, n-back)
- Full algebra/geometry curriculum (roadmap v3+)
- iOS, web, tablets (may come free with the stack, not a target)
- Monetisation

## Product pillars

1. **Drill** – quick quizzes per skill (Sprint 60 s, Set of 20, Untimed Practice).
2. **Path** – a skill tree with levels that unlock in a sensible order.
3. **Review** – daily spaced-repetition queue across all unlocked skills ("Daily Mix").
4. **Insight** – mistakes chart: top error patterns, slowest facts, trends.
5. **Nightmare Trial** – a boss-style session built from my own error patterns.
6. **Tricks** – short lessons for Vedic/mental shortcuts, followed by drills.
