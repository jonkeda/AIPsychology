# Structural Critique — Model V5

## TL;DR

- **S2T/S2D fork is not a clean dichotomy.** The model specifies S2T → S2D transition ("testing surfaces a threatening capability"), which makes this a conditional sequence, not a parallel fork determined by prior Identity Stakes.
- **S3B vs S7A distinction is unmeasurable.** Both show "bounded adoption" in surface behavior. The heuristic distinguisher (boundaries change under pressure vs. after evidence) is untestable, self-report-contaminated, and operationally hollow.
- **S6 states are not parallel.** Model text says combinations occur in specific cultures (S6A+C in startup, S6B+D in compliance cultures), suggesting constraints or ordering, not true parallelism.
- **S3 → S5 edge is missing from state diagram.** Text specifies this transition; diagram doesn't show it.
- **Multi-occupancy rules for S6 are unspecified.** Can S6A and S6B coexist? S6 and S7 simultaneously? No explicit constraints given.
- **S7A/B/F are not behaviorally distinguishable from mechanism anchors alone.** Distinguishing "mature calibration" from "identity expansion" from "generativity" requires internal state inference, not observable behavior.
- **S6B lacks transition explanation.** The mechanism anchor (self-efficacy displacement) doesn't explain why S3 (identity collapse) leads to S6B (high dependent usage).

## Verdict

V5 tightened the model's epistemic register and added mechanism anchors, which is good. But the structural commitments inherited from V4 contain unforced errors: the S2T/S2D fork is asserted as a dichotomy but specified as a sequence; the S3B/S7A distinction is operationally empty; the S6 states are claimed as parallel but constrained in ways the model doesn't acknowledge. These are not prose problems. They are graph problems. Fixing them requires renaming, merging, or reordering — not just clarifying the existing structure. The model is also missing operational rules for multi-occupancy and missing a documented edge in the state diagram.

---

## Findings

1. **S2T/S2D is not a parallel fork; it's a conditional sequence.** The model states that Identity Stakes determines whether S1 leads to S2T or S2D. But S2T's transitions specify: "→ **S2D Defensive Resistance** — testing surfaces a threatening capability." This means a person can enter S2T on low-stakes grounds and *discover* that their concern was wrong, moving them to S2D mid-evaluation. This undermines the claim that the fork is parallel and clean. The fork is actually determined partly by *prior* Identity Stakes (low stakes → S2T typically) and partly by *discovered outcome during testing* (test surfaces threat → S2D). This is a sequence with a branch, not two independent paths.

2. **S3B and S7A cannot be distinguished behaviorally from mechanism anchors alone.** Both describe "bounded adoption" — the person uses AI for some purposes, not others. The model attempts to distinguish them with a heuristic: "In S3B, boundaries are renegotiated **under capability pressure**. In S7A, boundaries move **only after measured evidence**." The model itself admits this is "a **heuristic**, not a measured fact...contaminated by self-report once a subject has read this model." This heuristic is not operationalized. No instrument exists to measure "capability pressure" vs "measured evidence" independently of self-report. Once a subject reads the model, they will rationalize their boundary changes as data-driven to appear in S7A rather than reactive to appear rational. The heuristic fails as a structural distinction.

3. **S6 states are claimed as parallel attractors but the model specifies they occur in constrained combinations.** The model states: "They are distinct attractors that pull from different upstream causes...A person can occupy more than one simultaneously — the most common combinations are S6A + S6C in startup cultures, and S6B + S6D in compliance-heavy cultures." If only certain combinations occur reliably, the states are not parallel; they have ordering or incompatibility constraints. The model doesn't specify why S6A+C and S6B+D are common while (presumably) S6A+B and S6C+D are rare or absent. If S6A (enthusiastic, high positive affect) and S6B (anxious, confidence-eroding) are both *simultaneously* high, the person would experience conflicting affect states. Are they genuinely compatible, or does the model fail to acknowledge that they're mutually exclusive? This needs explicit documentation.

4. **State diagram omits S3 → S5 direct transition.** The ASCII state map shows S3 branching to either S3B or onward, with the path S3B → S5 shown. But the S3 state description explicitly says: "Transitions: → **S5 Understanding** — direct integration when the person can hold the full confrontation." The diagram doesn't show this direct edge. This is a missing edge in the graph, either in the diagram or in the text description.

5. **Multi-occupancy rules are absent.** The model specifies that S7 states are "long-term patterns...not mutually exclusive" and that "most adapted users settle into a combination (S7A + S7C…S7B + S7F)." It also states S6 states "can occupy more than one simultaneously." But there are no rules governing *which* states can coexist. Can you be in S6A (enthusiastic, high-reward seeking) and S6B (dependent, low-confidence) at the same time? Can you be in S6A and S7A simultaneously? In S6B and S7A? The model gives no constraints. Without these, the state space becomes incoherent — every person could theoretically occupy any combination, which destroys the model's predictive structure.

6. **S7A, S7B, and S7F are not behaviorally distinguishable when only mechanism anchors are available.** The model distinguishes S7A ("knows when to use and when not"; mechanism: metacognitive calibration) from S7B ("identifies as a writer-with-AI"; mechanism: extended-self/tool incorporation) from S7F ("teaches others"; mechanism: generativity). These are internal psychological constructs. Two independent reviewers given only the mechanism anchors and no access to the person's self-report could not reliably assign the same label. How would you tell if a person's identity *includes* the AI tool (S7B) vs. whether they simply use the AI tool competently within their existing identity (S7A) from behavior alone? You cannot. This is not a measurement problem; it's a structural problem. The states are defined by internal experience, not by externally observable transitions or outcomes.

7. **S6B mechanism anchor doesn't explain the transition from S3 to S6B.** S6B is anchored to "self-efficacy displacement" — the person outsources judgment to AI rather than building their own. But the model also says S6B "inherits its trigger from the upstream S3 episode rather than from any current event." So S3 (identity collapse under capability threat) somehow leads to S6B (high AI usage driven by self-doubt). The mechanism anchor doesn't explain this transition. Why would identity collapse lead to high usage? The anchor suggests S6B is about *replacing* one's confidence with AI's, but the model doesn't explain why that would happen *after* an identity shock. A person in S3 (existential threat) might either withdraw (regression) or seek refuge (S6B), but the mechanism doesn't predict which. This is a missing causal link.

8. **S3B stability claim is contradicted by its own transition spec.** The model claims S3B ("bounded adoption with self-imposed scope") is "not a failure state — many people remain productive here for years." But S3B's transitions include "→ **S3 Ego Shock** — capability jump shatters the bargain." If the bargain is regularly shattered by capability jumps (which happen frequently in the AI domain), S3B is not a stable state; it's a temporary holding pattern. The claim of stability is undermined by the transition rule that destabilizes it. Either (a) redefine S3B as a temporary coping state (not stable), or (b) add a mechanism that explains why some people's bargains persist across capability jumps while others' shatter.

9. **Identity Stakes × Task Delegation composition is undefined.** The model specifies both axes as independent, but then gives a qualitative intensity table under S3 showing how they compose (Low×D1 → mild surprise; High×D4 → existential). The model removed the V4 intensity formula because "multipliers have no units." But without any composition rule, the axes become decorative. A practitioner cannot predict the experiential intensity of a state without knowing whether the axes multiply, add, or interact in some other way. The model describes composition qualitatively but not formally, leaving it underspecified.

10. **S2T mechanism anchor (calibration under uncertainty) is generic, not distinctive.** The anchor ties S2T to the Technology Acceptance Model — people adopt tech if they think it's useful and easy. But this mechanism applies to *any* technology evaluation, not specifically to low-stakes AI adoption. What makes S2T distinctive is not the mechanism but the outcome: low-stakes people test without ego defense. The mechanism anchor doesn't explain *why* low-stakes people are non-defensive or why high-stakes people are defensive. The anchor seems chosen for familiarity rather than for explanatory specificity. Compare with S2D, anchored to "identity-protection cognition" — that is specific and distinctive. S2T's anchor is too generic to serve its structural role.

11. **S7F requires a prior S3 experience but this prerequisite is conjecture and untested.** The model states: "Most stable when the person has previously passed through S3. Lived experience of Ego Shock is what makes them credible to others currently in it; without that experience, the advocacy tends to be naive (S6A flavor) or compelled (S6D flavor) and collapses under the first hostile question." This is stated as a heuristic, not a tested claim. But it's also stated as a structural property of the state — it's not marked as conjecture in the state description itself, only in a note at the end. This creates ambiguity: is S7F stable without S3 or not? If the S3 prerequisite is structural, it should be in the state definition. If it's conjecture, it shouldn't constrain the transitions.

12. **Removal of Adoption Ceiling from V4 left a gap in the model's coverage.** V5 states: "If a use case requires it, that use case justifies V6." But there's no documentation of what Adoption Ceiling was or what gap its removal created. A mature user who consciously decides to use AI only for D1 tasks due to deliberate professional choice (not identity bargaining) should fit somewhere in the model. Is this person in S7A (mature calibration)? Or is there a missing state for "I've adopted AI but I've chosen a low ceiling on delegation deliberately"? The removal is unexplained.

---

## Recommendations

### Priority 1: Restructure the S2T/S2D fork as a sequence, not a parallel fork.

**Change:** Rename the fork to reflect that S2T is the *entry point* to evaluation (low Identity Stakes) and S2D is reachable *either from S1 directly* (high Identity Stakes, typical) *or from S2T* (testing surfaces threat). Make the diagram show S2T → S2D as a possible transition and revise the post-S1 fork description.

**Concrete revision:**
- Modify the state map to show S1 → S2T (low stakes, typical) and S1 → S2D (high stakes, typical), but also S2T → S2D (threat surfaces during testing).
- Revise S2T description to clarify it's "non-defensive evaluation, which can convert to defensive evaluation if testing reveals threat."
- Revise the fork description in "Reading this model" to say: "After S1, low-stakes individuals typically enter S2T evaluation; high-stakes individuals typically enter S2D defense. S2T can transition to S2D if testing discovers threat."
- This makes the graph transitively cleaner — the fork is primarily determined by prior Stakes, but outcome-dependent transitions exist.

### Priority 2: Merge S3B and S7A or replace the heuristic with a mechanistic distinction.

**Change:** The current heuristic (boundaries change under pressure vs. after evidence) is not operationalized and is self-report-contaminated. Two options:

**Option A (Merge):** Combine S3B and S7A into a single "Bounded Adoption" state. Then distinguish them by *transition behavior*, not by internal motivation:
- **S7A** (subset of Bounded Adoption): enters from S5, S2T, or later S6/S7 states. Boundaries are *reinforced* by evidence.
- **S3B** (subset of Bounded Adoption): enters from S3 under emotional pressure. Boundaries are *renegotiated downward* when capability jumps occur.
- This makes the distinction observable from *transition history*, not from internal state.

**Option B (Mechanistic redefinition):** Keep S3B and S7A separate but anchor S3B differently. Currently S3B is anchored to "dissonance reduction via scope limitation." Extend this: S3B is dissonance reduction under *active emotional pressure* (S3 precedes it; the person must manage ongoing anxiety). S7A is not. This makes the mechanism anchors themselves distinctive, not a heuristic about future behavior.

**Recommendation:** Use Option A (merge and distinguish by transition history). The heuristic approach is inherently unreliable. Transition history is observable.

### Priority 3: Document the ordering constraints and mutual-exclusivity rules for S6 states.

**Change:** Specify whether S6A, S6B, S6C, S6D can coexist, are partially ordered, or have domain-specific constraints.

**Concrete revision:**
- Add a section after the S6 overview clarifying: "**Multi-occupancy constraints:** S6A (enthusiastic, high positive affect) and S6B (dependent, high anxiety) are experienced as incompatible by most people and rarely coexist. S6C (productivity-driven) and S6D (conformity-driven) can coexist in high-performance cultures where productivity *is* the norm."
- OR: Document that S6A+C and S6B+D are stable combinations, and that S6A+B and S6C+D are unstable or absent. Explain why.
- Add rules for coexistence with S7 states (e.g., "S6A (high usage, high reward) is compatible with S7A (calibrated use) only if the reward is coming from domains where calibration supports it").

**Rationale:** Without these constraints, the state space is incoherent. Practitioners need to know whether a person can be in two states simultaneously or whether observed combinations predict downstream transitions.

### Priority 4: Add S3 → S5 direct edge to the state diagram and clarify its conditions.

**Change:** The text specifies "S3 Ego Shock...→ S5 Understanding — direct integration when the person can hold the full confrontation." The diagram should show this edge.

**Concrete revision:**
- Update the ASCII state map to include a line from S3 directly to S5 (not only through S3B).
- Add a condition to the S3 transition description: "S3 → S5 (rare; requires the person to fully confront the identity threat without defense or negotiation and rebuild their self-concept immediately)."
- Define what "can hold the full confrontation" means operationally, or mark it as requiring longitudinal observation.

**Rationale:** The diagram is the model's primary specification. It must match the text.

### Priority 5: Add explicit multi-occupancy rules in a new "State Occupancy" section.

**Change:** Create a grid or explicit rules specifying which state combinations are allowed, forbidden, or domain-specific.

**Concrete revision:**
Add a section after the S7 end states:

```
### Multi-Occupancy and Simultaneous States

**S6 states (parallel, with constraints):**
- S6A and S6B are mutually exclusive (opposite affect/motivation patterns).
- S6C and S6D can coexist (productivity and conformity reinforce each other in cultures that value both).
- A person can be in more than one of {S6A, S6C} or {S6B, S6D} simultaneously; uncommon combinations are rare.

**S7 states (parallel, intentionally overlapping):**
- Any S7 state can coexist with any other S7 state (S7A+C, S7B+F are documented; others possible).

**S6 and S7 coexistence:**
- S6 states are high-engagement, typically high-usage phases.
- S7 states are stable long-term patterns.
- S6A (enthusiastic overuse) can transition to S7A or S7B but not coexist with either (overuse is not mature or expanded; it's overextended).
- S6B, S6C, S6D all lead to S7D (burnout) as primary exit. Coexistence with S7 end states is not documented.

**Dropout (reachable from every state):**
- A person in any S state or combination can exit to Dropout.
```

**Rationale:** The model claims multi-occupancy for S6 and S7 but doesn't specify the rules. This confusion makes the model's predictive structure unclear.
