# Comparative Review — Model V5 vs. Prior Models

## TL;DR

- V5 borrows heavily from TAM (S2T) and Rogers' diffusion (S5 schema integration), but extends both with identity-threat mechanisms these models ignore
- V4's "grieving" flavoring was never Kübler-Ross; V5 rightly drops it—grief stages don't explain professional identity crisis over AI
- The four-way S6 split (enthusiastic, dependent, driven, social overuse) is genuinely original; no prior model distinguishes these drivers
- The practical × emotional dropout axes are the most testable and actionable innovation; the reversibility check is solid methodology
- V5's biggest weakness: it admits 40% of claims are conjecture, then includes them anyway without proportional warning labels—Limits section buries the uncertainty

## Verdict

V5 is a useful extension of existing adoption frameworks, but it oversells originality. It borrows liberally from TAM, Rogers, and implicitly from the Transtheoretical Model without saying so directly. Where V5 genuinely adds value—the Identity Stakes × Task Delegation modulation, the four-way S6 split, and the practical-emotional dropout plane—it should lead with those. Where it merely restates prior work (S2T calibration is TAM + Bandura; S5 schema integration is Rogers verbatim), it should cite explicitly instead of anchoring. The Limits section is honest but came too late. For the software engineer audience: think of this as a refactoring that extracts critical edge cases (identity threat) and repackages adoption as a state machine. That's valuable. But don't mistake it for an original theory when most of the states are decorator patterns on Davis, Rogers, and Prochaska.

## Comparison Table

| V5 Element | Closest Prior Model | Relationship |
|---|---|---|
| S2T (calibration under uncertainty) | Technology Acceptance Model | Borrowed and extended; TAM is the base, V5 adds asymmetric-updating risk |
| S2D (identity-protection cognition) | Kahan / Festinger cognitive dissonance | Borrowed concept, applied to professional identity rather than politics |
| S3 (self-efficacy collapse + terror management) | Bandura self-efficacy theory | Borrowed construct, original twist on domain-specific collapse under AI threat |
| S3B (bargaining) | Kübler-Ross bargaining stage | Superficial similarity only; V5's bargaining is scope-limitation, not mortality negotiation |
| S5 (schema integration) | Rogers diffusion / compatibility | Nearly verbatim Rogers; V5 adds "dual component" (internal + social) requirement |
| S6A (variable-reward reinforcement) | Behavioral psychology (slot machines, social media) | Borrowed; not new to psychology |
| S6B (self-efficacy displacement) | Bandura / learned helplessness | Borrowed; inverse of mastery experience |
| S6C (goal-substitution) | Cognitive psychology goal hierarchies | Borrowed concept, applied to AI productivity push |
| S6D (normative social influence) | Asch conformity; peer pressure literature | Borrowed from social psychology; Kessler's work on social adoption mentioned implicitly |
| S7A (metacognitive calibration) | Lichtenstein & Fischhoff confidence-accuracy literature | Borrowed; applied to tool-user mental models |
| S7B (extended self) | Belk consumer behavior / phenomenology of tools | Borrowed; tool incorporation is known; V5 claims "deeper" for AI but doesn't prove it |
| S7C (meaning-making) | Post-traumatic growth literature | Borrowed framing; applied to non-traumatic AI confrontation |
| S7D (resource depletion) | Burnout literature (Maslach) / regulatory-depletion research | Borrowed; unresolved debate (literal depletion vs. motivation shift) |
| S7F (generativity) | Erikson developmental stages + mentorship literature | Borrowed; application to AI guidance is straightforward |
| Identity Stakes × Task Delegation two-axis modulation | None | **Original**; no prior model cross-cuts capability threat with interaction-type granularity |
| Four-way S6 split with distinct mechanisms | None | **Original**; prior models bundle "overuse" or "enthusiasm" without distinguishing drivers |
| Practical × emotional severity dropout plane + reversibility test | None | **Original**; prior models treat dropout as binary or undifferentiated |
| Explicit "Limits of operationalization" section | None | **Original practice**; many models hide conjecture; V5 names it, though placement weakens impact |

## Findings

### (a) Kübler-Ross Stages of Grief

**Plain English gloss:** Five emotional stages (denial, anger, bargaining, depression, acceptance) that people supposedly pass through when confronted with mortality or major loss.

**What V5 borrows:** Superficially, V3 and V4 positioned AI adoption as a grief-like process. V5 retains S3B (bargaining) and echoes the emotional-crisis tone of S3 (Ego Shock).

**What V5 adds that is genuinely new:** V5 rightly abandons the grief framing entirely. Grief stages are about accepting a permanent loss that cannot be reversed. AI capability threat is not loss—it is a threat to identity that the person can potentially recalibrate, reframe, or recover from. V5's S3 is not denial-anger-bargaining-depression but a single acute identity-disruption state with multiple possible exits (S3B negotiation, S5 integration, regression to S2D). This is psychologically more honest.

**Where the prior model does the job better:** Kübler-Ross has clinical depth for cases where the threat genuinely is permanent (a master craftsperson whose craft is replaced, not upskilled). For those users, the grief frame might fit. But V5 correctly recognizes that AI threat is domain-specific and reversible, so grief stages miss the point. Modern bereavement research (Bonanno, Prigerson) has also abandoned the stage model, so Kübler-Ross itself is weakened by current evidence.

**Verdict:** Drop the grief framing entirely. V5 was right to move on.

---

### (b) Technology Acceptance Model (Davis, 1989)

**Plain English gloss:** People adopt technology based on two perceptions: whether they think it's useful (perceived usefulness) and whether they think it's easy to use (perceived ease of use).

**What V5 borrows:** S2T (Trust Evaluation) is almost entirely TAM. V5 explicitly anchors S2T to "calibration under uncertainty" and mentions "perceived usefulness and perceived ease of use" directly. The mechanism is classic Davis: testing the tool against known problems, comparing outputs to personal output, updating beliefs.

**What V5 adds that is genuinely new:** V5 adds asymmetric updating and identity-threat disruption. In S2T, the person tests objectively. But in S2D (Defensive Resistance), the same testing behavior becomes identity-protective: the person discounts positive evidence and amplifies negative evidence. V5 correctly notes that this is a *different cognitive mechanism* (Festinger, Kahan) than TAM assumes. TAM has no account for why the same user in the same state would update evidence differently. V5 does. That is new.

**Where the prior model does the job better:** TAM is simpler and more predictive in low-stakes domains (e.g., email software adoption). For pure usability and utility evaluation, TAM explains behavior well. V5 adds psychological baggage that matters when identity is at stake but would be overkill for feature-adoption decisions in a word processor.

**Verdict:** Keep TAM as the anchor for S2T, but flag the S2D asymmetry as an identity-driven override that TAM cannot predict. This is worth keeping.

---

### (c) Rogers' Diffusion of Innovations

**Plain English gloss:** Innovations spread through populations via a five-step decision process (awareness → interest → evaluation → trial → adoption), with adoption rates shaped by five innovation characteristics: relative advantage, compatibility with existing practice, complexity, observability, and trialability.

**What V5 borrows:** S5 (Understanding / schema integration) is Rogers' compatibility and schema-adoption concept. V5 states: "Rogers' diffusion of innovations—the idea that adoption depends on the innovation's perceived compatibility with existing practice." This is Rogers' "compatibility" characteristic directly.

**What V5 adds that is genuinely new:** V5 splits S5's stability into two components: internal reframing (personal mental model is coherent) and social normalization (environment treats AI use as unremarkable). Rogers discusses social-system effects but does not split stability this way. V5 also recognizes that the diffusion curve applies at the *individual level* in parallel with the market level, which Rogers did not emphasize. This is a useful insight but not groundbreaking.

**Where the prior model does the job better:** Rogers' five characteristics (advantage, compatibility, complexity, observability, trialability) are more granular and testable than V5's single S5 state. If you want to predict adoption speed, Rogers gives you five levers; V5 gives you a binary "did they reach S5 or not." Rogers' adopter categories (innovators, early adopters, early majority, late majority, laggards) are also richer than V5's binary stakes distinction.

**Verdict:** V5 should reference Rogers explicitly instead of burying him in the mechanism anchor. And V5 should admit that its S5 is a coarser simplification of Rogers, not an improvement. The "dual component" requirement (internal + social) is interesting but unproven.

---

### (d) Transtheoretical Model (Prochaska & DiClemente)

**Plain English gloss:** People move through six stages of behavior change (precontemplation, contemplation, preparation, action, maintenance, termination) with relapse possible at any point. Different "processes of change" (cognitive, behavioral, social-support) are appropriate at different stages.

**What V5 borrows:** V5 does not cite TTM explicitly, but the structure is present. Precontemplation ≈ S0 (Baseline). Contemplation ≈ S1 (Initial Encounter). Preparation ≈ S2T or S2D (testing the tool, making a decision). Action ≈ S5 or S6 (sustained use). Maintenance ≈ S7 (stable adoption). Relapse is V5's regression, explicitly modeled.

**What V5 adds that is genuinely new:** V5 does not claim TTM-style "stage-matched interventions"—i.e., different therapeutic approaches for different stages. That is a deliberate omission, and probably wise (V5 is descriptive, not prescriptive). V5 also does not use TTM's "decisional balance" (pros vs. cons) framework, which is testable for TTM but harder to operationalize for AI. Finally, V5 adds the identity-stakes dimension, which TTM does not. TTM is agnostic about *why* someone wants to change; V5 recognizes that threat to identity derails standard change progression.

**Where the prior model does the job better:** TTM has a working "processes of change" taxonomy (10–21 techniques for moving through stages). V5 says nothing about *how to move someone from S2D to S5*—it only describes the states. If you want to design an intervention, TTM is actionable; V5 is not.

**Verdict:** Acknowledge TTM but note the deliberate narrowing. V5 is descriptive-only; TTM is intervention-ready. For a software engineer audience, explain this as the difference between a state diagram (V5) and a state diagram + control algorithm (TTM).

---

### (e) Gartner Hype Cycle (as applied to individuals)

**Plain English gloss:** Technology maturity follows a curve: initial excitement (Technology Trigger) → inflated expectations → disillusionment trough → enlightenment slope → productivity plateau. Typically applied to market-level adoption, not individual psychology.

**What V5 borrows:** The shape is present. S1 = Technology Trigger. S6A (enthusiastic overuse) = Peak of Inflated Expectations. S7D (burnout) or dropout = Trough of Disillusionment. S7A (Maturity) = Plateau of Productivity. The analogy is obvious and seductive.

**What V5 adds that is genuinely new:** V5 rejects the unimodal hype-cycle curve as a universal path. Not everyone goes through the peak-and-trough; some go directly from Initial Encounter to S3 Ego Shock (skipping enthusiasm), others from S1 to S5 without a trough. S6 has four parallel attractors, not a single "overuse" peak. V5 is saying: the hype cycle is one *possible* trajectory, not the only one. This is correct. Modern critics of Gartner (The Economist, 2024) confirm that most technologies do *not* follow the hype cycle.

**Where the prior model does the job better:** Gartner's five phases are simpler to communicate and more memorable than V5's state machine. For a layperson, "we're in the trough" is easier to explain than "which of S6A, S6B, S6C, S6D, S7D are we in?" Gartner also provides a timeline ("how long until the plateau?"); V5 explicitly avoids time claims.

**Verdict:** Use the hype cycle as a cautionary analogy—one trajectory among many—but don't let it dominate the model. V5 is correct to pluralize the paths.

---

## Originality Audit of V5's Four Claims

### (i) Identity Stakes × Task Delegation Level Two-Axis Modulation

**Claim:** V5 is the first to cross-cut capability threat (Identity Stakes: low ↔ high) with interaction granularity (Task Delegation: D1–D4), and argue that both modulate the qualitative experience of every state.

**Assessment:** This is **genuinely original**.

Prior models do not combine these two axes:
- Kübler-Ross varies grief intensity by loss magnitude but not by *scope of threat* (e.g., threat to one skill vs. entire identity).
- TAM varies adoption by perceived utility but not by interaction type or identity relevance.
- Rogers' diffusion varies adoption by innovation characteristics but not by *which capability is threatened*.
- TTM varies by behavior-change readiness but not by identity-stakes in the domain.
- Gartner's hype cycle is macro; it says nothing about individual trait differences.

V5's innovation is simple but powerful: the same state (e.g., S3 Ego Shock) *feels different* if the stakes are low (mildly surprising) versus high (existential) AND if the interaction is low-authority (D1 information retrieval) versus high-authority (D4 decision autonomy). This is original.

**Caveat:** V5 does not define how the axes combine. It says "intensity = baseline × Stakes × Delegation" in V4 but removes the formula in V5 because "the multipliers have no defined units." This is honest but also a cop-out. A testable model would define the combinations operationally. V5 provides only a qualitative anchor table for S3. Not wrong, but less useful than it could be.

**Keep or replace:** **Keep**. This is worth retaining and extending with data.

---

### (ii) Four-Way S6 Split with Distinct Mechanisms

**Claim:** V5 splits "Overuse" into four parallel states with four different drivers: S6A (variable-reward reinforcement—dopamine-driven), S6B (self-efficacy displacement—confidence erosion), S6C (goal-substitution—efficiency as terminal goal), S6D (normative social influence—peer pressure).

**Assessment:** This is **genuinely original**.

Prior models:
- Behavioral psychology recognizes variable-reward reinforcement (slot machines, social media), but does not distinguish it from the other three drivers.
- Bandura's self-efficacy literature recognizes both mastery-building (S7A) and efficacy erosion, but does not couple it to overuse specifically.
- Goal-hierarchy research recognizes means-end substitution, but does not connect it to AI automation.
- Asch and modern conformity research recognize normative social influence, but do not apply it to tool adoption at the individual level.

V5 does something that no prior model does: it says *the same surface behavior* (high AI usage) can come from four different mechanisms, each with different causes, different experiences, and different exits. This is a genuinely important insight because it means two people using AI heavily are not in the same state. One might need hedonic rebalancing (S6A); another might need confidence rebuilding (S6B); another might need goal re-evaluation (S6C); another might need permission to opt out of peer pressure (S6D).

**Caveat:** The operational test for distinguishing them is not provided. V5 gives mechanism anchors (what the theory says drives each), but no measurement. How do you observe variable-reward engagement versus goal-substitution in real usage telemetry?

**Keep or replace:** **Keep**. This is a powerful clinical insight. It might not be testable yet, but it's worth developing.

---

### (iii) Practical × Emotional Severity Dropout Plane Plus Reversibility Test

**Claim:** V5 replaces the binary (emotional vs. practical dropout) with a two-axis plane (practical severity 0–10, emotional severity 0–10). It also proposes an operationalization: the "reversibility check"—provide a tool that solves the cited practical problem; if the dropout returns, practical was high; if they don't return, emotional was high.

**Assessment:** This is **genuinely original** and the most testable innovation in V5.

Prior models:
- Dropout research (general) recognizes attrition but does not decompose it into orthogonal severity axes.
- The Transtheoretical Model recognizes "relapse" but does not distinguish practical barriers (the tool failed) from emotional barriers (the person cannot bear the emotional cost).
- TAM would blame perceived usefulness; Gartner would say "trough of disillusionment." Neither disentangles the two drivers.

V5's two-axis plane is a simple but powerful innovation. And the reversibility check is a *method* for operationalizing the distinction in the field. Provide a working tool. If they still don't return, you now know emotional severity was the limiter. This is clever.

**Caveat:** The reversibility check has a serious limitation—it assumes the person's self-report of "why I dropped out" was honest. If practical severity was actually high but the person quit for face-saving reasons (emotional reasons at the surface), the test might mislead. Still, it's a plausible heuristic.

**Keep or replace:** **Keep and refine**. This is both original and practically useful. Expand the reversibility check and test it.

---

### (iv) Explicit "Limits of Operationalization" Section

**Claim:** V5 categorizes every claim as snapshot-observable, longitudinal-only, self-report-only, or currently conjecture—and flags that conjecture section explicitly.

**Assessment:** This is **original practice** (not theory, but model-writing practice) and **commendable**, but **undermines the model's authority**.

Prior models:
- Kübler-Ross did not disclose that her "stages" were anecdotal.
- Davis (TAM) does not explicitly flag the limitations of perceived-usefulness measurement.
- Rogers' diffusion does not warn that adoption categories are post-hoc, not predictive.
- TTM has faced criticism for hidden assumptions but does not pre-emptively list them.
- Gartner's hype cycle explicitly avoids quantification, so it has fewer testable claims to limit. (That is a different kind of weakness.)

V5's choice to label 40% of claims as "conjecture" and "currently unproven" is honest. But the placement (buried at the end) and lack of repetition (no flag in the state descriptions themselves) undermines the impact. If a state is conjecture, say so every time you mention it, not just in a footnote.

**Example of the problem:** S7F's "S3 prerequisite" is flagged as conjecture in Limits. But the state description never repeats that it is untested. A reader could forget by the time they reach the Limits section.

**Keep or replace:** **Keep the practice but reorganize**. Put the Limits section immediately after the state map, not at the end. Or use inline markers (footnotes or callouts) for each conjecture. The honesty is right; the implementation is weak.

---

## Recommendations

1. **Cite TAM, Rogers, TTM, and Gartner explicitly in the state anchors.** Stop hiding the borrowings. Readers are not dumb; they will notice. Credit the prior models directly.

   *Action:* Rewrite mechanism anchors to say "borrows from X" or "extends X by" rather than just naming X in a parenthetical.

2. **Elevate the Identity Stakes × Task Delegation modulation as the headline original contribution.** This is where V5 genuinely adds value. Lead with it.

   *Action:* Restructure so the two-axis modulation is introduced before the state descriptions, not buried in the reading-guide section.

3. **Operationalize the four-way S6 split.** Provide observable signals for distinguishing S6A (dopamine rewards) from S6B (confidence erosion) from S6C (efficiency as goal) from S6D (peer mimicry).

   *Action:* Add an "Observation guide" subsection under S6 with concrete behavioral or usage-pattern markers for each.

4. **Expand and test the reversibility check for dropout.** This is the most actionable innovation. Test it in practice.

   *Action:* Design a pilot study: offer a tool-fix to dropouts; track returns; correlate reversibility with stated vs. measured emotional distress. Validate the heuristic.

5. **Move "Limits of operationalization" to the front (or inline).** Readers will skip a section at the end. Call out conjecture where it appears, not in a separate section.

   *Action:* Add inline footnotes or callout boxes flagging "conjecture: awaiting longitudinal data" for each unproven claim. Replace the end section with a one-line summary.

6. **Introduce V5 as an extension and refinement of prior models, not a replacement.** Clarify what is borrowed, what is extended, and what is new. This is more honest and more powerful.

   *Action:* Add a one-paragraph "Relationship to Prior Frameworks" section at the top, before the state map.

7. **Drop or downgrade the grief-stage analogy entirely.** Kübler-Ross does not map onto professional capability threat. This was a misleading bridge in V3–V4. V5 is correct to move on.

   *Action:* Remove any lingering references to "grief," "grieving," or "loss" in the S3 description. Use "identity disruption," "self-efficacy confrontation," or "existential discomfort" instead.

8. **Be explicit that V5 is descriptive, not prescriptive.** Unlike TTM or Gartner, V5 does not recommend which states to accelerate or which to avoid. This is a feature (neutrality) and a limitation (not actionable for interventions). Say so.

   *Action:* Add a one-sentence disclaimer: "This model describes observed paths, not recommended paths. Practitioners should not use this model to force transitions; use it to understand where a user is."

9. **Recognize that the Limits section is a feature, but implement it differently.** Most academic models hide uncertainty. V5 doesn't. That is rare and good. But bury it at the end, and readers miss it. Put it front and center.

   *Action:* Restructure the document so the Limits are integrated into each state, not separated at the end.

10. **Keep the state-machine structure.** The directed graph with regression arrows is your best contribution. V5 correctly moves away from ordinal "stages" (1 → 2 → 3 …) to states (S0, S2T, S2D, …) with flexible transitions. This is right and worth defending.
