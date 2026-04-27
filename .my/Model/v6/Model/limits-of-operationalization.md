# Limits of Operationalization

This file makes explicit which parts of the model are testable today, which require longitudinal data, and which are currently conjecture. It exists to prevent the model from being read as more empirically grounded than it is. Inline **Conjecture —** and **Testable —** markers in the state files point here for context.

## Snapshot-observable

Classifiable from a single observation of behavior or usage telemetry.

- **S0 Baseline vs everything else** — has the person had meaningful AI exposure?
- **S6E Enthusiastic Overuse vs S7B Burnout** — usage volume distinguishes them trivially (high vs near-zero).
- **D-level of a specific interaction** — observable from the interaction itself.

## Longitudinal-only

Distinguishable only with repeated observation, typically across model releases or workflow changes.

- **S2T Trust Evaluation vs S2D Defensive Resistance** — both look like "user testing the tool" in a snapshot. Asymmetric updating on positive evidence is the operative signal, only visible across multiple evaluations.
- **S3B Bargaining vs S7M Maturity** — boundary-movement behavior across multiple model releases. Single-release observation is not enough.
- **S6D Dependent Overuse trajectory** — distinguishing "S6D currently" from "S6D that collapsed into S7B Burnout" requires usage timeseries.
- **S2P vs S2D dressed in ethical language** — cross-domain consistency over multiple months.
- **Direct S3E → S5 vs accelerated S3E → S3B → S5** — observationally indistinguishable on a single observation; the direct path is a theoretical possibility whose existence in practice is unverified.

## Self-report or interview only

Cannot be directly observed; must be inferred from the person's account, with all the contamination that implies.

- **S3E vs S5** with similar surface behavior — internal state matters.
- **S7I Identity Expansion vs S7M Maturity** — both look like "uses AI competently." Identity expansion is internal.
- **S7E Ethical Integration** — reflective stance is unobservable without dialogue.
- **The driver of a dropout** — practical severity and emotional severity per the two-axis split.

## Currently conjecture (not testable as written)

These claims are in the model because they are useful frames, not because they are tested. Each is also marked inline at the point it appears.

- The dual-component stability requirement for S5 (internal reframing + social normalisation).
- S6E + S6R coexistence in startup-flavoured environments; S6D + S6S coexistence in compliance-heavy environments. Based on observation of two cultural archetypes.
- "Most people cycle through the model more than once."
- The cultural-variability section in full. No cross-cultural data has been gathered.
- The Delegation Ceiling construct. Useful as vocabulary; no measurement instrument exists.
- The three-resolution structure for S3X (transition, exit, advocacy). Covers observed responses but has not been validated against a representative sample of displaced workers.

## Softened from V5

- V5 listed "S7V-without-S3E collapse" as a near-certain claim. V6 softens this to: **Testable —** *S7V Evangelism without depth of engagement collapses under hostile questioning.* This is observable across multiple speaking events but is a different and weaker claim than the V5 version.

## Deliberately not in V6

- **Numerical transition probabilities and dwell times.** Adding fabricated numbers is worse than admitting they don't exist.
- **An "Adoption Ceiling" construct at the population level.** A per-person Delegation Ceiling is included; population-wide ceilings are not.
- **Empirical validation.** No claim in this model has been empirically validated.

## What V6 deliberately does not do

- It does not number states ordinally. Identifiers are handles, not orderings.
- It does not provide a numerical intensity formula.
- It does not claim the cultural section is empirically grounded.
- It does not pretend the S3B/S7M heuristic is a measured falsifier.
- It does not promise that the optimistic end states (S7M, S7I, S7V) are available to everyone.
