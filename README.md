# Pareto-Driven Development: PDD Rapid Delivery

`pdd-rapid-delivery` is a compact Codex skill for delivering the smallest complete result under an explicit time, token, or iteration constraint. It applies Pareto prioritisation to refinement while keeping production-quality controls mandatory.

## What it optimises

- Outcome quality per token, unit of time, or revision pass.
- Complete end-to-end delivery before optional polish.
- Blockers and the highest-impact gaps before cosmetic improvements.
- Targeted, reversible changes instead of broad regeneration.
- Evidence-based stopping rules.

PDD does **not** trade away security, safety, privacy, accessibility, compliance, accuracy, or data integrity. Those remain release constraints.

## Install

Clone the repository and copy it into your Codex skills directory:

```bash
git clone https://github.com/DevstackK/Paretodrivendevelopment-PDD-.git
mkdir -p ~/.codex/skills/pdd-rapid-delivery
cp Paretodrivendevelopment-PDD-/SKILL.md ~/.codex/skills/pdd-rapid-delivery/SKILL.md
```

For a repository-scoped installation, place the file at:

```text
.codex/skills/pdd-rapid-delivery/SKILL.md
```

## Use

Invoke it explicitly when the request has a real delivery constraint:

```text
Use $pdd-rapid-delivery to build the smallest production-ready slice within two weeks.
```

It is intentionally not aimed at ordinary, unconstrained drafting or analysis.

## Preliminary A/B result

The skill was tested on an identical ecommerce-dashboard task using the same model configuration, seed files, environment, sandbox, and acceptance gate. Only skill activation changed.

| Metric | Without skill | With compact PDD | Change |
| --- | ---: | ---: | ---: |
| Input tokens | 256,365 | 227,395 | -11.3% |
| Output tokens | 14,106 | 12,122 | -14.1% |
| Total reported tokens | 270,471 | 239,517 | **-11.4%** |
| Delivered code | 36,381 bytes | 29,947 bytes | **-17.7%** |
| Changed lines | 131 | 68 | **-48.1%** |
| Commands | 8 | 11 | +37.5% |
| Enterprise quality gate | Passed | Passed | No detected regression |

At published GPT-5.6 Sol standard API-equivalent rates on 6 November 2026, the measured runs were approximately:

| Run | Estimated model cost |
| --- | ---: |
| Without skill | $0.4224 |
| With compact PDD | $0.4046 |
| Saving | **$0.0178 / 4.2%** |

### Quality gate

Both artifacts passed checks for JavaScript syntax, diff integrity, complete static assets, accessible markup, reduced-motion support, persistent local state, CSV export, event handling, dialog workflows, and responsive styling. Browser rendering could not be verified because Chromium was restricted in the evaluation environment.

### Important limitation

This is a **single-task preliminary result**, not a universal performance claim. Model runs vary. A reliable benchmark should use several representative tasks, identical conditions, deterministic checks, and median results. The command count also increased in this run, so further refinement should focus on eliminating redundant environment and browser-capability checks.

## Skill size

- 30 lines
- 285 words
- 2,112 bytes

The earlier draft contained 641 words. The compact version reduced instruction words by 55.5% while preserving its core constraints and evaluation rules.

## Evaluation principles

For credible comparisons:

1. Keep the task, model, reasoning effort, environment, and acceptance checks fixed.
2. Change only whether the skill is activated.
3. Measure input, cached-input, output, commands, passes, elapsed time, blockers, and outcome quality.
4. Treat quality regression as failure even when token usage falls.
5. Use several representative tasks and compare medians.

## Repository contents

- `SKILL.md` — the installable Codex skill.
- `README.md` — usage, evaluation method, and preliminary results.
