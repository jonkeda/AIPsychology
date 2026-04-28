# Discussion 01 — Is the State Categorization Correct?

Working notes. Not part of the model. The aim is to surface assumptions baked into the V6 numbering scheme and decide which of them are actually load-bearing.

## What the V6 categorization currently is

V6 has eighteen states organised under seven prefix families:

| Prefix | What the prefix groups | States |
|---|---|---|
| **S0** | No engagement | S0 Baseline |
| **S1** | First substantive exposure | S1 Initial Encounter |
| **S2** | Stance-formation responses to S1 | S2T Trust Evaluation, S2D Defensive Resistance, S2P Pre-emptive Non-Adoption |
| **S3** | Identity-level disruption | S3E Ego Shock, S3B Bargaining, S3X Structural Displacement |
| (no S4) | — | — |
| **S5** | Stable functional integration | S5 Understanding |
| **S6** | High-volume use | S6E Enthusiastic, S6D Dependent, S6R Driven, S6S Social |
| **S7** | Long-residence end positions | S7M Maturity, S7I Identity Expansion, S7E Ethical Integration, S7B Burnout, S7V Evangelism |

The implicit logic: low numbers are early, high numbers are late, and the prefix groups things that share a structural position in the arc.

## Where the categorization is doing real work

Three places where the family grouping is genuinely informative and not just numbering:

1. **S2 as the fork after S1.** All three S2 states are entered from S1, and all three are stance-formation rather than action. The family captures something real: this is the moment at which a person commits to a posture toward AI.
2. **S3 as identity disruption.** S3E and S3B share a mechanism — the person's professional identity is destabilised by encountering a machine that does the thing the identity was built around. The family encodes that.
3. **S7 as long-residence positions.** Whatever else is true of S7M, S7I, S7E, S7B, S7V, they are positions someone can occupy for years, unlike S1 or S3E which are transitional.

## Where the categorization is doing thin or contradictory work

### S0 — splittable

S0 is currently one state with two readings: pre-encounter (transitional) and permanent non-user (terminal). The model handles this in prose ("Two readings"), but those are arguably two different things:

- A pre-encounter person has not yet had S1. Their next move is forward.
- A permanent non-user has decided, implicitly or explicitly, that S1 is not coming. Their position is stable.

**Open question:** is the pre-encounter / permanent-non-user distinction a state distinction, a property, or a phase? Three options:

- **Two states** (S0a Pre-encounter, S0b Permanent Non-User). Clean but adds a state for what is essentially a temporal property.
- **One state with a "permanence" property.** A person in S0 has a property that is "open" or "closed". Closed = permanent non-user. This matches the *Identity Stakes* / *Delegation Ceiling* pattern (per-person properties on top of states).
- **Status quo** — one state, two readings in prose. Workable but readers will keep asking.

The property option seems strongest. Permanent non-use is not a different *behaviour* — it's S0 with no exit edge.

### S2 — are S2T and S2D really different states?

Both S2T and S2D are entered from S1. Both involve testing AI behaviour. The differences:

- **Affect:** S2T is open evaluation, S2D is defensive evaluation under perceived identity threat.
- **Updating rule:** S2T updates symmetrically on positive and negative evidence. S2D updates asymmetrically — negative evidence sticks, positive evidence is discounted.
- **Modulator:** Identity Stakes drives the fork.

Asymmetric updating is observable only across multiple evaluations (the observation guide already says so). On a single observation S2T and S2D look identical. So the question is: are they two states distinguished by an axis property, or one state with a "stance-toward-evidence" property?

**Argument for keeping them separate:** the trajectories diverge. An S2T person can transition to S5 cleanly. An S2D person typically cannot — they have to pass through S3E or S3B first. The downstream behaviour is different even if the moment-to-moment behaviour is not.

**Argument for collapsing:** the fork is driven entirely by Identity Stakes, which the model already treats as an axis. Saying "high-stakes S2 evaluation" and "low-stakes S2 evaluation" would be more honest than naming them different states.

Status quo is defensible but not obviously correct. The same critique applies to S2P versus S2D (acknowledged in the observation guide and S2D file already).

### S3 — different levels stacked together

S3 currently contains three states that are not really at the same level:

- **S3E Ego Shock** is acute. Hours to weeks. Someone is in the middle of the disruption.
- **S3B Bargaining** is sustained. Months to years. Someone has built a stable scope-management posture.
- **S3X Structural Displacement** is structural. It is a recognition, not a phase. It is reached by realising something about the labour market, not by working through identity material.

S3X especially does not belong with S3E and S3B. It is closer to a long-residence position (an S7-flavoured terminus) than to an identity-disruption phase. A person in S3X is not disrupted in the same way an S3E person is — they have moved to a structural framing of the problem.

**Three options:**

1. Promote S3X to S8 (alongside S7B Burnout) as a long-residence position outside the integration cycle. Discussed in [Discussion 03](03-stages-states-and-judgement.md).
2. Leave S3X under S3 because it shares "this is being disrupted" connotation, even though structurally it is different.
3. Move S3X to its own prefix entirely (a true terminal-state family).

S3E and S3B are coherent as siblings: S3E is acute, S3B is the chronic version of the same tension. That part of S3 is fine.

### S4 — the missing number

S4 does not exist anywhere in V6 or V5. The numbering jumps from S3 to S5. This is presumably an artifact of an earlier draft that has not been documented.

**Options:**

- Renumber S5 → S4 in V7 to close the gap.
- Reserve S4 for a state that has not been written yet (a candidate: a transitional state between S3-disruption and S5-stable-integration, sometimes implicit in the model but not named).
- Document the gap in `00-relationship-to-prior.md` and leave it.

Renumbering is mechanically expensive and breaks every link from V5 reviews. Reserving S4 is honest. Documenting and leaving is cheapest. Recommendation: document the gap.

## The prefix system as a whole

The prefix-as-family system makes promises it does not always keep:

- **Promise:** prefix indicates structural position in the arc.
- **Reality:** S3X is a terminus not a disruption phase; S6 prefixes group four states that should arguably be one (see [Discussion 02](02-collapse-s6-s7.md)); S7 prefixes group five states with no shared structural property other than "long residence".

The S2 family is the cleanest. The S6 family is the loosest. The S7 family is internally heterogeneous: S7M/S7I/S7E are coexisting end positions, S7B is a recovery state, S7V is an externally-directed posture. They share a number because they are all "after S5" but that is not a structural property in the same way "fork after S1" is.

## Recommendations for V7 consideration

| Change | Cost | Benefit |
|---|---|---|
| Make S0 permanence a property, not two readings | Low | Removes a recurring confusion |
| Document S2T vs S2D as one state with stakes property — or commit to keeping them separate and explicitly say why | Low–Medium | Closes the per-domain-stakes circular-prediction critique already accepted in 004a |
| Move S3X out of S3 into a terminal-state family (S8 or its own prefix) | Medium | Reflects what S3X actually is |
| Document the missing S4 in 00-relationship-to-prior | Trivial | Stops readers wondering |
| Address S6 and S7 collapse separately | High | See [Discussion 02](02-collapse-s6-s7.md) |
