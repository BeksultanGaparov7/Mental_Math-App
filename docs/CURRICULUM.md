# Curriculum (skill tree)

Each **skill** has a generator, levels, and a mastery rule.
Mastery of a level = last 20 attempts ≥ 90 % correct **and** median time ≤ target.
Mastering a level unlocks the next; mastering level 1 of a skill can unlock other skills.

## Tree (MVP)

```
Addition ──┬── Subtraction ──┐
           │                 ├── Multi-digit mental ── Vedic tricks
Multiplication ── Division ──┤
           │                 └── Fractions ↔ Decimals ↔ Percents
           ├── Squares ── Square roots
           └── Primes & Factors ── GCD/LCM
```

## Skills and levels

| Skill | L1 | L2 | L3 | L4 | L5 | Target time (L1→L5) |
|---|---|---|---|---|---|---|
| **Addition** | 1d+1d | 2d+1d | 2d+2d no carry | 2d+2d carry | 3d+2d | 1.5 → 5 s |
| **Subtraction** | ≤ 18 − 1d | 2d−1d | 2d−2d no borrow | 2d−2d borrow | 100/1000 complements | 1.5 → 5 s |
| **Multiplication** | tables 2–5 | tables 6–9 | tables 11–12 | 2d×1d | teens × teens (11–19) | 1.5 → 6 s |
| **Division** | inverse tables 2–5 | inverse 6–9 | inverse 11–12 | 2d÷1d exact | 3d÷1d exact | 1.5 → 6 s |
| **Squares** | 1–12 | 13–20 | 21–30 | ending in 5 (to 95) | near 50 / near 100 | 1.5 → 4 s |
| **Square roots** | perfect ≤ 144 | ≤ 400 | ≤ 900 | estimate √n to 1 dp | — | 2 → 6 s |
| **Primes & factors** | prime? ≤ 50 | prime? ≤ 100 | factor pairs ≤ 100 | prime factorisation ≤ 200 | GCD/LCM | 2 → 8 s |
| **Fractions / % / decimals** | halves/quarters/tenths | eighths, fifths | thirds, sixths, ninths, sevenths | % of number (10/25/50/x) | % change, fraction ops | 2 → 8 s |
| **Vedic tricks** | ×11 | squares ending in 5 | Nikhilam near 100 | Urdhva 2d×2d | ×5, ×25, ÷5 shortcuts | 3 → 10 s |

## Vedic / trick lessons (MVP set)

Each = 1 animated lesson card (≤ 30 s) → guided examples → drill.

1. **×11** – split & add middle (43×11 → 4|7|3 = 473), carry case.
2. **Squares ending in 5** – n5² = n(n+1)|25 (65² = 42|25).
3. **Nikhilam (base 100)** – 97×96: deficits 3,4 → 97−4 = 93 | 3×4 = 12 → 9312.
4. **Urdhva-Tiryak 2d×2d** – vertical & crosswise (23×41: 2·4 | 2·1+3·4 | 3·1).
5. **×5 / ×25 / ÷5** – ×10÷2, ×100÷4, ×2÷10.
6. **Squares near 50** – (50±a)² = (25±a)|a².
7. **Subtraction from 1000** – "all from 9, last from 10".

## Later (roadmap)

- v1.1 Estimation (number line, rounding products), mixed order of operations
- v2 Spatial: mental rotation, paper folding; cubes, powers of 2
- v3 Algebra 1 fluency: one-/two-step equations, distributing, combining like terms,
  exponent rules, factoring trinomials, slope from two points
- v4 Algebra 2 & geometry: radicals, quadratics (discriminant at a glance), log facts,
  angle facts, Pythagorean triples, special triangles, area/volume formulas
