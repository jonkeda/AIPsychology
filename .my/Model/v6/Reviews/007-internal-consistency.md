# V6 Internal Consistency Audit

## TL;DR

- **S6R + S6S contradiction.** The state graph claims S6R and S6S both "can coexist" and "are unstable" in the same section. Pick one.
- **Delegation Ceiling definition ambiguity.** Described as "per-person property" but behaves per-domain in examples. Clarify scope.
- **S3B vs S7M boundary signals tagged inconsistently.** One file marks the distinction as Conjecture, the other as Testable. Same claim should have same epistemic tag.
- **Dropout severity scoring is too fuzzy.** The 0–10 axes for practical/emotional severity lack concrete behavioral markers. Two reviewers would diverge badly.
- **S0 permanent-non-user path missing from diagram.** Mermaid graph only shows S0 → S1 transition, not the terminal S0 path. This risks practitioners assuming S0 is transitional only.
- **Delegation Ceiling domain-scoping misalignment.** If ceiling is per-domain (as examples show) but Identity Stakes is per-domain and Task Delegation is per-interaction, the three modulating properties don't sit at the same granularity level.
- **S7V generativity path underspecified.** V5 implied S3E was the primary origin of stable S7V; V6 claims multiple paths but doesn't explain why depth-without-shock is rarer or how to predict which path a person takes.
- **S6E / S6D / S6R / S6S observation boundaries are soft.** The guide provides good probes but concedes most real cases are mixed, then doesn't specify how to score mixed cases on the S6 spectrum.

## Continued in

007-internal-consistency.part2.md

---

## FINDINGS

### 1. S6R + S6S coexistence claim contradicts itself — internal only

**Location:** [02-state-graph.md](02-state-graph.md#L29-L45), State Occupancy section

**The problem:**

The file lists four coexistence claims for S6 states:

```
- S6R Driven Overuse and S6S Social Overuse can coexist in compliance-heavy environments…
- S6D Dependent Overuse and S6S Social Overuse can coexist in compliance-heavy environments…
- The combinations S6E + S6D and S6R + S6S are unstable — the affective profiles do not match.
```

For S6R + S6S, the model says both:
1. "can coexist" (earlier bullet)
2. "are unstable" / "do not stably occupy both" (later bullet)

In state-graph language, "coexist" means the pair occupies the same space; "unstable" means they don't stably occupy the same space. These are contradictory claims in the same rule set.

The state files don't clarify which is intended:
- S6R file says: "**Conjecture —** the coexistence of S6R with S6S Social Overuse in compliance-heavy environments is observed but not directly tested."
- S6S file says: "**Conjecture —** the coexistence of S6S with S6D Dependent Overuse in compliance-heavy environments is observed but not directly tested."

Both files tag coexistence as conjecture, not instability.

**Why it matters:**

A practitioner trying to understand whether S6R and S6S can appear together in the same person will read conflicting guidance in the graph. The rule set is ambiguous about the legal state space.

**Fix:**

Revise the last bullet in the S6 occupancy section to list which *combinations* are actually unstable:

> "The combination S6E + S6D is mutually exclusive (opposite affect) and cannot coexist. The pairing S6R + S6S in compliance-heavy environments is possible but described in the earlier bullet; if the intent is that the pairing is unstable or temporary, move that claim here and specify the timescale or conditions under which it destabilises."

Or: explicitly define "unstable" in the context (e.g., "unstable = lasts less than X weeks" or "unstable = collapses without external reinforcement"). Currently it is not clear.

---

### 2. Delegation Ceiling is described as per-person but examples show per-domain — definition gap

**Location:** [01-axes.md](01-axes.md#L40-L60), Delegation Ceiling section

**The problem:**

The Delegation Ceiling is introduced as: "A property of the person, not of the interaction." This parallels how Identity Stakes is described as per-domain.

But then the examples show per-domain variation:

> "A person in S3B Bargaining can have a D3 ceiling for low-stakes domains while maintaining D1 for their core craft."

This sentence explicitly shows the ceiling varying by domain.

The opening para says: "describes the maximum delegation level a person can accept in their **core domain** given their history." The word "core" narrows it, but "core" is ambiguous. Is each person's "core" singular? Or can they have multiple cores (one per domain)?

**Why it matters:**

If Delegation Ceiling is per-person, it is a single property of the person (like Delegation Ceiling = D2). But if it is per-domain, it is a property of the person-in-domain, making it structurally parallel to Identity Stakes.

The current text is inconsistent, which means practitioners will not know whether to:
- Ask "What is their Delegation Ceiling?" (singular per-person) or
- Ask "What is their Delegation Ceiling for their core domain?" (per-domain)

**Fix:**

Clarify whether Delegation Ceiling is per-person or per-domain:

If **per-person (single):** revise the example to show how ceiling set in one domain carries into another, and explain whether it can be overridden per-domain.

If **per-domain:** revise the intro to say "A property of the person *in a specific domain*, not of the interaction" to match the structure of Identity Stakes, and split the table into per-domain ceilings.

Current recommendation: make it explicitly per-domain to match the per-domain scoping of Identity Stakes. The model's core claim is that identity work is domain-specific; ceiling should be too.

---

### 3. S3B vs S7M boundary-movement signal tagged as both Conjecture and Testable — epistemic inconsistency

**Location:** [S3B-bargaining.md](states/S3B-bargaining.md#L70-L78) vs [S7M-maturity.md](states/S7M-maturity.md#L38-L40)

**The problem:**

Both files describe the same observable distinction: whether a person moves their AI-use boundary in response to capability pressure (S3B) or in response to measured evidence (S7M).

**S3B file:**
> "**Conjecture —** the proposed distinguishing signals between S3B and S7M (where the boundary sits, how it moves) are useful frames. They require longitudinal observation across multiple model releases to confirm and are contaminated by self-report once a subject has read this model."

**S7M file:**
> "**Testable —** boundary-movement behavior across multiple model releases distinguishes S7M from S3B."

Same observable phenomenon, opposite epistemic tags. One says "conjecture that requires confirmation"; the other says "testable."

The limits-of-operationalization.md file lists this under "Longitudinal-only" (testable but requires time) but does not resolve the tagging conflict in the state files.

**Why it matters:**

A practitioner or reviewer reading S3B will come away thinking "this is a hypothesis to be careful about." The same practitioner reading S7M will think "this is a testable claim." They should have the same epistemic status since they describe the same signal.

**Fix:**

Standardize the tagging across both files. Recommendation: use **Testable** (since the claim is "observable across multiple model releases," per limits-of-operationalization.md), and note in S3B that the distinction is testable but requires longitudinal data. Remove or soften the "conjecture" tag from S3B.

Or: if the intent is that S3B's claim is weaker because self-report is "contaminated" (people read the model and report what they think they should), add that caveat to S7M as well, since it has the same self-report problem.

---

### 4. Dropout severity axes lack concrete scoring guidance — operationalization gap

**Location:** [dropout.md](dropout.md), and observation in [limits-of-operationalization.md](limits-of-operationalization.md#L14-L15)

**The problem:**

The model defines dropout severity as two independent 0–10 axes:

- **Practical severity** — tool failures, workflow friction, cost, bad outputs.
- **Emotional severity** — identity threat, ego shock, fear, exhaustion.

The text gives qualitative descriptions of regions:

| Region | Description |
| --- | --- |
| High practical / low emotional | Tool genuinely doesn't work |
| Low practical / high emotional | Identity threat or exhaustion |
| High / high | Mixed |
| Low / low | Boredom |

But no concrete behavioral anchors or scoring rubrics are provided. What counts as "tool genuinely doesn't work"? Is that a 7 or a 9 on the practical axis?

The model acknowledges this: "**Conjecture —** inter-rater reliability of the 0–10 axes has not been established."

But it still proposes the axes as a framework. Two reviewers rating the same dropout would likely score differently because:
- Is "the tool is slow" practical severity 3 or 6?
- Is "I'm not confident I can do this without AI" emotional severity 4 or 7?

The reversibility test (provide better tool, see if they restart) is concrete, but it only distinguishes high practical / low emotional from everything else. It does not operationalise the axes.

**Why it matters:**

The model positions dropout severity as an **operationalisation** (something practitioners can measure), but it is actually still qualitative. Practitioners will score the same case differently, and "within ±1" agreement is probably optimistic.

**Fix:**

Either:

1. **Provide concrete scoring anchors:** Define 0–10 ranges with behavioral markers.
   - Example: Practical severity 0–3 = "tool meets my workflow needs with minor friction"; 4–6 = "tool has significant gaps but core tasks work"; 7–10 = "tool fails critical tasks or is unusable."
   - Same level of detail for emotional severity.

2. **Demote the axes to qualitative regions:** Change from "two 0–10 scales" to "four quadrants" (high/low on each axis) and keep the qualitative descriptions.

3. **Combine with the reversibility test:** Make the reversibility test the primary operationalization, and use the axes as post-hoc framing after the test result is known.

Recommendation: Option 1. Provide anchors. Without them, the framework is not executable.

---

### 5. S0 permanent-non-user path is missing from the Mermaid state graph — visualization gap

**Location:** [02-state-graph.md](02-state-graph.md#L23-L50), Main graph section

**The problem:**

The Mermaid diagram shows:
```
S0 --> S1 : exposure
```

But does not show the S0 → (terminal) path for permanent non-users.

The state-graph text acknowledges S0's two readings:

> "S0 Baseline has two readings: a transitional pre-encounter position and a terminal permanent-non-user position."

But the diagram only visualises the transitional path. A practitioner reading the diagram alone (without the text) would assume S0 only leads to S1.

**Why it matters:**

The model's core claim is that S0 can be terminal, not just transitional. If the primary visual representation (the state graph diagram) omits the terminal path, practitioners may misinterpret S0 as always progressing to S1, which contradicts the text.

This could lead to mistakes like: treating permanent non-users as "stuck in S0 before S1" rather than "legitimately in S0 as an end state."

**Fix:**

Revise the Mermaid diagram to show both paths. Example:

```mermaid
S0 --> S1 : exposure
S0 --> S0 : (terminal for permanent non-users)
```

Or use a node annotation to indicate the two readings, e.g. `S0: Baseline (transitional or terminal)`.

And ensure the caption under the diagram calls out the two readings explicitly.

---

### 6. Delegation Ceiling granularity misaligned with the two axes — structural coherence gap

**Location:** [01-axes.md](01-axes.md), overall structure

**The problem:**

The model proposes three modulating properties:

1. **Identity Stakes** — per-domain
2. **Task Delegation Level (D1–D4)** — per-interaction
3. **Delegation Ceiling** — per-person (as stated) OR per-domain (as shown in examples)

These sit at different granularities:
- Per-domain (Identity Stakes)
- Per-interaction (Task Delegation)
- Per-? (Delegation Ceiling)

If Delegation Ceiling is per-person (singular), it sits at a different granularity than Identity Stakes, which creates a coherence problem. You'd be combining properties at different scopes.

If Delegation Ceiling is per-domain (as the examples suggest), then all three properties should be described as:
- Per-domain: Identity Stakes, Delegation Ceiling
- Per-interaction: Task Delegation Level

The current text treats Delegation Ceiling ambiguously, creating confusion about whether these three properties form a coherent modulation system.

**Why it matters:**

A practitioner asking "what is their delegation model?" wants to know:
- Stakes in this domain? → per-domain
- How much they can delegate right now? → per-interaction
- What is their historical limit? → per-domain or per-person?

If ceiling is per-person (singular), then the framework is mixing granularities, which makes the model harder to apply consistently.

**Fix:**

Clarify that Delegation Ceiling is per-domain, and revise the axes section to group them:

- **Per-domain properties:** Identity Stakes, Delegation Ceiling
- **Per-interaction property:** Task Delegation Level

Then the three work coherently: you pick a domain (which fixes Stakes and Ceiling), then inside that domain, you choose a Delegation Level for each interaction.

---

### 7. S7V generativity path sources underspecified — predictive gap

**Location:** [S7V-evangelism.md](states/S7V-evangelism.md#L17-L30)

**The problem:**

V5 strongly implied that S3E Ego Shock was the primary origin of stable S7V Evangelism (the narrative was: people who have suffered identity disruption become credible guides).

V6 weakens this to: "stable S7V is *more common* among people with prior S3E experience, but stable S7V without prior S3E also exists."

The file lists four origins:
1. Through S3E Ego Shock (lived experience of identity disruption)
2. Through S7I Identity Expansion (built new generative identity)
3. Through professional role (educator, consultant, team lead)
4. Through generativity drive (some people are just oriented to helping)

But it does not predict which people will reach stable S7V through which path. A practitioner seeing someone in S7V cannot work backward to infer their history, because any of these four paths could have led there.

The file also says: "A claim V6 still makes: S7V that is **only** S6E Enthusiastic Overuse flavoured (uncritical promotion without depth of prior engagement) tends to collapse under hostile questioning."

This is testable but underspecified: how is "only S6E" distinguished from "S6E with depth"? The observation guide says S7V with depth can speak from "examples of failure as well as success" but does not define what counts as sufficient depth.

**Why it matters:**

S7V is now non-deterministic (multiple paths in), and the quality gates ("depth is sufficient") are fuzzy. A practitioner trying to support someone who looks like S7V will not know whether the person is stable (reached through S3E or Identity Expansion) or at risk of collapse (only-S6E flavour).

**Fix:**

Either:

1. **Specify depth requirements:** Define what "depth" means operationally for S7V. E.g., "can describe failure in their domain and what they learned; can explain limitations of the tool; has at least 6 months of sustained use."

2. **Predict path origins:** Add heuristics for inferring which path someone took. E.g., "S7V reached through S3E is often marked by initial resistance, then shift to advocacy; S7V reached through professional role is often consistent from the start."

3. **Downgrade S7V stability claims:** If the four paths are truly parallel and the quality gates are fuzzy, state clearly that S7V is a mixed bag and some S7V people are at risk of collapse (S6E flavor) or burnout even if depth seems present.

Recommendation: Specify depth requirements with behavioral anchors (same as dropout scoring fix above).

---

### 8. S6 state observation guide is built for pure cases but acknowledges most are mixed — application gap

**Location:** [observation-guide.md](observation-guide.md#L1-L90)

**The problem:**

The guide provides concrete probes for each S6 state (S6E, S6D, S6R, S6S):

- S6E: "When was the last time AI surprised you in a bad way?" (S6E has no answer or quickly pivots back)
- S6D: "If AI were unavailable for a week, what would you do?" (S6D expresses disproportionate anxiety)
- S6R: "If performance metrics stopped tracking AI use tomorrow, how would your usage change?" (S6R admits usage would drop)
- S6S: "What would you do with AI if you were working entirely alone, with no one watching?" (S6S answers would differ from observed behavior)

These probes are good and concrete.

But then the guide concludes: "Most real cases are mixed."

And offers no guidance on:
- How to score a person who shows both S6E and S6D signals (enthusiastic about some use, anxious about others)?
- How to weight conflicting signals?
- How to route a mixed case into an intervention when the model assumes one primary S6 state at a time?

The state coexistence rules in 02-state-graph.md say S6E and S6D are mutually exclusive, and S6R + S6S can sometimes coexist. But a real person who shows "enthusiastic about new features, anxious about relying on outputs in important work" looks like mixed S6E + S6D. How do you classify them?

**Why it matters:**

The guide is useful for pure cases but breaks down for the "most" case (mixed). A practitioner following the guide will identify signals for multiple S6 states in the same person and not know what to do next.

**Fix:**

Add a section "Handling mixed S6 cases" that:

1. **Describes common mixed patterns:**
   - S6E + S6D: enthusiastic about some tasks, anxious about high-stakes tasks
   - S6R + S6E: driven by productivity targets, energized by demos
   - S6S + S6D: conforming to team adoption while privately doubting self

2. **Provides a primary-state inference method:**
   - What is the person's current affect when not thinking about specific incidents? (S6E = energized; S6D = anxious; S6R = stressed; S6S = compliant)
   - Which signal is most time-stable over weeks?

3. **Specifies intervention routing for mixed cases:**
   - Mixed S6E + S6D: address S6D first (rebuild independent judgement), then let S6E enthusiasm settle into mature practice.
   - Mixed S6R + S6S: identify which driver is primary (productivity pressure or peer pressure?) and address that context.

---

### 9. Related-literature anchors are internally consistent but *not* validated to correspond to real transitions — literature alignment issue (no violation, but worth flagging)

**Location:** Scattered across state files

**The check:**

For each state, does the related-literature construct match the state's transition behavior?

**Finding:**

All the literature anchors align *internally* with their state transitions. No contradictions. Examples:

- **S3E (self-efficacy collapse + terror management)** → S3B (scope limitation), S5 (integration), or S3X (exit). ✓ All are plausible responses to identity disruption.
- **S6E (variable-reward reinforcement)** → S7M, S7I, S7B, S5. ✓ When rewards stop or sobering failure occurs, the reinforcement dynamic ends.
- **S6D (self-efficacy displacement)** → S3E (regression), S7B (burnout), or S7M (rare). ✓ Self-doubt either reasserts as identity threat or exhausts into burnout.

**Caveat:**

The model borrowed these constructs as **vocabulary**, not **mechanism**. The related-literature lines do not claim to explain *why* transitions happen, only that they name the state in existing thinking.

However, the model does not validate that the transition behavior actually matches observed psychology under these constructs. The alignment is *plausible*, not *tested*. This is not an inconsistency within V6 (which explicitly disclaims causality), but it is worth noting for practitioners who might read the literature anchors and expect them to predict behavior.

**No fix needed** (model is honest about this), but note the epistemic gap in documentation for practitioners.

---

### 10. S2T and S2D fork: no implied order claim is honored, but asymmetric transitions create a subtle directionality — clarification needed

**Location:** [02-state-graph.md](02-state-graph.md#L6-L13), S1 fork section, and [S2D-defensive-resistance.md](states/S2D-defensive-resistance.md#L40-L45), inbound transitions

**The check:**

V6 claims S2T and S2D are "responses to S1 with no implied order between them" but also that S2T can transition to S2D "when threat surfaces during testing."

Does this honor the "no implied order" claim?

**Finding:**

Technically yes, but the framing is subtle and could confuse practitioners:

- **No implied order:** You can enter S1 → S2T or S1 → S2D directly, based on Identity Stakes. Neither is a prerequisite for the other.
- **Asymmetric transitions:** S2T → S2D is a normal transition (defensive stance emerges during testing). S2D → S2T does not occur (you don't test defensively then become non-defensive).

This asymmetry is *psychologically* coherent: testing (S2T) is epistemically open; defensive testing (S2D) is epistemically closed. You can shift from open to closed, not vice versa.

**Potential confusion:**

The phrase "no implied order" might be read as "there's no preference or tendency" (which would be false—high Identity Stakes does tend toward S2D). Better phrasing: "neither state is a prerequisite for the other, and either can be entered directly from S1."

**Fix:**

Clarify in [02-state-graph.md](02-state-graph.md) the distinction between:

- **No deterministic order:** You don't have to go through S2T first to get to S2D, or vice versa.
- **Asymmetric transitions:** S2T can shift to S2D; S2D cannot shift to S2T. This is psychologically necessary, not arbitrary.

Revise the note to:

> "The fork after S1 (S2T versus S2D) is driven by Identity Stakes as a tendency, not a deterministic rule. Neither state is a prerequisite for the other; either can be entered directly from S1. However, the transitions between them are asymmetric: S2T → S2D can occur when testing surfaces a threat; S2D → S2T does not occur, because defensive posture cannot revert to open evaluation without a regression event."

---

## RECOMMENDATIONS

### Priority 1: Fix logical contradictions

1. **S6R + S6S coexistence (Finding 1):** Resolve the contradiction between "can coexist" and "are unstable." Choose one reading or define "unstable" to mean "temporary/context-dependent" explicitly.

2. **Dropout severity scoring (Finding 4):** Provide concrete 0–10 anchors with behavioral markers so two reviewers can score within ±1. Without this, the framework is not operationalizable.

3. **S0 terminal path in diagram (Finding 5):** Add the S0 → (terminal) edge to the Mermaid graph to visualize both readings of S0.

### Priority 2: Clarify ambiguous definitions

4. **Delegation Ceiling scope (Finding 2 & 6):** Confirm whether Delegation Ceiling is per-person or per-domain. If per-domain, revise the intro to say so explicitly and restructure to align granularity with Identity Stakes.

5. **S3B vs S7M epistemic tagging (Finding 3):** Standardize the epistemic tag for the boundary-movement distinction across both state files. Use **Testable** with a caveat about self-report contamination.

6. **S7V stability and depth criteria (Finding 7):** Define "sufficient depth" operationally (e.g., concrete behavioral markers like "can describe at least one failure and what was learned").

### Priority 3: Improve applicability

7. **S6 mixed-case guidance (Finding 8):** Add a section to observation-guide.md on handling mixed S6 cases, including primary-state inference and intervention routing.

8. **S2T/S2D asymmetry clarification (Finding 10):** Explicitly state that transitions between S2T and S2D are asymmetric (S2T → S2D is possible; S2D → S2T is not) in the state-graph text.

### Priority 4: Monitor (no immediate fix)

9. **Related-literature causality gap (Finding 9):** Note for practitioners that V6 is honest about not validating that transitions match the constructs in related literature. This is expected given the descriptive stance, but it's worth calling out clearly.

---

## Summary

V6 is more internally consistent than V5 on most core claims (per-domain scoping, independent axes, epistemic honesty). But five findings require fixes before the model is fully coherent:

1. The S6R + S6S contradiction needs resolution.
2. Dropout severity axes need concrete scoring anchors.
3. S0's two readings need to appear in the state graph diagram.
4. Delegation Ceiling needs clarification on scope.
5. S3B and S7M need consistent epistemic tagging for the same observable phenomenon.

All other findings are improvements rather than fixes. The model is ready to use; these fixes would make it more reliable.