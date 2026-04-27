# V4 → V5 Diff Review

## TL;DR

- Mechanism anchors **added**. Each state now tied to a cognitive-science mechanism (novelty appraisal, calibration, identity-protection cognition). Improvement for understanding why states behave as they do, but some anchors rest on unverified assumptions.
- State **renaming** (S1 Initial Encounter.5 → S2T Trust Evaluation, S2 → S2D Defensive Resistance). Clearer labels; removes the confusing `.5` ordinal. Lateral improvement; breaks compatibility with V4 references.
- **Formula deleted**. V4 claimed intensity = baseline × Stakes × Delegation. V5 removes it because it has no units and isn't measurable. Honest move; doesn't fix the underlying problem.
- S3B Bargaining/S7A Maturity distinction **downgraded**. V4 called it "falsifiable"; V5 downgrades to "heuristic." Requires longitudinal observation, contaminated by self-report. Regression in testability.
- Dropout split into **two axes**. Replaces binary emotional/practical with 0–10 severity scores on each axis. Improvement. Adds reversibility test as operationalization.
- **"Limits of operationalization" added**. Categorizes claims as snapshot-observable, longitudinal-only, self-report-only, or conjecture. Intellectual honesty win. Exposes how little is testable.
- Conjecture tags **deployed**. S5 Understanding dual-component stability, S7F Evangelism-without-S3 Ego Shock collapse, "most people cycle more than once," and Cultural Variability section marked as untested.
- Adoption Ceiling **removed**. V4 presented it as optional; V5 drops it. No loss — never deployed anyway.
- V5 is a **defensibility pass**, not an expansion. It removes V4's pseudo-scientific veneer and is more honest. The mechanism anchors add explanatory power if they hold up. The downgrade of S3B Bargaining/S7A Maturity to heuristic, the conjecture tags, and the operationalization section all mark intellectual maturity. V5 also reveals the empirical base is thin: the S3B Bargaining/S7A Maturity distinction relies on longitudinal observation that hasn't happened, S5 Understanding's stability claim is untestable as written, and Cultural Variability is pure conjecture. V5 doesn't fix these — it acknowledges them.

## Findings

### 1. Mechanism anchors per state

**What changed:** V5 anchors each state to an established psychological mechanism. S1 Initial Encounter → novelty appraisal (Lazarus / Folkman); S2T Trust Evaluation → calibration under uncertainty and the Technology Acceptance Model; S3 Ego Shock → self-efficacy collapse (Bandura) plus terror-management threat responses; S3B Bargaining → cognitive-dissonance reduction (Festinger); S5 Understanding → schema integration (Rogers' diffusion theory); S6A Enthusiastic Overuse → variable-reward reinforcement; S6B Dependent Overuse → self-efficacy displacement; S6C Driven Overuse → goal-substitution; S6D Social Overuse → normative social influence (Asch); S7A Maturity → metacognitive calibration; S7B Identity Expansion → extended-self incorporation (Belk); S7C Ethical Integration → meaning-making; S7D Burnout → resource depletion; S7F Evangelism → generativity (Erikson, broadened).

**Why:** V5's introduction states the model was "purely descriptive" before. Adding mechanisms makes it explanatory: you understand not just that someone enters S3 Ego Shock, but why and what cognitive system is engaged.

**Whether it worked:** Partially. The mechanisms are real — all cited from established literature. The problem is they are necessary-but-not-sufficient frames. S3 Ego Shock is anchored to self-efficacy collapse and terror-management threat response, but the model doesn't explain why one person's self-efficacy collapse leads to S3 Ego Shock while another's leads to S3B Bargaining. The mechanism anchors raise the explanatory bar without answering how mechanisms interact or which dominates in any given case. Some are mechanism-shaped conjectures rather than tested claims (see finding 7).

**Verdict:** Keep, but refine. Each mechanism should have a testable prediction attached: "If S3 Ego Shock is primarily self-efficacy collapse, then [specific observable consequence]." Without that, the mechanism is scaffolding, not science.

### 2. S1 Initial Encounter.5 → S2T Trust Evaluation and S2 → S2D Defensive Resistance rename

**What changed:** V4 used S1 Initial Encounter.5 (Trust Evaluation) and S2 (Defensive Resistance). The `.5` implied S1 Initial Encounter.5 was "between" S1 Initial Encounter and S2 — both are responses to S1 Initial Encounter, not ordered steps. V5 renames to S2T Trust Evaluation and S2D Defensive Resistance using first letter to denote response type.

**Why:** Remove notational confusion. The `.5` creates the false impression there is an S2 after S1 Initial Encounter.5.

**Whether it worked:** Yes, but incompletely. S2T Trust Evaluation/S2D Defensive Resistance are clearer than S1 Initial Encounter.5/S2. The renaming breaks references to V4 in existing materials. Two states with the same leading digit risk verbal confusion ("Did you say S2 or S-two-T?"). Notation is technically superior; compatibility cost is real.

**Verdict:** Keep. The introduction should explicitly state: "If you know V4, S2T Trust Evaluation is the old S1 Initial Encounter.5 and S2D Defensive Resistance is the old S2. There is no new S2 — those two states exhausted it."

### 3. Pseudo-formula deletion

**What changed:** V4 stated: "Emotional intensity in any state = baseline × Identity Stakes × Task Delegation Level." V5 removes the formula entirely and replaces it with a qualitative table under S3 Ego Shock.

**Why:** The formula has no units. What is "baseline"? V5 correctly diagnoses this as pseudo-mathematical window-dressing.

**Whether it worked:** Yes. The qualitative table ("Low × D1 = Mild surprise; High × D4 = Existential") is more honest. The cost is that the model forfeits any claim to precision about intensity. That is a correct concession.

**Verdict:** Keep. The model should now explicitly state whether intensity is thought to be additive, multiplicative, non-linear, or unknown.

### 4. "Falsifiable marker" → "heuristic distinction" on S3B Bargaining/S7A Maturity

**What changed:** V4 claims S3B Bargaining and S7A Maturity are "indistinguishable from behavior alone" and offers a "falsifiable marker." V5 keeps the same distinction but downgrades it from "falsifiable" to "heuristic," noting it requires longitudinal observation and is "contaminated by self-report once a subject has read this model."

**Why:** V4's claim was too strong. The distinguishing test (watch the person respond to a model release) is not falsifiable in the Popperian sense — any boundary-movement can be rationalized as either pressure-driven or evidence-driven.

**Whether it worked:** Partially. The intellectual honesty is correct. V5's solution (downgrading to heuristic) is a step backward in testability. A better move would be to propose a different falsifiable test (timeline analysis: if boundaries shifted within weeks of a release without deliberate testing, S3B Bargaining is more likely; if only after measured evaluation, S7A Maturity).

**Verdict:** Refine. Replace the heuristic with a specific operationalization: ask "Walk me through the last time you decided to expand what you use AI for. Was it because the tool became capable of something new, or because you couldn't maintain the boundary anymore?"

### 5. Two-axis dropout plus reversibility test

**What changed:** V4 defines two dropout modes (emotional and practical). V5 replaces them with a 2D space (Practical Severity 0–10, Emotional Severity 0–10). A dropout is a position in the plane. V5 also adds the reversibility check: provide the dropout with a tool that solves their cited problem; if they restart, practical was high; if not, emotional was driving the exit.

**Why:** The binary split misses mixed cases (tool failure that triggered identity threat). The reversibility test is a clever operationalization: instead of asking "Was it emotional or practical?" you do something and observe whether the outcome changes.

**Whether it worked:** Yes for the two axes, partially for the reversibility test. The axes allow common real-world cases (high practical / high emotional). The reversibility test has limits: someone who drops out emotionally might still refuse to re-engage if the new tool carries the same identity threat — the test returns "emotional" but doesn't actually test practical severity. The test assumes the "solution to the cited problem" is what the person actually needs.

**Verdict:** Keep, but note limits. The two-axis model is an improvement. The reversibility test should be described as "tends to work" rather than "definitive."

### 6. "Limits of operationalization" section added

**What changed:** V5 categorizes every claim as snapshot-observable, longitudinal-only, self-report-only, or currently conjecture.

**Why:** V5 explicitly wants to prevent the model from being read as more empirically grounded than it is.

**Whether it worked:** Yes. The section is intellectually honest and useful. It makes explicit what the model is claiming to know and what it is guessing about.

**Verdict:** Keep and expand. For each longitudinal-only or self-report-only claim, propose a specific measurement protocol that would make it testable.

### 7. Conjecture tags

**What changed:** V5 marks four major claims as untested: S5 Understanding stability requires both internal reframing and social normalization; S7F Evangelism is unstable without prior S3 Ego Shock; most people cycle through the model more than once; the entire Cultural Variability section.

**Why:** These claims are useful frames for thinking, not tested. V5 distinguishes "we have evidence" from "this seems plausible but we don't know."

**Whether it worked:** Partially. The honesty is correct. All four are indeed conjectures — plausible, some well-motivated by theory, none empirically verified. Marking something as conjecture is not the same as removing it. The model becomes harder to use if half its major claims are unverified — a reader doesn't know whether to design around the claim or treat it as a placeholder.

**Verdict:** Keep the tags, but refine guidance on use: "A conjecture should be treated as a working hypothesis, not a fact. If you're designing an intervention based on a conjecture, explicitly test whether the predicted outcome occurs. Document any cases where the conjecture fails."

### 8. Adoption Ceiling removed

**What changed:** V4 proposed Adoption Ceiling as an "optional extension" — the idea that a person might be mature at low delegation levels (D1–D2) but in ego shock at high delegation (D3–D4). V5 removes this entirely.

**Why:** Adoption Ceiling was never formalized or used in V4. Removing it reduces clutter without losing substance.

**Whether it worked:** Yes, but the underlying problem persists. Adoption Ceiling was meant to solve a real-world pattern: many people are mature with low-stakes tools (D1) but defensive when the same tools are used for identity-loaded creative work (D3–D4). V5 removes Adoption Ceiling without proposing an alternative. The model is cleaner but less precise about this common case.

**Verdict:** Keep removed; note the gap in recommendations below.

### 9. The ⚡ trigger marker rule is inconsistently applied

V5 formulates the rule: "A state carries ⚡ if and only if at least one named external event materially changes the probability of entering or leaving that state." Placement is inconsistent. S2T Trust Evaluation has no ⚡ ("internally driven and not reliably accelerated or reversed by named external events"), but S2T Trust Evaluation can be re-triggered from S5 Understanding via "looping back to evaluate a new tool or model" — a new model release is an external event. S1 Initial Encounter has ⚡; S5 Understanding doesn't, even though S5 Understanding is the state a person tries to remain in and external triggers commonly push them out.

### 10. Cultural Variability lacks mechanism anchors

V5 acknowledges Cultural Variability is conjecture but still makes specific claims: "High craft-identity cultures amplify S2D Defensive Resistance, S3 Ego Shock, S3B Bargaining." It doesn't say *why* craft identity amplifies S2D Defensive Resistance. Is it that high craft-identity people are more likely to enter S2D Defensive Resistance, experience S2D Defensive Resistance differently, or spend more time there?

### 11. No proposal for how to recover from S6B Dependent Overuse (Dependent Overuse)

S6B Dependent Overuse is described as eroded self-efficacy driven by outsourcing decisions. The transitions listed are "→ S3 Ego Shock (regression) or → S7D Burnout." S6B Dependent Overuse is a particularly nasty state: the person has lost confidence in their own judgment and is checking AI against AI. How does a person escape this while rebuilding self-efficacy? The model suggests regression or burnout as the only exits, but both are costly. A third exit — supported self-efficacy rebuild with structured low-stakes practice — is plausible but not described.

## Recommendations

1. **Operationalize the unfalsifiable conjectures or remove them.** The model's credibility rests on distinguishing what it knows from what it is guessing. Three conjectures are particularly unfalsifiable as written:
   - **S5 Understanding dual-component stability.** "Any observed discomfort can be attributed to mismatch" makes the claim unfalsifiable. Either propose a way to measure each component separately or remove the dual-component claim.
   - **S7F Evangelism-without-S3 Ego Shock collapse.** If you haven't observed anyone in stable S7F Evangelism without prior S3 Ego Shock, what is the evidence for the collapse claim? This is speculation without supporting data.
   - **"Most people cycle more than once."** If purely qualitative, also unfalsifiable. Either propose a measurement (such as "the median person re-enters S3 Ego Shock at least twice over a 5-year period") or drop the claim.

   For each, add: "To test this claim, we would [specific protocol]. This would require [time and cost]. Current status: not yet done."

2. **Operationalize or revise the S3B Bargaining/S7A Maturity distinction.** Either propose a testable operationalization (structured interview, timeline analysis, behavioral prediction), or collapse S3B Bargaining and S7A Maturity into a single "Bounded Adoption" state with sub-conditions.

3. **Propose operationalizations for longitudinal-only and self-report-only claims.** For V6, add a "Measurement protocol" appendix:
   - **S2T Trust Evaluation versus S2D Defensive Resistance:** "Ask the user: Tell me about the last time you tested an AI tool. Did you update your estimate of capabilities based on what you saw, or did you find yourself dismissing positive results while focusing on limitations?"
   - **S3B Bargaining versus S7A Maturity:** "Collect boundary-movement data across three model releases. Code: moved within 1 week of release without published testing data = S3B Bargaining; moved only after announced benchmarks or real-world trials = S7A Maturity."

4. **Address the Adoption Ceiling gap.** Three options:
   - Add a sub-distinction under S7A Maturity (S7A Maturity-D2: calibrated for D1–D2; S7A Maturity-D3+: calibrated for high delegation).
   - Propose a fourth axis, "Delegation Ceiling," tracking the maximum delegation level a person will use.
   - Add a note that a person occupies multiple states simultaneously (S7A Maturity for D1–D2, S3 Ego Shock for D4) and make multi-state occupancy more explicit.

5. **Expand the External Trigger layer.** Distinguish triggers that initiate transitions, accelerate them, and reverse them. Add a trigger-interaction matrix.

6. **Add mechanism interaction rules.** S3 Ego Shock is anchored to both self-efficacy collapse and terror-management threat. Which dominates? Propose: "Self-efficacy collapse dominates for skilled professionals; terror-management dominates for young or early-career users."

7. **Reframe conjectures as hypotheses with experimental designs.** Example: "S5 Understanding stability requires both internal reframing and social normalization. Test: measure internal reframing (pre/post interview on mental-model coherence) and social normalization (peer adoption survey). Compare S5 Understanding users with both versus only one. Predict: the both group has lower dropout. Cost: 6-month study, 50 users, 3 interview rounds."
