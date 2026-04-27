# Adversarial / Steel-Man Critique — Plain-Language Version

This is a simpler rewrite of [004-adversarial.md](004-adversarial.md). Same findings, plain language. If you've read the original and it landed, skip this one.

## What this review is doing

The other reviews try to help. This one attacks. The job is to find the weakest parts of V5 and push on them hard, the way a hostile reviewer would. If a claim survives this, it's probably real. If it falls apart, you needed to know.

## TL;DR

- **Mechanism anchors** (the psychology-jargon labels V5 attaches to each state) don't actually explain anything. They're nicknames, not engines.
- The new "Limits of operationalization" section is V5 admitting it can't measure its own core distinctions. Those weren't fresh limits discovered in V5 — they were always there. V4 just didn't say so.
- V5 is V4 with humbler claims and longer footnotes. Same states, same axes, same transitions. The new bits are admissions of what can't be measured, plus mechanism labels with no tested predictions.
- The 2D dropout plane (Practical severity 0–10, Emotional severity 0–10) has no scoring rule, no data, and an "operational test" that's circular.
- The model attaches "identity-protection cognition" (the thing where people reject information that threatens their sense of self) to four different states. If one mechanism explains four states, it doesn't tell them apart — it just says "people protect their identity, full stop."
- The model now says any later state can fall back to any earlier state. That makes every outcome explainable after the fact. Stayed in S2D Defensive Resistance for years? No trigger came. Left right away? Trigger came. Heads I win, tails you lose.
- V5 is more honest than V4. That's not the same as being a better model. The core problem is unchanged: V5 describes observed behaviors and dresses them in mechanism-anchor language, but no mechanism actually rules out any behavior.

## Findings

### 1. Mechanism anchors are renaming, not explaining

V5 anchors S2D Defensive Resistance (the defensive-evaluation state) to "identity-protection cognition" and cites Kahan and Festinger. That's a label slapped on the behavior the model already described: weighing negative evidence heavier than positive. Naming the mechanism doesn't explain *why* the person does that, and it doesn't predict what they'll do next.

A mechanism would earn its keep if it ruled things out. For example: if "identity-protection cognition" predicted "S2D Defensive Resistance people will accept any evidence that protects their identity, even when it contradicts what they said yesterday," that would be a real prediction. You could test it. The model doesn't make that prediction. S2D Defensive Resistance is still just "asymmetric updating." The mechanism label is **decoration**.

Not a single anchor in V5 has a tested prediction attached. No section says "if S2D Defensive Resistance is identity-protection-driven, then we should see behavior X that we don't see in S2T Trust Evaluation." The anchors are **one-way labels**, not two-way constraints.

### 2. "Limits of operationalization" is V5 admitting the model was never falsifiable

The new section lists what can't be measured:

- S2T Trust Evaluation versus S2D Defensive Resistance — both look like a person testing AI, and the asymmetric updating that distinguishes them is "only visible across multiple evaluations."
- S3B Bargaining versus S7A Maturity — telling them apart needs a long-term observation across multiple model releases.
- The dual-component S5 Understanding — both the internal piece (mental reframing) and social piece (people around you treating AI as normal) are unobservable.

These aren't limits V5 discovered. V4 already claimed S2T Trust Evaluation and S2D Defensive Resistance were distinguishable states. V5 admits the only way to actually distinguish them is to watch someone over several model releases and judge whether their updating "looked asymmetric." That's not a measurement. That's a story you tell after the fact.

If the only way to tell two states apart is to watch outcomes and decide which definition fits, the states aren't separate claims about reality. They're **interpretive frames** — labels you apply after you already know what happened.

### 3. The two-piece S5 Understanding explains every outcome

S5 Understanding (the integrated, stable state) requires two things at once: internal reframing, and social normalization. Neither is measurable. The model itself says: "the dual-component requirement is currently conjecture. No instrument is specified for either component, and any observed discomfort can be attributed to mismatch."

This is the classic unfalsifiable move. Define a success state with two unmeasurable parts. Person stays stable? They had both. Person collapses? One of the pieces was missing. The model survives every outcome. Someone who reaches S5 Understanding and then quits AI doesn't refute the model — they're explained as "lacked social normalization."

### 4. The 2D dropout plane is empty

V4 had a simple split for people who quit AI. V5 replaces it with a 2D plane: Practical severity 0–10 and Emotional severity 0–10. But the model never says how to score someone's position on the plane, never shows data on where actual dropouts land, and never predicts which region of the plane leads to which outcome.

The "operational test": offer the person a better tool. If they restart, the problem was practical. If they don't, the problem was emotional. This is **circular**. The only evidence that the new tool is "better" is that *you* think it's better. If they refuse it, you conclude it must have been emotional — but maybe the tool just wasn't actually better for them. You haven't measured anything. You've assigned a label after the outcome.

### 5. Identity-protection cognition is everywhere, so it distinguishes nothing

The model anchors four different states to identity-protection-style mechanisms:

- S2D Defensive Resistance — "identity-protection cognition"
- S3 Ego Shock — "self-efficacy collapse"
- S3B Bargaining — "cognitive dissonance reduction"
- S7C Ethical Integration — "meaning-making"

Kahan's research shows motivated reasoning shows up almost everywhere humans care about something. So if it explains four states, it doesn't tell them apart. All four show identity-protective behavior. Why is the S2D Defensive Resistance person's defensive evaluation a *different state* from the S3 Ego Shock person's panic? The model's implicit answer is "intensity differs." But intensity isn't measured. It isn't predicted by the mechanism either. It comes from the two axes (Identity Stakes × Task Delegation), which are independent of the anchor. A mechanism that applies to four states isn't constraining the model. It's naming a **universal behavior** and calling it an explanation.

### 6. The "S7F Evangelism needs prior S3 Ego Shock" claim is flagged as a guess but used as a structural rule

The model says: stable AI evangelism (S7F Evangelism) is most stable when the person previously went through S3 Ego Shock (the panic state). The idea: you can't credibly help others through the rough part if you never had a rough part yourself. Without that history, the advocacy is naive ("S6A Enthusiastic Overuse flavor") or forced ("S6D Social Overuse flavor") and falls apart at the first hostile question.

Then the model immediately says: "the 'S3 Ego Shock prerequisite for stable S7F Evangelism' claim is currently conjecture."

If it's a guess, it shouldn't shape the structure of the model. If it's true, it should be a hard requirement. V5 has it both ways. A counterexample — a successful evangelist who never went through S3 Ego Shock — gets reclassified as "unstable S7F Evangelism" or "S6D Social Overuse flavor" rather than counting as a refutation.

### 7. The S3B Bargaining versus S7A Maturity test depends on which state you already assigned

The model offers a way to tell S3B Bargaining (defensive boundary deals with yourself about AI) from S7A Maturity (genuine bounded adoption based on testing): "In S3B Bargaining, boundaries are renegotiated under capability pressure. In S7A Maturity, boundaries move only after measured evidence."

Sounds good. But which state someone is in determines how you read the same behavior.

Take a person with bounded AI use. A new model comes out. They don't change their boundary.

- If you've already labeled them S3B Bargaining, you say: "they're awaiting the next pressure point that will shatter the boundary."
- If you've already labeled them S7A Maturity, you say: "they tested and the evidence wasn't compelling."

Same non-action, opposite interpretations, depending on the prior label. A distinction that needs the subject's self-report and long-term observation to apply isn't a property of the states. It's a **post-hoc story**.

### 8. Mechanism anchors don't constrain transitions

A real structural rule would say something like: "If someone is in S2D Defensive Resistance, they cannot go directly to S5 Understanding without passing through S3 Ego Shock."

The model doesn't make any such rule. From S2D Defensive Resistance, the person can go to S5 Understanding, S2T Trust Evaluation, S3 Ego Shock, or dropout. Knowing the mechanism anchor tells you nothing about which transition will happen. The anchor is a label for the current state, not a predictor of the next one.

### 9. "Regression is a property of every transition" makes the state structure untestable

The model now says: "Regression is a property of every transition, not a destination. Any state in S5 Understanding–S7 can be pushed back to earlier states by [list of triggers]."

If any state can fall back to any earlier state, the structure can't be tested. Person stayed in S2D Defensive Resistance for two years and then suddenly left? A trigger came at year two. Person jumped from S0 Baseline straight to S5 Understanding with no intermediate states? "Possible for low stakes with prior conceptual familiarity." Every observed path has an exit explanation. A model in which any path is allowed isn't wrong. It's **empty**.

### 10. V5 downgrades V4's falsifiability claims without rebuilding anything

V5 says: "Several V4 claims are downgraded from 'falsifiable' to 'heuristic' where the model lacks a workable measurement protocol."

This is presented as careful refinement. In practice it's an admission that V4's falsifiability claims were aspirational. The right response to "this claim isn't falsifiable" isn't "flag it as a heuristic and keep it." It's "remove it, or build a way to measure it."

The model still inherits V4's whole state structure. The new mechanism labels don't constrain anything. The newly-admitted measurement limits were always there. The new 2D dropout plane isn't measurable. None of these changes touch the underlying problem: the model has **no testable predictions**.

## Recommendations

1. **Run an empirical study before V6.** Pick two transitions (S1 Initial Encounter → S2T Trust Evaluation versus S1 Initial Encounter → S2D Defensive Resistance, and S2D Defensive Resistance → S3 Ego Shock versus S2D Defensive Resistance → S3B Bargaining) and gather behavioral data on the actual signals. Do S2T Trust Evaluation people show symmetric updating, and S2D Defensive Resistance people show asymmetric updating? Can you measure it? Can you predict which transition a given person takes? Run the study. Publish results. If the transitions are real, V6 can anchor to tested mechanisms. If not, V6 needs to restructure the states.

2. **Pick a lane: testable, or descriptive.** Either build testable predictions (by running recommendation 1) or admit the model is descriptive only — a thinking tool and shared vocabulary, not a causal model. Staying in the middle is the worst option. It's neither testable nor honestly framed.

3. **If you keep the model as-is, fix the anchor language.** Change "Mechanism anchor:" to "Related literature:" That signals the connection is conceptual, not explanatory. Stop claiming the mechanism constrains the model.

4. **Stop adding stuff before measuring what's already there.** V4 to V5 added mechanism anchors (unmeasured), a 2D dropout plane (unmeasured), and a Limits section (admitting unmeasurability). V5 to V6 should not add more states, more axes, or more mechanism labels. Test the existing skeleton or simplify it.
