# Discussion 03 — Stages, States, and the Question of "Better"

Working notes. The aim is to surface a tension the modeller has noticed but not fully named: V6 calls these *states* but treats them, much of the time, like *stages* — and there is a separate, related tension between *describing* what people do and *recommending* what they should do.

## Stages or states?

The model uses the word **state**. Most descriptions assume the word **stage**. The two are different:

| | Stages | States |
|---|---|---|
| **Direction** | Move through them in roughly one direction | Can be entered, left, re-entered |
| **Sequence** | Earlier ones precede later ones | No required order |
| **Regression** | Unusual, often pathologised | Routine; described and named |
| **Examples** | Piaget's developmental stages, Kübler-Ross | Mood states, attachment states, system states |

V6 has features of both:

**Looks like stages:**
- Numbering implies order (S0 → S1 → S2 → S3 → S5 → S6/S7).
- The arc is mostly forward.
- Going back to S0 is described as effectively impossible.
- S7M is implicitly more *integrated* than S5, which is more integrated than S3B, and so on.

**Looks like states:**
- Regression edges exist (S7 → S3E on capability shock).
- Dropout is reachable from every state.
- S2T → S2D is an asymmetric regression-like edge.
- A person can revisit S3B repeatedly across model releases.

The honest answer is that V6 is **stages with state-shaped escape valves**. The forward path is the dominant assumption. The state machinery is added because the forward path turns out not to be irreversible.

This matters because the two framings recommend different things. A stage model implies a target (the late stages). A state model implies no target (just current location). V6 oscillates between the two without saying which it is doing.

## Will people ever go back to S0?

Probably not, in practice, and the model is right to say so. S0 means "no engagement, no stance". Once a person has had S1 and reacted to it, they have a stance. Even withdrawal is a stance (S2D, S2P, dropout). Returning to "no stance" requires forgetting, not changing.

The exception: long-term dropout in someone who never built a strong reaction may functionally resemble S0 again after enough years. This is rare and worth a one-line note rather than a transition edge.

## The S8 question — should Burnout and Structural Displacement be a separate family?

The modeller's instinct: S7B Burnout and S3X Structural Displacement feel like *terminal* positions in a way the other states do not. They share several properties:

- They are reached *after* significant engagement, not at the start.
- Time scales are long. Months to permanent.
- They sit outside the integration cycle. A person in S7B is not actively integrating; a person in S3X is not actively bargaining.
- Resolution from them is structural (recovery, transition, exit), not psychological calibration.
- They share an end-state quality with each other that they do not share with the S7 integration positions.

Arguments for promoting them to **S8**:

- It honestly reflects their role as terminal/recovery positions.
- It removes S7B from the "S7 integration" family where it does not fit (S7B is the failure of integration, not a style of it).
- It places S3X with S7B, which matches their shared post-engagement, structural-resolution character.

Arguments against:

- S7B is reachable from many places. Calling it S8B is a renumbering that does not add diagnostic clarity.
- S3X is already documented in S3 because it shares "this is being disrupted" connotation with S3E and S3B. Moving it costs cross-references.
- Adding a new prefix family for two states is heavyweight.

If the model also adopts the S6/S7 collapse from [Discussion 02](02-collapse-s6-s7.md), then S7B will already be the only "burnout" state in the model. Promoting it to S8B at the same time is cheap. S3X moving to S8X is also cheap if done in the same version.

**Provisional recommendation for V7:** if the S6/S7 collapse happens, also promote S7B → S8B and S3X → S8X. The new S8 family means: *terminal positions reached after significant engagement, resolved through structural rather than psychological means*. It is a small renumbering with real diagnostic content.

## Better and worse states

The modeller has admitted it: S7M *feels* better than S6D, S2D *feels* unhealthy, S7B *feels* like something to leave. The healthiness file already encodes this:

- *Sustainable* states (S7M, S7I, S7E, S5, S3B for many, S2P, S0 permanent).
- *Sustainable with cost* states (S6E, S6R, S6S, S7V).
- *Transitional only* states (S3E, S2T, S2D, S1).
- *Recovery* (S7B).
- *Sustainable but corrosive* (S6D, sustained S2D).
- *Legitimate, not pathological* (S3X).

This is a ranking dressed in non-judgemental language. The model says "we don't use the word healthy inside state descriptions" then provides a hierarchy that is unmistakably a ranking of better and worse.

That is **not necessarily wrong**. But the model needs to decide what it is.

Three options, in order of honesty:

1. **Pure description.** No ranking, no health levels, no "sustainable but corrosive". States are described, not graded. The user reads them and decides what to do. The healthiness file disappears or becomes a separate non-model document.
2. **Description plus declared ranking.** Keep the descriptions value-neutral, but include a separate, clearly-flagged section that says: "The author considers some states healthier than others. Here is the ranking and the reasoning. This is editorial, not part of the model." Readers can use or ignore it.
3. **Prescriptive model.** The model openly says: S7M is the goal, S6D is bad, S7B should be exited. Practitioners are told to move people toward the better states. This is what the healthiness file currently does in everything but name.

V6 is doing option 3 while claiming option 1, with option 2 framing in the healthiness file's opening sentence. This is incoherent.

The modeller's stated intent is descriptive. If that is real, option 1 or 2 should be picked deliberately. If the actual aim is to help people end up in S7M and avoid S6D, option 3 should be claimed openly.

## What kind of model is this, then?

The honest answer combines several roles, and they interfere with each other:

- **Vocabulary.** Names for recognisable patterns. Genuinely useful.
- **Map of where someone is right now.** Diagnostic. Practitioner-relevant.
- **Implied trajectory.** The numbering and the arc say there is a forward direction.
- **Implicit ranking.** Some states are presented as healthier than others.

The vocabulary and the map are uncontroversial. The trajectory and the ranking are doing prescriptive work without admitting it.

## Recommendation

Pick a position and write it into Model6.md before the state descriptions, not after. Three sentences would do it:

> *This model is descriptive: it names states, describes how people enter and leave them, and says nothing about which states a person should be in. Some states are easier to sustain than others, and that information is recorded in [healthiness.md](healthiness.md) as the author's interpretation, not as a claim about right outcomes. Practitioners using this model should choose for themselves whether they are using it to understand a person's current position or to push them toward a different one.*

Or some version of that. The point is to make the descriptive-versus-prescriptive choice an explicit decision rather than a tension that runs under the surface of every state description.

## Recommendation summary

| Question | Recommendation |
|---|---|
| Stage or state? | Acknowledge V6 is stages with state-shaped escape valves; do not pretend either framing is pure. |
| Will people return to S0? | Effectively no. Document and move on. |
| S8 family? | Worth doing in V7 alongside the S6/S7 collapse — promote S7B → S8B and S3X → S8X as terminal positions. |
| Descriptive or prescriptive? | Pick one and state it in Model6.md. The current oscillation is the underlying problem behind several reviewer critiques. |
