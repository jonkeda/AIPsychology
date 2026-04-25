# V4 → V5 Diff Review

## TL;DR

- **Mechanism anchors added.** Each state now tied to a cognitive-science mechanism (novelty appraisal, calibration, identity-protection cognition, etc.). Improvement for understanding *why* states behave as they do, but some anchors rest on unverified assumptions.
- **State renaming (S1.5 → S2T, S2 → S2D).** Clearer labels. Removes the confusing `.5` ordinal. Lateral improvement in clarity, breaks compatibility with V4 references.
- **Formula deleted.** V4 claimed intensity = baseline × Stakes × Delegation. V5 removes it because it has no units and isn't measurable. Honest move; doesn't fix the underlying problem of intensity being non-quantitative.
- **S3B/S7A distinction downgraded.** V4 called it "falsifiable"; V5 downgrades to "heuristic." Requires longitudinal observation and is contaminated by self-report once people read the model. Regression in testability.
- **Dropout split into two axes.** Replaces binary emotional/practical with 0–10 severity scores on each axis. Improvement. Adds reversibility test as an operationalization attempt.
- **"Limits of operationalization" added.** Explicitly categorizes claims as snapshot-observable, longitudinal-only, self-report-only, or conjecture. Intellectual honesty win. Also exposes how little is actually testable.
- **Conjecture tags deployed.** S5 dual-component stability, S7F–without–S3 collapse, "most people cycle more than once," and the entire Cultural Variability section marked as untested. Honest. Weakens the model's empirical footprint.
- **Adoption Ceiling removed.** V4 presented it as optional; V5 explicitly drops it. No loss — it was never deployed anyway. Doesn't solve the underlying problem it was meant to address.

---

## Verdict

V5 is a **defensibility pass**, not an expansion. It removes the pseudo-scientific veneer from V4 and is more honest about what it does and doesn't know. The mechanism anchors add explanatory power if they hold up. The downgrade of S3B/S7A to heuristic, the conjecture tags, and the operationalization section all mark intellectual maturity. However, V5 also reveals that the model's empirical base is thin: the S3B/S7A distinction relies on longitudinal observation that hasn't happened, S5's stability claim is untestable as written, and the Cultural Variability section is pure conjecture. V5 doesn't fix these problems; it just acknowledges them. The mechanisms are useful frames for thinking, not tested theories. The model remains useful for structuring thought about AI adoption, worse at supporting prediction or intervention.

---

## Diff Summary Table

| Change | Direction | Confidence |
| --- | --- | --- |
| Mechanism anchors per state | Improvement | High — anchors clarify causal logic; confidence in specific mechanisms varies |
| S1.5 → S2T, S2 → S2D rename | Lateral (net slight improvement) | High — clearer labels, breaks V4 references |
| Formula deletion | Improvement | High — formula was unworkable |
| S3B/S7A falsifiable → heuristic | Regression | High — less testable, more honest |
| Two-axis dropout | Improvement | Medium-high — reversibility test is clever but not yet validated |
| "Limits of operationalization" section | Improvement | High — transparency about empirical gaps |
| Conjecture tags | Lateral (mixed) | High — honest, but weakens model scope |
| Adoption Ceiling removed | Lateral (net neutral) | High — never implemented, no loss |

---

## Findings

### 1. Mechanism anchors per state

**What changed:** V5 anchors each state to an underlying psychological mechanism from established cognitive science. S1 is tied to novelty appraisal (Lazarus/Folkman); S2T to calibration under uncertainty and the Technology Acceptance Model; S3 to self-efficacy collapse (Bandura) plus terror-management threat responses; S3B to cognitive-dissonance reduction (Festinger); S5 to schema integration (Rogers' diffusion theory); S6A to variable-reward reinforcement; S6B to self-efficacy displacement; S6C to goal-substitution; S6D to normative social influence (Asch); S7A to metacognitive calibration; S7B to extended-self incorporation (Belk); S7C to meaning-making; S7D to resource depletion; S7F to generativity (Erikson, broadened).

**Why it was made:** V5's introduction states the model was "purely descriptive" before. Adding mechanisms makes it explanatory: you understand not just that someone enters S3, but *why* they enter it and what cognitive system is engaged. This is academically stronger and practically useful for designing interventions.

**Whether it worked:** Partially. The mechanisms are real — all are cited from established literature. The problem is that most of them are necessary-but-not-sufficient frames. For example, S3 is anchored to self-efficacy collapse *and* terror-management threat response, but the model doesn't explain why one person's self-efficacy collapse leads to S3 Ego Shock while another's leads to S3B Bargaining. The mechanism anchors raise the explanatory bar without answering how the mechanisms interact or which one dominates in any given case. They are useful for understanding *what kinds of cognition matter* but not for prediction.

Additionally, some mechanisms are mechanism-shaped conjectures rather than tested claims. See Finding 7 below on conjectures.

**Keep / refine / revert:** Keep, but refine. Each mechanism should have a testable prediction attached: "If S3 is primarily self-efficacy collapse, then [specific observable consequence]." Without that, the mechanism is scaffolding, not science.

---

### 2. S1.5 → S2T and S2 → S2D rename

**What changed:** V4 used S1.5 (Trust Evaluation) and S2 (Defensive Resistance) to label two paths from S1. The `.5` implied S1.5 was "between" S1 and S2, which was misleading — both S1.5 and S2 are *responses* to S1, not ordered steps. V5 renames to S2T (Trust Evaluation) and S2D (Defensive Resistance). The new labels use first letter to denote the response type and remove the false ordinal implication.

**Why it was made:** Remove the notational confusion. The `.5` creates the false impression that there is an S2 that comes after S1.5, when actually both branch from S1 and S2 (the old label) doesn't exist as a concept anymore.

**Whether it worked:** Yes, but incompletely. S2T and S2D are clearer than S1.5 and S2. However, the renaming breaks any existing references to S2 in V4 (which many readers may have internalized). Introducing two states with the same leading digit (S2T, S2D) risks confusion in verbal discussion: "Did you say S2 or did you say S-two-T?" The notation is technically superior but the compatibility cost is real.

**Keep / refine / revert:** Keep. The old notation was actively misleading; clearer notation is worth the compatibility break. To minimize confusion, the introduction should explicitly state: "If you know V4, S2T is the old S1.5 and S2D is the old S2. There is no new S2 — those two states exhausted it."

---

### 3. Pseudo-formula deletion

**What changed:** V4 stated: "Emotional intensity in any state = baseline × Identity Stakes × Task Delegation Level." V5 removes the formula entirely and replaces it with a qualitative table under S3: intensity scales with both axes, but there is no numerical formula.

**Why it was made:** The formula has no units. What is "baseline"? What unit is intensity measured in? How are multiplicands defined? If intensity scales as low/high × D1/D2/D3/D4, what is the actual numerical result? The model never specifies. V5 correctly diagnoses this as pseudo-mathematical window-dressing and removes it.

**Whether it worked:** Yes. The qualitative table ("Low × D1 = Mild surprise; High × D4 = Existential") is more honest and more usable. The cost is that the model forfeits any claim to precision about intensity. That is a *correct* concession: the model doesn't have the measurement instruments to support precision.

**Keep / refine / revert:** Keep. The formula deletion is intellectually necessary. However, the model should now explicitly state whether intensity is thought to be additive, multiplicative, non-linear, or something else — or explicitly admit the functional form is unknown.

---

### 4. "Falsifiable marker" → "heuristic distinction" on S3B/S7A

**What changed:** V4 claims S3B and S7A are "indistinguishable from behavior alone" and offers a "falsifiable marker" to tell them apart: In S3B, boundaries move under capability pressure; in S7A, boundaries move under *evidence*. V5 keeps the same distinction but downgrades it from "falsifiable" to "heuristic," notes that it requires longitudinal observation across multiple model releases, and admits it is "contaminated by self-report once a subject has read this model."

**Why it was made:** V4's claim was too strong. The distinguishing test (watch how the person responds to a model release) is not falsifiable in the Popperian sense — any boundary-movement can be rationalized as either pressure-driven or evidence-driven depending on how you interpret the person's motivation. V5 acknowledges that this is a useful heuristic frame, not a clean empirical test.

**Whether it worked:** Partially. The intellectual honesty is correct. S3B and S7A *do* look behaviorally identical (both involve bounded adoption), and V5 is right that the distinction is harder to measure than V4 pretended. However, V5 's solution (downgrading to heuristic) is a step backward in testability. A better move would be to propose a *different* falsifiable test (e.g., timeline analysis: if the person's boundaries shifted within weeks of a release without deliberate testing, S3B is more likely; if they shifted only after measured evaluation, S7A is more likely). V5 doesn't do that; it just admits the problem.

**Keep / refine / revert:** Refine. Accept that the "heuristic distinction" is not a measure, but replace it with a specific operationalization: interview the person with the question "Walk me through the last time you decided to expand what you use AI for. Was it because the tool became capable of something new (evidence), or because you couldn't maintain the boundary anymore (pressure)?" This is still self-report, but it's a direct question rather than an inference.

---

### 5. Two-axis dropout replacing the binary emotional/practical split, plus the reversibility test

**What changed:** V4 defines two dropout modes: emotional (identity threat, fear) and practical (tool doesn't work). V5 replaces them with a two-dimensional space: Practical Severity (0–10) and Emotional Severity (0–10). A dropout is a position in the plane, not a category. V5 also adds the "reversibility check": provide the dropout with a tool that solves their cited problem. If they restart, practical severity was high. If they don't, emotional severity was driving the exit.

**Why it was made:** The binary split misses mixed cases (tool failure that triggered identity threat; workflow friction that landed at an identity-vulnerable moment). The two-axis model is more precise. The reversibility test is a clever operationalization: instead of asking "Was it emotional or practical?" (unanswerable without reading minds), you *do something* and observe whether the outcome changes.

**Whether it worked:** Yes for the two-axis model, partially for the reversibility test. The axes are a legitimate improvement — they allow for the most common real-world cases (high practical / high emotional). The reversibility test is operationally clever and testable in principle. However, it has limits: (1) someone who drops out emotionally might *still* refuse to re-engage if the new tool carries the same identity threat, in which case the test returns "emotional" but doesn't actually test practical severity; (2) the test assumes the "solution to the cited problem" is what the person actually needs, when sometimes the person's problem statement is a rationalization.

**Keep / refine / revert:** Keep, but note the test's limits. The two-axis model is an improvement. The reversibility test is useful but should be described as "tends to work" rather than "definitive."

---

### 6. "Limits of operationalization" section added

**What changed:** V5 adds a new section that categorizes every claim in the model as (a) snapshot-observable (classifiable from a single observation), (b) longitudinal-only (requires repeated observation), (c) self-report-only (observable only via interview), or (d) currently conjecture (not testable as written). Examples: S0 vs everything else is snapshot-observable; S2T vs S2D requires longitudinal data; S3 internal state requires interview; S5's dual-component stability is conjecture.

**Why it was made:** V5 explicitly wants to prevent the model from being read as more empirically grounded than it is. The section forces the author (and reader) to ask: what evidence would actually test this claim? And often, the answer is "we don't have it."

**Whether it worked:** Yes. This section is intellectually honest and useful. It does two things right: (1) it makes explicit what the model is claiming to know, (2) it makes explicit what the model is guessing about. Any practitioner using the model should read this section first.

**Keep / refine / revert:** Keep and expand. The operationalization section should be expanded for V6 to include: for each longitudinal-only or self-report-only claim, propose a specific measurement protocol that *would* make it testable. (Example: for "most people cycle through the model more than once," propose: monthly interviews with a cohort of 100 users over 18 months, tracking state membership by [specific behavioral / interview criteria]. This would cost X and take Y time.)

---

### 7. Conjecture tags on S5 dual-component stability, S7F-without-S3, "most people cycle more than once," and Cultural Variability section

**What changed:** V5 marks four major claims as currently untested conjecture: (1) S5 stability requires both internal reframing *and* social normalization; (2) S7F is unstable without prior S3; (3) most people cycle through the model more than once; (4) the entire Cultural Variability section. Each is tagged with a note like "This is currently conjecture. No instrument is specified for either component."

**Why it was made:** These claims are in the model because they are *useful frames for thinking*, not because they are tested. V5 distinguishes between "we have evidence for this" and "this seems plausible but we don't know." This is intellectually mature.

**Whether it worked:** Partially. The honesty is correct. All four claims are indeed conjectures — they are plausible, some are well-motivated by theory, but none have been empirically verified. The problem is that marking something as conjecture is not the same as *removing* it, and the model becomes harder to use if half its major claims are unverified. A reader doesn't know whether to design around the claim or treat it as a placeholder.

Example: "S5 stability requires both internal reframing and social normalization" is a conjecture. But what does a designer do with it? If they believe it, they should design interventions to support both components. If they're skeptical, should they ignore it? The conjecture tag doesn't answer the question.

**Keep / refine / revert:** Keep the tags, but refine V5's guidance on how to use conjectures. Add a section like: "Using conjectures in practice: a conjecture should be treated as a working hypothesis, not a fact. If you're designing an intervention based on a conjecture, explicitly test whether the predicted outcome occurs. Document any cases where the conjecture fails."

---

### 8. Adoption Ceiling removed

**What changed:** V4 proposes Adoption Ceiling as an "optional extension": the idea that a person might be mature at low delegation levels (D1–D2) but still in ego shock at high delegation (D3–D4). V5 removes this optional extension entirely and states: "V4 introduced this as an optional extension. V5 removes the option. If a use case requires it, that use case justifies V6."

**Why it was made:** Adoption Ceiling was never formalized or used in V4. Removing it reduces clutter without losing substance.

**Whether it worked:** Yes, but the underlying problem persists. Adoption Ceiling was meant to solve a real-world pattern: many people are mature with tools used for low-stakes information work (D1) but defensive or shocked when the same tools are used for identity-loaded creative work (D3–D4). V4 identified this pattern but couldn't formalize it. V5 removes Adoption Ceiling without proposing an alternative. The model is now *cleaner* but *less precise* about this common case.

**Keep / refine / revert:** Keep (don't re-add Adoption Ceiling), but note the gap in the findings section below.

---

## V4 Elements That Should Have Changed But Didn't

### The "⚡ trigger marker" rule is inconsistently applied

V5 formulates the rule: "A state carries ⚡ if and only if at least one named external event materially changes the probability of entering or leaving that state." However, the placement is inconsistent.

Example: S2T (Trust Evaluation) has no ⚡ marker, with the note "S2T is internally driven and is not reliably accelerated or reversed by named external events." But S2T can be re-triggered from S5 via "looping back to evaluate a new tool or model," and a new model release is an external event. Why no ⚡?

Example: S1 has ⚡ (compressed by mandates, peer adoption, demos), but S5 doesn't, even though S5 is the state a person tries to remain in and external triggers commonly push them out of it (capability jump, visible failure, workplace change). The rule seems applied inconsistently.

**Recommendation:** Either apply the ⚡ rule consistently and document the reasoning, or move the trigger discussion outside the state descriptions and into a separate "Trigger interactions" section.

### Cultural Variability section lacks mechanism anchors

V5 acknowledges that Cultural Variability is conjecture. However, it still makes specific claims: "High craft-identity cultures amplify S2D, S3, S3B." But it doesn't say *why* craft identity amplifies S2D. What is the mechanism? Is it that high craft-identity people are more likely to enter S2D, or that they experience S2D differently, or that they spend more time there? V5 doesn't distinguish.

**Recommendation:** For V6, add mechanism anchors to cultural claims: "High craft-identity cultures amplify S2D because [mechanism]. Predicted outcome: [testable consequence]."

### No proposal for how to recover from S6B (Dependent Overuse)

S6B is described as eroded self-efficacy driven by outsourcing decisions. The transitions listed are "→ S3 Ego Shock (regression) or → S7D Burnout." But S6B is a particularly nasty state: the person has lost confidence in their own judgment and is checking AI against AI. How does a person *escape* this while rebuilding self-efficacy?

V4 doesn't address this. V5 inherits the problem. The model suggests regression (S3) or burnout (S7D) as the only exits, but both are costly. A third exit — supported self-efficacy rebuild with structured low-stakes practice — is plausible but not described.

**Recommendation:** For V6, propose "S6B → S5 via structured judgment exercises" and describe what that looks like operationally.

---

## V5 Changes To Revert In V6

### Do not keep the S3B/S7A "heuristic distinction" as-is

V5's solution to the S3B/S7A problem (downgrade to heuristic) is intellectually honest but operationally weak. A person reading the model might ask: "Which state am I in?" and the only answer is "observe your boundary movement over several model releases." That is not actionable.

**Recommendation:** For V6, either (a) propose a testable operationalization (structured interview, timeline analysis, behavioral prediction), or (b) collapse S3B and S7A into a single "Bounded Adoption" state with sub-conditions. The heuristic distinction should not survive unchanged.

### Remove conjectures that are currently unactionable

Three conjectures in V5 are problematic because they are unfalsifiable as written:

1. **S5 dual-component stability.** V5 states: "stability has two components, both required: internal reframing and social normalization. *Note: the dual-component requirement is currently conjecture.*" But the note also says: "any observed discomfort can be attributed to mismatch." If discomfort can be attributed to mismatch between internal and social components, then the claim is unfalsifiable — any discomfort is explained away. Either propose a way to measure each component separately (internal reframing score: X, social normalization score: Y) or remove the dual-component claim.

2. **S7F-without-S3 collapse.** V5 notes: "The 'S3 prerequisite for stable S7F' claim is currently conjecture. A future longitudinal study could refute it." But if you haven't observed anyone in stable S7F without prior S3, what is the evidence *for* the collapse claim? This is speculative in the wrong direction — it is a prediction without supporting data.

3. **"Most people cycle more than once."** V5 notes: "More than once" is qualitative. V5 deliberately avoids numerical claims." But if the claim is purely qualitative, it is also unfalsifiable (what counts as "more than once"?). Either propose a measurement (e.g., "the median person re-enters S3 at least 2 times over a 5-year period") or drop the claim.

**Recommendation:** For V6, either add falsifiability structures to these claims or remove them.

---

## Recommendations

### Priority 1: Operationalize the unfalsifiable conjectures or remove them

The model's credibility rests on distinguishing between what it knows and what it is guessing. V5 does this well. But guesses should have exit criteria: a way to either confirm or refute them. The three conjectures listed above are currently non-falsifiable, which means they are not guesses — they are just assertions.

For each conjecture, add: "To test this claim, we would [specific measurement protocol]. This would require [time and cost]. Current status: not yet done."

### Priority 2: Propose operationalizations for longitudinal-only and self-report-only claims

V5 correctly identifies that many states can only be classified via interview or longitudinal observation. But the model doesn't specify *what to ask* or *what to measure*. For V6, add a "Measurement protocol" appendix:

- **S2T vs S2D operationalization:** "Ask the user: 'Tell me about the last time you tested an AI tool. Did you update your estimate of the tool's capabilities based on what you saw (S2T), or did you find yourself dismissing positive results while focusing on limitations (S2D)?' Record whether the user's subsequent behavior matched their self-report."
- **S3B vs S7A operationalization:** "Collect boundary-movement data across three model releases. Code: moved within 1 week of release without published testing data = S3B; moved only after announced benchmarks or real-world trials = S7A."

### Priority 3: Address the Adoption Ceiling gap

The model identifies the pattern (mature at D1–D2, shocked at D3–D4) but has no clean way to represent it. Rather than re-introduce Adoption Ceiling, propose an alternative:

Option A: Add a sub-distinction under S7A (e.g., S7A-D2: "calibrated for D1–D2"; S7A-D3+: "calibrated for high delegation") to track this.

Option B: Propose a fourth axis, "Delegation Ceiling," orthogonal to Identity Stakes, that tracks the maximum delegation level a person is willing to use.

Option C: Add a note that a person occupies *multiple* states simultaneously (S7A for D1–D2, S3 for D4) and make multi-state occupancy more explicit throughout the model.

### Priority 4: Expand the External Trigger layer

V5 lists trigger types (model release, workplace mandate, media narrative) but doesn't distinguish between triggers that initiate transitions vs. triggers that accelerate them vs. triggers that reverse them. For V6, add a trigger-interaction matrix:

| Trigger | Effect on S1→S2D | Effect on S2D→S3 | Effect on S5→S7A | Effect on S7→S3 (regression) |
| --- | --- | --- | --- | --- |
| Model release | Speeds | Massive | Possible | Strong |
| Workplace mandate | Massive | Minimal | Minimal | Weak |

This would move the trigger discussion from implicit annotations to explicit prediction.

### Priority 5: Add mechanism interaction rules

V5 adds mechanism anchors but doesn't specify when one mechanism overrides another. Example: S3 is anchored to both self-efficacy collapse *and* terror-management threat. Which dominates? Is there a rule? For V6, propose: "Self-efficacy collapse dominates for skilled professionals (X evidence); terror-management dominates for young or early-career users (Y evidence)."

### Priority 6: Reframe conjectures as hypotheses and propose experimental designs

Rather than leaving conjectures as placeholders, reframe them as testable hypotheses and propose what experiments would test them:

- **Hypothesis:** S5 stability requires both internal reframing and social normalization.
  - **Test:** Measure internal reframing (pre/post interview on mental model coherence) and social normalization (peer adoption survey). Compare S5 users who have both vs. only one component. Predict: the "both" group has lower dropout and slower regression.
  - **Cost:** 6-month study, 50 users, 3 interview rounds.

This moves conjectures from "we're not sure" to "we know how to find out."
