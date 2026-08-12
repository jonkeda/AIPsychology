# Identifiers

The identifier scheme is the change that motivated V7. This document explains why the numbering failed, what replaces it, and how to translate V6 material.

## Why the numbers had to go

V6 used identifiers of the form `S0`, `S1`, `S2T`, `S3E`, `S5`, `S6D`, `S7M`. A single token was being asked to carry three separate jobs:

1. **Identity** — a unique handle for one position.
2. **Order** — the numeric part implied that lower comes before higher.
3. **Family** — the numeric prefix implied that everything sharing a number shares a structural property.

Job 1 worked. Jobs 2 and 3 failed, and they failed in ways that could not be fixed by renumbering.

### The order the model does not have

V6 stated plainly that the labels were identifiers rather than ordinals, that regression was routine, and that no position was a target. Readers ignored all of this, because `S7M` after `S6D` after `S5` is a ladder and no disclaimer survives contact with a ladder. Every reviewer who engaged with the model at length re-imported the developmental reading somewhere.

The problem is structural. A model whose central claim is *there is no required order* cannot use ordinal identifiers. The notation contradicts the thesis.

### The families that were not families

The prefix promised shared structure. It delivered it in two places and not in the rest:

| Prefix | Promise | Reality |
| --- | --- | --- |
| `S2` | Stance formation after first contact | Held. Genuinely a fork. |
| `S3` | Identity disruption | Half held. `S3E` and `S3B` are siblings; `S3X` is a terminal economic recognition that belongs elsewhere. |
| `S6` | High-volume use | Four separate identifiers for one pattern with four motives. |
| `S7` | Long residence | Five identifiers with nothing in common except "after `S5`". Three are coexisting styles, one is a withdrawal, one is an outward-facing behaviour. |

### The gap and the churn

`S4` never existed. The numbering jumped from `S3` to `S5` as an artifact of an early draft and stayed that way through two versions because closing it meant renumbering everything downstream.

The V7 proposal that preceded this design set illustrates the trap. It closed the gap by shifting `S5 → S4`, `S6 → S5`, `S7 → S6`, and promoting the terminal positions to `S7`. The result is a scheme in which `S5` means Understanding in V6 and Overuse in V7, and `S7` means Integration in V6 and Burnout in V7. Every review document, every practitioner note, and every conversation held under V6 becomes actively misleading rather than merely outdated. A renumbering that silently changes what a token means is worse than the gap it closes.

Numbers will keep producing this problem. Any future addition to the middle of the graph forces the same choice between a gap and a churn.

## The V7 scheme

**Positions are identified by two-letter mnemonic codes. There are no numbers.**

Each code is the initials of the position's name. Codes carry no order, no rank, and no arithmetic. A new position can be added at any time without disturbing any existing one.

Positions are grouped into five **families**. Families are named with words rather than letters or numbers, so that the grouping conveys meaning without smuggling in sequence. The family is descriptive metadata, not part of the identifier.

### The positions

| Code | Name | Family | One-line description |
| --- | --- | --- | --- |
| **NE** | No Engagement | Pre-engagement | Has not meaningfully used AI in this domain |
| **FC** | First Contact | Pre-engagement | The first substantive encounter and the reaction to it |
| **OE** | Open Evaluation | Stance | Testing the tool without a stake in the answer |
| **GE** | Guarded Evaluation | Stance | Testing the tool while defending a position |
| **VR** | Values Refusal | Stance | Declining on grounds that precede the tool's performance |
| **IS** | Identity Shock | Disruption | Acute destabilisation when the skill is convincingly replicated |
| **SB** | Scope Boundary | Disruption | A stable negotiated line: AI here, not there |
| **CU** | Calibrated Use | Working | Accurate judgement about where the tool helps |
| **OU** | Overuse | Working | Use volume beyond what judgement supports |
| **OL** | Oversight Load | Working | Work has become checking output rather than producing it |
| **IP** | Integrated Practice | Working | AI is part of how the work is done and how the person understands the work |
| **BO** | Burnout | Exit | Withdrawal after cost exceeded value |
| **SD** | Structural Displacement | Exit | Recognition that no viable position remains in the domain |
| **DX** | Disengagement | Exit | Stopped using the tool, for practical or emotional reasons |

Fourteen positions, one of which (`OL` Oversight Load) is new and provisional. V6 had eighteen.

### The overlay

| Code | Name | Attaches to | Description |
| --- | --- | --- | --- |
| **AV** | Advocacy | `IP` Integrated Practice, sometimes `OU` Overuse | Publicly promoting AI adoption to peers, the organisation, or a field |

`AV` Advocacy is not a position. It is a behaviour that runs on top of one. A person is never *in* `AV` Advocacy; they are in `IP` Integrated Practice *with* `AV` Advocacy active. V6 treated the equivalent (`S7V`) as a state, which produced the awkward result that a person could apparently leave Integration by starting to talk about it in public.

## Writing conventions

- **Codes are uppercase, two letters, no punctuation:** `CU` Calibrated Use, `GE` Guarded Evaluation, `SD` Structural Displacement.
- **The code is always paired with its full name, on every appearance:** the code in backticks, then the plain-text name — `GE` Guarded Evaluation. A bare code is never written on its own.
- **Always pair code with domain on first use in a discussion:** `GE` Guarded Evaluation (technical writing). A code without a domain is incomplete, because a position without a domain is not a claim the model makes.
- **Attributes follow the name in lowercase after a colon:** `OU` Overuse: anxiety, chronic. Multiple attributes are comma-separated in order of dominance.
- **The overlay follows with a plus:** `IP` Integrated Practice + `AV` Advocacy (public).
- **In prose the code leads and the name follows** — "`GE` Guarded Evaluation" — and the pairing is repeated on every mention, not just the first.

A full position statement therefore reads:

> `GE` Guarded Evaluation (illustration): entrenched — and — `CU` Calibrated Use (client email) — and — `IP` Integrated Practice + `AV` Advocacy (research synthesis): mastery, ethical

That is one person, three domains, on one day.

## Attributes replace states

Where V6 used a separate identifier to record a motive or a style, V7 uses one position with an attribute. The behaviour being described is identical; the number of things to memorise drops.

**`OU` Overuse carries a driver.** Multiple drivers are common and are listed in order of dominance.

| Driver | What sustains the use | V6 equivalent |
| --- | --- | --- |
| `reward` | Intermittent good outputs sustain use regardless of failure rate | `S6E` Enthusiastic |
| `anxiety` | Self-trust has transferred to the tool; the person doubts their own judgement without it | `S6D` Dependent |
| `efficiency` | Throughput targets or external pressure override quality judgement | `S6R` Driven |
| `social` | Peer adoption, team norms, or visibility pressure drive use | `S6S` Social |
| `mandate` | Use is a condition of the role, tracked and enforced | **New in V7 —** see [07-environment-shift.md](07-environment-shift.md) |

**`IP` Integrated Practice carries a style.** Any combination; all three at once is common.

| Style | What it means | V6 equivalent |
| --- | --- | --- |
| `mastery` | The line between use and non-use is drawn on competence grounds and moves on evidence | `S7M` Maturity |
| `expanded` | The self-concept has grown to include what the person can now do with the tool | `S7I` Identity Expansion |
| `ethical` | Attribution, consent, and disclosure are built into the work rather than added afterwards | `S7E` Ethical Integration |

Full attribute lists for every position appear in [05-states-early.md](05-states-early.md) and [06-states-working.md](06-states-working.md).

## Translation from V6

The table below is exact. Every V6 identifier maps to exactly one V7 identifier plus, where applicable, an attribute.

| V6 | V7 | Notes |
| --- | --- | --- |
| `S0` Baseline | `NE` No Engagement | The pre-encounter / permanent-non-user split becomes the `horizon` attribute |
| `S1` Initial Encounter | `FC` First Contact | Gains `trigger` and `prior-knowledge` attributes |
| `S2T` Trust Evaluation | `OE` Open Evaluation | Renamed to avoid implying that trust is the object of evaluation |
| `S2D` Defensive Resistance | `GE` Guarded Evaluation | Renamed. "Resistance" was evaluative and framed the person as an obstacle |
| `S2P` Pre-emptive Non-Adoption | `VR` Values Refusal | Renamed for plainness |
| `S3E` Ego Shock | `IS` Identity Shock | Renamed. "Ego" carries psychoanalytic freight the model does not intend |
| `S3B` Bargaining | `SB` Scope Boundary | Renamed. "Bargaining" imported a Kübler-Ross association the model explicitly rejects |
| `S3X` Structural Displacement | `SD` Structural Displacement | Moved from the Disruption family to Exit |
| `S5` Understanding | `CU` Calibrated Use | Renamed. "Understanding" implied a comprehension achievement rather than a working equilibrium |
| `S6E` Enthusiastic Overuse | `OU` Overuse: reward | |
| `S6D` Dependent Overuse | `OU` Overuse: anxiety | |
| `S6R` Driven Overuse | `OU` Overuse: efficiency | |
| `S6S` Social Overuse | `OU` Overuse: social | |
| `S7M` Maturity | `IP` Integrated Practice: mastery | |
| `S7I` Identity Expansion | `IP` Integrated Practice: expanded | |
| `S7E` Ethical Integration | `IP` Integrated Practice: ethical | |
| `S7V` Evangelism | `IP` Integrated Practice + `AV` Advocacy | Demoted from state to overlay |
| `S7B` Burnout | `BO` Burnout | Moved from the Integration family to Exit |
| Dropout | `DX` Disengagement | Promoted from a cross-cutting concept to a named position |
| — | `OL` Oversight Load | **New in V7 —** no V6 equivalent |

### Renames are deliberate, not cosmetic

Six positions were renamed rather than merely re-coded. In each case the V6 name was doing evaluative or theoretical work the model does not want:

- **Defensive Resistance → Guarded Evaluation.** "Resistance" is what a change programme calls someone who disagrees with it. The position describes a person evaluating a genuine threat carefully. The new name describes the behaviour without taking the organisation's side.
- **Ego Shock → Identity Shock.** "Ego" invokes a psychoanalytic apparatus the model does not use and cannot support.
- **Bargaining → Scope Boundary.** "Bargaining" is the third Kübler-Ross stage. The model spends effort denying that it is a grief model and then borrowed grief vocabulary for a position that is frequently stable and functional for years.
- **Understanding → Calibrated Use.** "Understanding" sounds like an achievement of comprehension, which invited the reading that everything before it was misunderstanding.
- **Pre-emptive Non-Adoption → Values Refusal.** Defined by what it is, not by what it is not.
- **Evangelism → Advocacy.** "Evangelism" is industry slang with a religious edge that colours the description of anyone it is applied to.

### Deprecated tokens

The tokens `S0`–`S7` and all suffixed variants are **retired**. They are not reused with new meanings. Any document using them is V6 or earlier, and the table above translates it unambiguously. This is the property the numeric proposal could not offer.
