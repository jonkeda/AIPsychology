# Slice 08 — Pre-emptive Ethical Rejection Path

Covers source item **20**: add a branch from S1 Initial Encounter for users who perform rapid ethical appraisal and decline without testing, distinct from post-engagement ethical reflection.

## What the source asks for

From [3-Answers-Model5.md](../../Questions/3-Answers-Model5.md) section A.4 and the original request in 3-Questions.md:

> Some users perform rapid ethical appraisal at Initial Encounter and move directly to Ethical Integration or non-adoption without testing. This is distinct from post-engagement Ethical Integration and represents ethical commitment prior to capability assessment.

## What to add

### New state: PEN — Pre-emptive Non-Adoption

> "I have thought about this. I don't need to try it to know it's not for me."

A stable non-adoption position reached at or shortly after S1 Initial Encounter, based on values-grounded ethical appraisal rather than on capability testing or identity threat.

This is distinct from:

- **S7E Ethical Integration** — which requires extended use followed by reflective stance. S7E users are AI users who think carefully about their use. PEN users never substantively use AI in the affected domain.
- **S2D Defensive Resistance** — which is identity-protection cognition. PEN is moral identity prioritization. The person is protecting their values, not their competence.
- **Emotional dropout** — which is a response to a negative experience. PEN happens before any significant engagement.
- **Practical dropout** — which is triggered by tool failure. PEN happens regardless of capability.

The three distinguishing signals (from 3-Answers section A.4):

1. **Cross-domain consistency.** The ethical objection applies across domains, not just the person's identity-threatened domain. It only becomes diagnostic in combination with the other two signals.
2. **Evidence response.** Demonstrating AI capability does not break the position — the better AI performs, the worse the ethical concern (more displacement, more bias at scale, more authentic fakes). In both PEN and S2D Defensive Resistance, capability evidence does not break the position, but the *reason* it does not break is different.
3. **Emotional register.** S2D Defensive Resistance has anxiety underneath — fear of obsolescence. PEN has moral conviction, sometimes grief, sometimes contempt. The threat appraisal is "this threatens something I care about" not "this threatens me."

None of these signals is reliable in a single observation. They are diagnostic only over time and in combination.

### State definition

```markdown
## PEN — Pre-emptive Non-Adoption

> "I have thought about this. I don't need to try it to know it's not for me."

The person has performed a rapid ethical appraisal at or shortly after S1 Initial Encounter and reached a stable conclusion to decline engagement. The conclusion is prior to capability assessment — the person is not declining because AI fails at the task, but because they have concluded that using it conflicts with their values.

**Mechanism:**

Conceptually related to **moral identity prioritization** — the tendency to act in line with one's core values when those values conflict with a course of action, independent of whether that course of action would produce good outcomes by other measures. Moral identity (the degree to which being a moral person is central to one's self-concept) is an established construct in social psychology.

**What makes PEN stable:**

The position is stable when the ethical objection is grounded in a value that is unlikely to shift under capability pressure. "I believe in the economic value of human creative work" or "I believe AI training data practices are exploitative" are positions that hold regardless of whether AI improves. They are not positions about AI's current capabilities.

**Entry condition from S1:**

Pre-emptive non-adoption is most likely when:

- The person has prior ethical frameworks applied to technology (privacy advocacy, open-source ethics, labor rights).
- The ethical concern is specific and addressable in principle (if the concern were resolved, would they reconsider?). This is the key diagnostic test — if resolving the concern would not change the position, the stated reason is a proxy for a deeper value.
- The encounter happens in a low-personal-stakes context — the person is not defending their own livelihood, they are acting on values.

**Transitions:**

- → **S5 Understanding** or **S7E Ethical Integration**: possible if the stated ethical concern is substantively addressed and the person genuinely re-evaluates. Rare, but the model should not treat PEN as permanent.
- → **Stable non-adoption**: the most common outcome. The person does not progress further in the model for this domain.
- → **S2D Defensive Resistance**: possible if closer engagement reveals identity stakes the person had not initially recognized. The ethical frame was covering a competence-threat dynamic.

**⚡ External triggers:**

No strong ⚡ marker. The position is internally grounded. Regulatory changes (AI banned in a domain, copyright law outcomes) can validate the position externally but typically do not create it.
```

### Diagnostic difficulty — explicitly note it

In the `PEN` state file and in `Model6.md`:

```markdown
## Diagnostic difficulty: PEN versus S2D Defensive Resistance with ethical language

From outside, pre-emptive non-adoption and S2D Defensive Resistance dressed in ethical language look almost identical. Both decline to engage, both cite principled reasons, both discount capability evidence. The distinction only becomes visible over time:

- Does the objection apply consistently across domains where identity is not at stake?
- Does the objection hold if the stated concern is demonstrably addressed?
- What is the emotional register — anxiety or moral conviction?

Most real cases are mixed. The model does not require a clean classification. A person can be simultaneously in S2D Defensive Resistance (protecting competence) and making genuine ethical arguments (that are also true and genuinely held). Labeling a mixed case as "pure PEN" would be wrong; so would labeling it "pure S2D." Use the frame to understand the mixture, not to classify it.
```

## State graph update

Add to the mermaid diagram:

```
S1 -->|ethical pre-commitment| PEN
PEN -->|ethical concern resolved| S5
PEN --> StableNonAdoption
PEN -->|competence threat surfaces| S2D
```

The `StableNonAdoption` endpoint can be treated as a named dropout variant or just labeled as a dropout. It is different from emotional or practical dropout in that it is not a negative experience — it is a conclusion.

## File to create

`states/PEN-pre-emptive-non-adoption.md` using the standard template from slice 01.

## Addition to populations.md

Short note in `populations.md`:

```markdown
## Pre-emptive Non-Adoption

Not all non-adoption is dropout. A subset of people reach a stable non-adoption position at first encounter, based on an ethical or values-grounded appraisal. This is not S2D Defensive Resistance (which is competence-protection), not emotional dropout (which requires a negative experience), and not S7E Ethical Integration (which requires prior use).

See `states/PEN-pre-emptive-non-adoption.md` for the full description. The key practical note: before treating someone as S2D Defensive Resistance because they won't engage, check whether their position is cross-domain consistent and values-rooted rather than identity-defensive. If it is, the model's S2D toolkit (reduced identity threat, low-stakes entry) will not work. Engaging with the ethical substance is the right approach.
```

## Verification checklist

- [ ] `states/PEN-pre-emptive-non-adoption.md` exists.
- [ ] S1 Initial Encounter file has the PEN exit edge.
- [ ] Mermaid diagram includes PEN.
- [ ] Diagnostic difficulty section clearly states the S2D vs PEN ambiguity.
- [ ] `populations.md` has the short PEN note.
- [ ] PEN transitions back to S5 or S7E Ethical Integration are included (PEN is not a dead end).
