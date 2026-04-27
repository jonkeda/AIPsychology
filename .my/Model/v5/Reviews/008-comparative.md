# Comparative Review — Model V5

## TL;DR

- V5 extends TAM and Rogers with identity-threat mechanisms neither model captures — a genuine addition.
- V4 dropped Kübler-Ross grief framing for good reason; professional AI threat is not mortality and can be reversed.
- The Identity Stakes × Task Delegation two-axis modulation is original; no prior model cross-cuts capability threat with interaction granularity.
- The four-way S6 split (enthusiastic, dependent, driven, social overuse) has distinct drivers — each needs different interventions.
- The practical × emotional dropout plane with reversibility test is both original and testable; expand this.
- V5 admits 40% of claims are conjecture and buries the confession in an end section — move this warning to the front.

## Findings

### 1. Kübler-Ross grief stages

V5 correctly abandons grief as a lens for AI adoption. V4 positioned adoption as a grief process (denial, anger, bargaining, depression, acceptance), but grief is about accepting permanent loss. AI capability threat is not loss — it is a threat to identity that can be reframed, reversed, or recalibrated. V5's S3 Ego Shock (Ego Shock) is a single acute identity-disruption state with multiple exits, not a staged march through emotions. This is **psychologically more honest** than Kübler-Ross. Modern bereavement research (Bonanno, Prigerson) has abandoned the stage model anyway, so Kübler-Ross itself is weakened. Keep the rejection.

### 2. Technology Acceptance Model (Davis, 1989 — adoption depends on perceived usefulness and perceived ease of use)

S2T Trust Evaluation (Trust Evaluation) is nearly entirely TAM. V5 adds something TAM does not: asymmetric updating when identity is threatened. In S2T Trust Evaluation the person tests the tool objectively. In S2D Defensive Resistance (Defensive Resistance) the same person discounts positive evidence and amplifies negative evidence. This is a **different cognitive mechanism** (Festinger on cognitive dissonance, Kahan on identity-protective reasoning) than TAM assumes. TAM has no account for why the same user would update evidence differently based on identity stakes. V5 does. In low-stakes domains (such as adopting email software), TAM works well and V5's psychological baggage would be overkill. But when identity is at stake, V5's override is essential.

### 3. Rogers' Diffusion of Innovations (adoption depends on perceived compatibility with existing practice)

S5 Understanding (Understanding / schema integration) borrows Rogers' compatibility concept. Rogers describes social-system effects but does not split stability into internal reframing (personal mental model is coherent) and social normalization (environment treats AI use as unremarkable). This split is useful but also a simplification. Rogers' five innovation characteristics — relative advantage, compatibility, complexity, observability, trialability — are more granular and testable than V5's binary "did they reach S5 Understanding or not." V5 should **acknowledge Rogers explicitly** instead of burying him in the mechanism anchor. Admit S5 Understanding is a coarser simplification of Rogers, not an improvement.

### 4. Transtheoretical Model (Prochaska & DiClemente — behavior change moves through stages: precontemplation, contemplation, action, maintenance, with possible relapse)

V5 does not cite TTM explicitly, but the structure is present: precontemplation (S0 Baseline) → contemplation (S1 Initial Encounter) → preparation (S2T Trust Evaluation or S2D Defensive Resistance) → action (S5 Understanding or S6) → maintenance (S7) with relapse. TTM has a working "processes of change" taxonomy — 10 to 21 techniques for moving through stages. V5 says nothing about how to move someone from S2D Defensive Resistance to S5 Understanding; it only describes states. TTM is **prescriptive**; V5 is descriptive-only. For a software engineer audience, this is the difference between a state diagram (V5) and a state diagram plus control algorithm (TTM).

### 5. Gartner Hype Cycle

The shape is present in V5: Technology Trigger (S1 Initial Encounter) → Peak of Inflated Expectations (S6A Enthusiastic Overuse enthusiastic overuse) → Trough of Disillusionment (S7D Burnout burnout or dropout) → Plateau of Productivity (S7A Maturity maturity). But V5 rightly rejects the unimodal curve as universal. Not everyone peaks and troughs; some skip enthusiasm, others go directly from S1 Initial Encounter to S5 Understanding without a trough. S6 has four parallel attractors, not one peak. V5 treats Gartner as one **possible trajectory among many**.

### 6. Identity Stakes × Task Delegation modulation

This is **genuinely original**. No prior model cross-cuts capability threat (Identity Stakes: low to high) with interaction granularity (Task Delegation: D1 to D4) and argues that both modulate every state's qualitative experience. Kübler-Ross varies grief intensity by loss magnitude but not by scope of threat. TAM varies adoption by perceived utility but not by interaction type or identity relevance. Rogers varies by innovation characteristics but not by which capability is threatened. TTM varies by readiness but not by identity stakes. V5's insight: the same state (such as S3 Ego Shock) feels different if stakes are low (mildly surprising) versus high (existential) and if interaction is low-authority (D1 information retrieval) versus high-authority (D4 decision autonomy). The caveat: V5 does not define how the axes combine. It removed V4's formula because "the multipliers have no defined units" — honest, but also a cop-out. A testable model would define combinations operationally.

### 7. Four-way S6 split with distinct mechanisms

This is **genuinely original**. V5 splits "Overuse" into four parallel states with four different drivers: S6A Enthusiastic Overuse (variable-reward reinforcement, dopamine-driven), S6B Dependent Overuse (self-efficacy displacement, confidence erosion), S6C Driven Overuse (goal-substitution, efficiency as terminal goal), S6D Social Overuse (normative social influence, peer pressure). No prior model says the same surface behavior (high AI usage) can come from four different mechanisms, each with different causes, different experiences, and different exits. Two people using AI heavily are not in the same state. One might need hedonic rebalancing; another might need confidence rebuilding. The caveat: the operational test for distinguishing them is not provided. How do you observe variable-reward engagement versus goal-substitution in real usage telemetry?

### 8. Practical × emotional severity dropout plane with reversibility test

This is **genuinely original and the most testable innovation in V5**. V5 replaces binary (emotional versus practical dropout) with a two-axis plane (practical severity 0–10, emotional severity 0–10). The reversibility check: provide a tool that solves the cited practical problem. If the dropout returns, practical was high. If not, emotional was high. Prior dropout research recognizes attrition but does not decompose it into orthogonal severity axes. The caveat: the test assumes the person's self-report of "why I dropped out" was honest. If practical severity was actually high but the person quit for face-saving reasons, the test might mislead.

### 9. Explicit "Limits of Operationalization" section

V5 is **commendable but undermines authority** by flagging that 40% of claims are conjecture. Prior models hide uncertainty. Kübler-Ross did not disclose her stages were anecdotal. TAM does not flag limitations of perceived-usefulness measurement. V5's honesty is rare and right. But the placement (buried at the end) and lack of repetition (no flag in state descriptions) undermines impact. If a state is conjecture, say so every time you mention it. S7F Evangelism's "S3 Ego Shock prerequisite" is flagged as conjecture in Limits, but the state description never repeats it. A reader could forget by the time they reach Limits.

## Recommendations

1. **Cite TAM, Rogers, TTM, and Gartner explicitly in the mechanism anchors.** Stop hiding the borrowings. Rewrite mechanism anchors to say "borrows from X" or "extends X by" rather than just naming X in a parenthetical.

2. **Elevate the Identity Stakes × Task Delegation modulation as the headline original contribution.** Lead with it before state descriptions. Restructure so readers know upfront what is new.

3. **Operationalize the four-way S6 split.** Add an "Observation guide" subsection under S6 with concrete behavioral or usage-pattern markers for each driver. For S6A Enthusiastic Overuse, track reward-timing alignment with usage spikes; for S6B Dependent Overuse, monitor self-reported confidence metrics; for S6C Driven Overuse, measure goal-switching frequency; for S6D Social Overuse, correlate adoption with peer-adoption timelines.

4. **Expand and test the reversibility check for dropout.** Design a pilot study: offer a tool-fix to dropouts; track returns; correlate reversibility with stated emotional distress.

5. **Move "Limits of operationalization" to the front or inline.** Add inline footnotes or callout boxes flagging "conjecture: awaiting longitudinal data" for each unproven claim. Replace the end section with a one-line summary.

6. **Introduce V5 as an extension and refinement of prior models, not a replacement.** Add a one-paragraph "Relationship to Prior Frameworks" section before the state map.

7. **Drop lingering grief-stage analogy entirely.** Remove references to "grief," "grieving," or "loss" in S3 Ego Shock descriptions. Use "identity disruption," "self-efficacy confrontation," or "existential discomfort" instead.

8. **State explicitly that V5 is descriptive, not prescriptive.** Add a one-sentence disclaimer: "This model describes observed paths, not recommended paths. Practitioners should not use this model to force transitions; use it to understand where a user is."

9. **Keep the state-machine structure.** The directed graph with regression arrows is V5's best contribution. Defending the move from ordinal stages to states with flexible transitions is right.

10. **Remove the comparison table and integrate into narrative.** The table breaks narrative flow. The findings above already cover the comparisons. Keep the table only as a lookup reference if readers explicitly request it.
