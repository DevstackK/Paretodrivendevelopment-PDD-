---
name: pdd-rapid-delivery
description: Deliver a complete result under an explicit time, token, or iteration constraint using impact-based prioritization and bounded refinement. Use for rapid delivery, token efficiency, limited revision passes, or an explicit 80/20 workflow; not for unconstrained ordinary drafting or analysis.
---

# PDD Rapid Delivery

Deliver the smallest complete result that passes the user's requirements. Optimize outcome quality per token, time, or revision—not resource use alone.

## Rules

- Preserve the requested scope, format, technology, and authorization boundaries.
- Treat security, safety, privacy, accessibility, compliance, accuracy, and data integrity as release constraints.
- Establish the deliverable, audience, acceptance criteria, explicit constraint, and baseline or target when available. Ask only questions whose answers could materially change the result.
- Produce a complete end-to-end version before polishing.
- Classify remaining issues as blockers, high-impact gaps, or optional polish. Fix blockers, then the smallest set of high-impact gaps.
- Prefer targeted, reversible edits over regeneration, alternatives, new dependencies, or abstractions.
- Use one focused refinement pass by default. Continue only for a failed acceptance criterion, unresolved blocker, or high-consequence risk.
- Stop when acceptance criteria pass, no blocker remains, and another pass is unlikely to materially improve the outcome. State unresolved limits without implying verification.

## Efficiency evaluation

When evaluating this skill:

- Keep prompt, model, reasoning level, environment, and checks fixed; vary only skill activation.
- Record input, cached-input, and output tokens, commands, passes, elapsed time, acceptance checks, and blockers when exposed. Label estimates.
- Compare outcome quality per token and command count. Never claim efficiency from shorter output alone.
- Prefer several representative tasks and median results; treat one run as preliminary.

Report measurements only when the user requests evaluation or constrained-delivery reporting.
