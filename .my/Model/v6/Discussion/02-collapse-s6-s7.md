# Discussion 02 — Collapsing S6 and S7

Working notes. Builds on the proposal in [012p-one-shot-plain.md](../Reviews/012p-one-shot-plain.md). The aim is to walk through what the collapse actually changes in V6, what it costs, and where it leaves the model's vocabulary.

## What the proposal is

Replace the eight states S6E, S6D, S6R, S6S, S7M, S7I, S7E with **two states plus driver attributes**:

- **S6 Overuse** — one state. Carries one or more drivers: Reward-Driven, Anxiety-Driven, Efficiency-Driven, Social-Driven.
- **S7 Integration** — one state. Carries one or more calibration styles: Mastery-Focused, Identity-Expanding, Ethically-Integrated.

Keep **S7B Burnout** and **S7V Evangelism** as their own states.

State count goes from 18 to 14 (12 if S2P is also collapsed; see [Discussion 01](01-categorization.md)).

## Why the collapse fits V6 specifically

Three V6 features make this proposal an obvious move rather than a controversial one:

1. **The observation guide already concedes it.** *"Volume alone does not distinguish. All four S6 states can produce similar usage volume. The driver is what differs."* That is the definition of a property, not a state.
2. **The S7 coexistence rule already concedes it.** The state graph says any S7 state can coexist with any other S7 state, with no transitions between them. States that coexist indefinitely without transitions are dimensions, not states.
3. **V6 already uses driver/property machinery.** Identity Stakes and Delegation Ceiling are not states; they are per-person properties that modulate states. Adding "S6 driver" and "S7 calibration style" as similar properties matches the existing pattern, not an exotic addition.

## What is gained

- **Eight false distinctions disappear.** A practitioner watching someone in front of them is no longer asked to distinguish S6E from S6R from S6S in real time. They are asked to identify drivers, which is a separate diagnostic task that the observation guide already describes.
- **The state graph simplifies.** Many of the cross-S7 coexistence rules in `02-state-graph.md` become statements about a single S7 state with multiple attributes. That is one paragraph instead of a section.
- **Healthiness becomes more honest.** The current healthiness file says S6E is "healthy short-term, costly long-term." That is a description of a *driver pattern*, not a state. Treating it as a driver makes the framing explicit.

## What is at risk

- **Loss of vocabulary.** "S6E Enthusiastic Overuse" is a memorable label that points at a recognisable type. "S6 Overuse, Reward-Driven" is more accurate but less catchy. Practitioners may keep the old labels informally.
- **Coexistence becomes the default.** Once drivers are attributes, a person in S6 routinely carries two or three drivers. This is realistic but adds analysis surface — every observation carries a driver-signature, not a single driver.
- **V5/V6 → V7 churn.** Anyone who has internalised the S6E/S6D/S6R/S6S distinction will have to re-learn it. The reviews and answers in this version reference the four-state form throughout.

The first risk is real but small — labels can be aliased ("S6 Reward-Driven" can be referred to as "S6E" informally). The second is the substantive cost: the collapse trades simpler state count for richer per-state attributes.

## What stays unchanged

- **Drivers themselves.** Reward-Driven, Anxiety-Driven, Efficiency-Driven, Social-Driven are exactly the four current S6 substates. Nothing about the underlying psychology changes.
- **S7M/S7I/S7E content.** Each one's description, observation markers, and mechanism anchors stay. They become attributes attached to a single S7 state instead of three separate state files.
- **Transitions in and out.** S5 → S6, S6 → S7B, S6 → S7, S7 → S3E, S7 → S7B, S7 → Dropout — all unchanged at the state level.
- **S7B and S7V.** Burnout and Evangelism are genuinely different shapes. S7B is a recovery position with distinct behavioural markers. S7V is an externally-directed posture that can co-occur with any of the integration styles. Both stay.

## What the collapsed graph looks like

```
S5 Understanding
  ├─→ S6 Overuse  [drivers: reward / anxiety / efficiency / social]
  │     ├─→ S7 Integration
  │     ├─→ S7B Burnout
  │     └─→ Dropout
  └─→ S7 Integration  [styles: mastery / identity-expansion / ethical]
        ├─→ S3E (regression)
        ├─→ S7B Burnout
        ├─→ S7V Evangelism (overlay)
        └─→ Dropout
```

S7V is shown as an overlay because it can be present with any S7 calibration style — the current model already says this.

## What S6/S7 do not collapse to

This proposal does not say:
- "S6 and S7 are the same thing." They are different — S6 is high-volume use without sustainable calibration; S7 is calibrated use whether high-volume or not. The distinction is real and stays.
- "Drivers are not states." A driver and a state are different objects. A state is a posture toward AI. A driver is what is sustaining that posture. The proposal removes the four S6 *states* and keeps the four *drivers* as a separate axis.
- "Multiple S7 styles are interchangeable." The three styles are recognisable and worth naming. They just are not separate states.

## Open question — does S7B move too?

The 012 proposal keeps S7B Burnout as its own state. That is defensible — burnout has distinct observable markers (withdrawal, affective collapse, productivity drop) and a distinct entry condition (cost outran value). It is not a calibration style; it is a state in the strong sense.

The same argument applies, weakly, to S6: someone in S6-burnout-trajectory looks different from someone in S6-stable-overuse. But the model already handles this with the S6 → S7B transition rather than as a separate S6 substate, so no change needed there.

## Recommendation

The collapse is a clear V7 candidate. The only V6-era question worth deciding now is **whether to start using the driver/style vocabulary informally** in the V6 documents — for example, in the observation guide where it would clarify what a practitioner is actually looking for. Adding driver labels alongside the current state labels is cheap and prepares the ground.

Wholesale renaming should wait for V7 to avoid mid-version churn.
