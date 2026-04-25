# V3 → V4 Diff Review

Reviewer lens: Prompt J from [005-prompts-v4.md](../005-prompts-v4.md). Evaluate V4 as a diff against V3. For each change: improvement, lateral move, or regression?

Sources: [Model3.md](../../Model/v3/Model3.md), [Model4.md](../../Model/v4/Model4.md).

---

## TL;DR

- **Net assessment: V4 is a real improvement, but smaller than it presents itself.** Of the eight headline changes, three are improvements, three are lateral, two are mixed.
- **Best changes:** the S6 split (V3 had four subtypes glued under one stage; V4 makes them first-class), and removing V3's "Stage 7E Regression Loop" (it was never a destination, only a property).
- **Worst change:** the S1.5 numbering. Calling it "1.5" while insisting numbers aren't ordinal is self-defeating — it tells the reader the opposite of what the reading guide says.
- **Cosmetic but defensible:** "stages" → "states" and the state-machine diagram. The vocabulary change is honest about what the model already was, but doesn't add predictive power on its own.
- **Oversold:** the falsifiable markers on S3B/S7A. The change is real (V3 had no markers at all) but V4 calls them "falsifiable" when they are at most "in-principle testable with a study you haven't designed." See [003-model4-falsifiability.md](003-model4-falsifiability.md) for the full takedown.
- **Missed opportunities (V3 problems V4 didn't fix):** no transition probabilities, no dwell times, no mechanism anchoring, the intensity formula is still pseudo-math, the Cultural Variability section is still unfalsifiable, the trigger ⚡ markers are still inconsistent.
- **Should anything be reverted in V5?** Only the "1.5" label. Rename to S2A or fold its content into S1's reading guide. Everything else V4 changed should stay.

**Verdict:** V4 earned the version bump on substance (S6 split, dropout split, regression refactor) but earned only half of what it claims on rigor (the falsifiability story is aspirational). Keep the structural changes; patch the rhetoric.

---

## Contents

1. [The eight headline changes, scored](#1-the-eight-headline-changes-scored)
2. [V3 problems V4 should have fixed but didn't](#2-v3-problems-v4-should-have-fixed-but-didnt)
3. [V4 changes that should be reverted in V5](#3-v4-changes-that-should-be-reverted-in-v5)
4. [Recommendations](#4-recommendations)

---

## 1. The eight headline changes, scored

### 1.1 "Stages" → "states" + state-machine framing

**Score: lateral move, defensible.**

V3 already said "the cycle is not linear — it loops" and listed regression triggers. V4 doesn't change what the model *does*; it changes what it claims to *be*. That's honest editorial work, not new architecture.

The state-machine framing is more accurate than "stages" because:

- V3's stage numbers strongly implied an ordinal sequence (people read "Stage 4" as "after Stage 3"), then V3 had to keep correcting that implication with prose ("can be entered from 1A, 3B, or 5"). V4's "states are identifiers, not ordinals" is the cleaner version of the same content.
- V3's "Stage 7E Regression Loop" was a category error inside the stage taxonomy. State-machine framing makes it obvious why.

The framing is **lateral on predictive power.** Calling something a state machine without specifying transition probabilities is a vocabulary upgrade, not a model upgrade. V4 is honest about not specifying probabilities — but it should also be honest that the upgrade is therefore terminological.

**Verdict: keep. Don't oversell it.**

### 1.2 S1.5 (Trust Evaluation) promoted out of the emotional path

**Score: improvement, with a labeling regression.**

V3's Stage 4 (Trust Evaluation) was numbered after Stage 3 (Ego Shock), implying you reach it through the emotional path. V3 then had to spend a paragraph saying "actually, low-identity users skip 2 and 3 and go straight to 4." That was a constant tension in V3.

V4 fixes the *content* problem correctly: Trust Evaluation now sits early in the graph as the natural path for low-stakes users, and is reachable from S1 directly. This is right.

But V4 fixes it with the **worst possible label.** "S1.5" is a fractional number in a system that just spent a paragraph telling the reader numbers aren't ordinal. The reader is now juggling two contradictory rules: (a) the numbers don't mean order, (b) except this one, which means "between 1 and 2." Pick one.

**Verdict: keep the structural promotion. Rename. Suggested: S2 → S2D (Defensive), S1.5 → S2T (Trust). Or drop the digit entirely and use semantic IDs.**

### 1.3 Removing V3's Stage 1B Dismissal (folded into S2)

**Score: improvement.**

V3's Stage 1B was Stage 1A's twin under a hidden user attribute (high vs low identity stakes). That meant the same observable behavior — dismissal — was assigned to two different stages depending on who the person was. That's a bad taxonomy: you can't classify the behavior without first classifying the person.

V4's solution is correct: dismissal is one state (S2 Defensive Resistance), and the user attribute is moved into the Identity Stakes axis where it belongs. Same content, cleaner factoring.

**Verdict: keep. This is one of V4's best changes.**

### 1.4 Splitting V3's Stage 6 into four parallel S6 states

**Score: improvement.**

V3 had Stage 6 as "Overcompensation" with four subtypes (6A–6D) listed underneath. The subtypes had genuinely different drivers (dopamine, anxiety, productivity pressure, peer pressure) and exit paths, but were lumped under one stage label.

V4 promotes them to first-class states. This matters because the V3 framing implied a single "Overcompensation phase" people pass through, when in practice the four subtypes are different attractors entering from different upstream states (S6B specifically inherits from S3, S6D from social context, etc.). The graph encodes this; the V3 nesting hid it.

V4 also adds the multi-occupancy claim ("a person can occupy more than one simultaneously"). That's correct in practice — V3 implicitly required you to pick a subtype, which doesn't match observed behavior.

**Verdict: keep. Best structural change in V4.**

### 1.5 Adding "falsifiable markers" to S3B and S7A

**Score: improvement on substance, oversold on rigor.**

V3 had no way to distinguish bargaining (3B) from healthy maturity (7A) — both were "bounded adoption." The model treated them as different states without telling you how to tell them apart. V4 adds an explicit marker: under capability pressure, S3B users move their lines reflexively; S7A users move them only on evidence.

The conceptual content is right. The rhetorical wrapper isn't. As reviewed in [003-model4-falsifiability.md](003-model4-falsifiability.md), the marker:

- Requires a triggering event to apply (no test between releases)
- Uses an arbitrary observation window ("a week")
- Depends on intent attribution ("reflexively") that isn't directly observable
- Is wide open to self-report contamination once anyone reads the model

Calling this "falsifiable" is a stretch. "Heuristic distinction with an obvious operationalization path" would be honest.

**Verdict: keep the marker. Downgrade the language or add a study protocol.**

### 1.6 Removing V3's Stage 7E Regression Loop

**Score: improvement.**

V3 listed "7E Regression Loop" alongside end states like Maturity and Burnout. That was a category error — regression isn't a destination, it's a transition you can take from any state to any earlier state. V3 had to acknowledge this in the prose ("a person in any stable end state can be pushed back…") which contradicted the taxonomy itself.

V4 deletes 7E and recasts regression as a property of every transition. This is correct and overdue.

**Verdict: keep. Cleanest single edit in V4.**

### 1.7 The Identity Stakes × Task Delegation Level intensity calculus

**Score: mixed. Right factoring, wrong formula.**

The factoring is right. V3 conflated person-level identity attachment with interaction-level delegation depth into a single "delegation depth axis," which produced contradictions (a high-identity user at D1 was sometimes Stage 1A, sometimes Stage 2, depending on which paragraph you read). V4 splits these into two axes — Identity Stakes (per-domain, per-person) and Task Delegation Level (per-interaction). That's a real advance.

The formula is wrong. `intensity = baseline × Identity Stakes × Task Delegation Level` has no units, no scale, undefined baseline, and a binary multiplied by a 4-level ordinal. It's pseudo-math. V3 at least had the honesty to present the same content as a qualitative table.

**Verdict: keep the two-axis split. Delete the formula. Keep the qualitative anchor table.**

### 1.8 The dropout-mechanism split (emotional vs practical)

**Score: lateral move, sometimes a regression.**

V3 already had this split. It was in V3's "Dropout Mechanisms" section with the same names, similar definitions, and the same warning about wrong interventions. V4's text is slightly cleaner but the substance is V3's.

What V4 adds:

- Practical dropout is now reachable from "every state, including S7A." V3 located it mostly at Stages 2, 4, 6. The expansion is correct.

What V4 didn't fix:

- The binary framing is still wrong. Most real dropouts are mixed (tool fails AND failure lands on identity). Both V3 and V4 present a clean either/or. See [003-model4-falsifiability.md, section 1.4](003-model4-falsifiability.md).

**Verdict: lateral. The "every state" expansion is good; the binary framing should have been replaced with two severity axes in V4 and wasn't.**

---

## 2. V3 problems V4 should have fixed but didn't

These are issues present in V3 that V4 inherited unchanged.

### 2.1 No transition probabilities or dwell times

V3 said the cycle "loops" and that "most people cycle through more than once." V4 calls itself a state machine. Neither version specifies how often, how fast, or with what probability any transition fires. A state machine without transition rates is a directed graph.

This is the biggest unaddressed gap. A V5-scale change.

### 2.2 No mechanism anchoring

V3 named stages descriptively (Defensive Resistance, Ego Shock, Bargaining). V4 kept the same descriptive names. Neither anchors states to underlying cognitive mechanisms (cognitive dissonance, threat appraisal, self-efficacy, identity-protection cognition). This is what makes the model vulnerable to the "folk psychology" critique — and V4 didn't address it.

### 2.3 The intensity formula was pseudo-math in V3 too

V3 had "psychological weight = stage × delegation depth" implicitly. V4 made it explicit and worse by formalizing it as multiplication. Neither version is operational.

### 2.4 Cultural Variability is unfalsifiable in both versions

V3 introduced the section. V4 copied it nearly verbatim. In both, every cultural pattern is described as a modulation of intensity/duration/flavor while "core structure holds." No observation could refute that. V4 missed the chance to specify what cultural data would force structural revision.

### 2.5 Trigger ⚡ markers inconsistent

V3 used ⚡ inconsistently — some states had them, some didn't, with no rule for when they should appear. V4 kept the convention and the inconsistency.

### 2.6 The "internal reframing + social normalization" requirement for S5 stability

V3 introduced this. V4 kept it. It's unfalsifiable in both: any observed discomfort gets attributed to mismatch, any observed stability to alignment. No instrument is specified for either component.

---

## 3. V4 changes that should be reverted in V5

Only one.

### 3.1 The "S1.5" label

The numbering convention is the worst kind of inconsistency: it explicitly contradicts the reading guide that introduces it. The reading guide says numbers are identifiers, not ordinals. The label `1.5` is an ordinal expression. The reader is asked to remember that one specific identifier means "between 1 and 2," but the others don't mean anything sequential. That's two contradictory parsing rules running in the same line of text.

**Fix:** rename. Either:

- **Semantic relabel:** S2D (Defensive), S2T (Trust). Both are responses to S1, neither is "before" the other.
- **Drop the digit:** Trust Evaluation = `Eval`, Defensive Resistance = `Defense`, etc. Lose the numbers entirely. The graph carries the structure; the numbers add nothing.
- **Worst case if you keep numbers:** S1A and S1B for the post-S1 fork. Avoids fractions, signals the branch.

Everything else V4 changed should stay.

---

## 4. Recommendations

Prioritized for a V4.1 patch (rhetoric and labels) vs deferred to V5 (structure and dynamics).

### V4.1 patch (do now)

1. **Rename S1.5.** Pick any of the three options in section 3.1. This is the single most visibly broken thing in V4.
2. **Downgrade the falsifiability language** on S3B/S7A markers, OR add a one-page study protocol appendix. See [003-model4-falsifiability.md, Priority 1](003-model4-falsifiability.md).
3. **Delete the intensity formula.** Keep the qualitative table.
4. **Mark unfalsifiable claims** (Cultural Variability, S5 dual-component stability, S7F-without-S3, "most people cycle more than once") with an inline note that they're conjecture rather than tested predictions.
5. **Fix ⚡ trigger marker consistency.** Either apply the convention everywhere it would apply or drop it.
6. **Replace the binary dropout split** with two severity axes (practical 0–10 × emotional 0–10). Carry over from [003-model4-falsifiability.md, Priority 4](003-model4-falsifiability.md).

### V5 (defer until you have data or have decided to anchor in mechanism)

1. **Transition probabilities and dwell times.** Architectural change.
2. **Mechanism anchoring per state.** Architectural change. See Prompt E in [005-prompts-v4.md](../005-prompts-v4.md).
3. **Cultural Variability that specifies what would refute it.** Either operationalize or scope-limit explicitly.
4. **Resolve Adoption Ceiling.** Either commit to it as a first-class construct with rules, or remove the optional-extension paragraph entirely.

---

**Bottom line on the diff:** V4 earned the version number on three solid structural improvements (S6 split, dropout-state cleanup via 1B fold, 7E removal), one good factoring (the two-axis split), and one good but oversold addition (the markers). The single regression is the S1.5 label. None of the V4 changes need to be reverted in V5 except that label. The big work that V4 didn't do — dynamics, mechanism, falsifiable cultural claims — is what V5 is for. Don't start V5 yet; ship V4.1 first.
