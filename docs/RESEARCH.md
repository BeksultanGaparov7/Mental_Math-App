# Research basis

Rule: a drill enters the MVP only if it has **direct** evidence of improving math
performance, or is a fact set that algebra/geometry procedures use constantly.
Evidence grades: **A** strong (meta-analyses / replicated RCTs), **B** good (several
studies, correlational + some causal), **C** plausible/practical, **D** little or no
transfer.

> Citations are from memory of the literature; verify details before quoting them
> outside this project.

## 1. Learning methods (apply to every drill)

| Method | Grade | Key sources | How the app uses it |
|---|---|---|---|
| Retrieval practice (testing effect) | A | Roediger & Karpicke 2006; Dunlosky et al. 2013 (rated "high utility") | Every drill is answer-producing recall, not multiple-choice by default |
| Spaced / distributed practice | A | Cepeda et al. 2006 meta-analysis; Dunlosky et al. 2013 | Per-item scheduler (see `ADAPTIVE.md`) |
| Interleaving problem types | A/B | Rohrer & Taylor 2007; Rohrer, Dedrick & Stershic 2015 (7th-grade math RCT) | Daily Mix and Nightmare Trial mix skills |
| Immediate corrective feedback | B | Hattie & Timperley 2007 | Show correct answer + trick hint after a miss |
| Desirable difficulty | B | Bjork & Bjork 2011 | Target ~85 % success rate (adaptive difficulty) |
| Gamification | B (small effect) | Sailer & Homner 2020 meta-analysis | Motivation layer only; never at the cost of the above |

## 2. Content: what to drill

| Skill | Grade | Why it matters for algebra/geometry | Sources |
|---|---|---|---|
| **Single-digit arithmetic fact fluency** (+ − × ÷) | A | Automatic facts reduce cognitive load during multi-step problems; fluency predicts later math achievement | Sweller (cognitive load theory); Price, Mazzocco & Ansari 2013; Fuchs et al. fact-fluency interventions |
| **Multi-digit mental arithmetic** (2d±2d, 2d×1d) | B | Same mechanism; constant in equation solving | as above |
| **Fractions, decimals, percents** | A/B | Fraction & division knowledge at age 10–12 predicts high-school algebra even after controlling for IQ and family background | Siegler et al. 2012 (Psych. Science) |
| **Number sense / estimation** (number line, magnitude) | B | Magnitude understanding correlates with and supports arithmetic | Booth & Siegler 2006, 2008; Schneider et al. 2018 meta-analysis |
| **Squares, square roots, powers** | C (fact knowledge) | Used in quadratics, Pythagoras, simplifying radicals | Curriculum logic |
| **Primes, factor pairs, divisibility, GCD/LCM** | C | Factoring, simplifying fractions/rational expressions | Curriculum logic |
| **Vedic / shortcut techniques** | C | Speeds up large products; little controlled research | Tirthaji 1965 (source text); classroom reports only |
| **Spatial skills** (mental rotation) | A/B | Spatial training is durable and transfers; linked to math & geometry | Uttal et al. 2013 meta-analysis; Cheng & Mix 2014 |

## 3. What we deliberately exclude or demote

| Drill | Grade | Finding | Decision |
|---|---|---|---|
| Working-memory training (n-back, Corsi grid, digit span) | D for math | Improves the trained task; no reliable far transfer to math or IQ | Melby-Lervåg & Hulme 2013; Melby-Lervåg, Redick & Hulme 2016 → optional "fun" mode, v2+ |
| Commercial "brain training" claims | D | Little evidence of far transfer | Simons et al. 2016 → no IQ claims in the app |
| Chess / logic puzzles for math | D | No measurable transfer to math | Sala & Gobet 2016, 2017 → excluded |

## 4. Caveats that shape design

- **Timed pressure** can raise anxiety for some learners (Boaler; Ramirez et al. on math
  anxiety). → Every timed mode has an untimed twin; timers are visible but not punitive.
- Speed only matters once accuracy is high → difficulty adapts on **accuracy first**,
  then response time.
- Tricks must be followed by retrieval drills, or they don't stick.

## 5. MVP priority (payoff ÷ effort)

1. Fact fluency + − × ÷ (A)  2. Spaced/interleaved engine (A)  3. Fractions/decimals/% (A/B)
4. Squares & roots (C, cheap)  5. Primes/factors (C, cheap)  6. Multi-digit mental (B)
7. Vedic tricks (C, user priority)  8. Estimation (B) — v1.1  9. Spatial (A/B) — v2
