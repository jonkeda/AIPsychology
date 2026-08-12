# Plan — Transition Guidance

A work plan for a document set that does not exist yet. This file specifies **what needs to be written and to what standard**, not the guidance itself.

## Why this is being written

The model currently describes positions and names the edges between them. It says nothing about how anyone moves along an edge, what helps, what backfires, how long it reasonably takes, or how to tell "needs more time" from "this is not going to happen."

That gap is where most practical questions land. A manager who understands that someone is guarded about their core domain immediately asks what to do about it. An individual who recognises they are approaching burnout wants to know what happens next and whether it passes. Neither question is currently answered.

Three things make this worth writing now:

**There is at least one recorded case of the model helping, and it helped through transition information rather than through description.** The useful content was not the label — it was knowing the position was a phase, that it had a known exit, and that a break was the exit. That is transition guidance, and it is the only part of the model with any observed effect.

**The organisational use case requires it.** [09-adoption-programme.md](09-adoption-programme.md) tells organisations to change conditions rather than target positions, and then does not say which conditions change what. The advice is currently incomplete in the place where it matters.

**The stance question has been resolved in a way that permits it.** Prior versions oscillated between describing and recommending. The resolution below makes recommendation possible without abandoning the descriptive core.

## The stance the set must take

**Settle this before writing a word.** Every document in the set depends on it, and the previous versions' failure to settle it is the source of most reviewer objections.

> **Descriptive about persons. Prescriptive about conditions. Openly normative for a stated purpose, with the purpose named.**

Three parts, each doing specific work:

**Descriptive about persons.** No position is a failure or a deficiency. A person in guarded evaluation is evaluating, and may be right. The guidance never characterises a person as needing to change.

**Prescriptive about conditions.** Conditions are what the organisation controls and where the levers are. Guidance about conditions can be direct and specific without implying anything about the people in them.

**Openly normative for a stated purpose.** This is the change. Where an organisation has a legitimate business need — software development that works effectively with AI capability — some positions serve that need and others do not. The guidance may say so, provided it names the purpose it is serving.

The formulation to use, and to repeat wherever a preference appears:

> For an organisation that needs AI-collaborative development, calibrated use and integrated practice serve that need. Burnout and sustained anxiety-driven overuse do not. This is a business judgement relative to a stated purpose. It is not a claim about which positions are better for a person to occupy.

**One exception that must be preserved.** Structural displacement is not in the same category as burnout. Where a domain genuinely has no viable future, recognising that is an accurate reading rather than a failure to adapt. The guidance must not treat it as a state to be moved out of.

## Prerequisites

The set should not be written until these are done, because each would force a rewrite.

| Prerequisite | Source | Why it blocks |
| --- | --- | --- |
| Prior-art reconciliation | [../UseCases/03-prior-art.md](../UseCases/03-prior-art.md) | Transition advice for oversight load and calibrated trust exists in the automation literature. Writing it from scratch would duplicate better-supported work |
| The component cut | [../UseCases/02-component-audit.md](../UseCases/02-component-audit.md) | Transitions involving cut components must not be written |
| Position set frozen | [../Design/10-decisions.md](../Design/10-decisions.md) | Every entry is keyed to a position pair |
| Discriminability check | [03-cheap-evidence.md](03-cheap-evidence.md) | Guidance for moving between two positions that cannot be told apart is worthless |

## The tension with the component audit

The audit recommended demoting the transition graph, on the grounds that it contributed to no diagnostic scenario. This plan proposes building substantial content on top of that graph. The two need reconciling rather than leaving in contradiction.

**Proposed resolution: the graph earns its place edge by edge, not as a whole.**

The audit's finding was about *diagnostic* use — knowing which edges exist does not help identify where someone is. That finding stands. Transition guidance is a different use, and it is the one case where edges do work: an edge with usable guidance attached is carrying weight, and an edge with nothing to say about it is decoration.

**This makes the writing process a filter.** Any edge for which no honest guidance can be written should be removed from the model. That is a productive constraint and it should be applied deliberately rather than worked around.

## The document set

Nine files. The split follows how the material will be used, not how the model is organised.

| File | Contents | Priority |
| --- | --- | --- |
| `00-index.md` | Entry point, the stance, how to use the set | Required |
| `01-how-transitions-work.md` | The cross-cutting findings: conditions over persuasion, who holds which lever, why pushing backfires | **Highest** |
| `02-early.md` | First contact fork, guarded evaluation, values refusal | Medium |
| `03-disruption.md` | Identity shock, scope boundary | High |
| `04-working.md` | Calibrated use, overuse, oversight load, integrated practice | High |
| `05-recovery.md` | Burnout recovery and prevention, structural displacement, disengagement | **Highest** |
| `06-timescales.md` | Reasonable durations, and distinguishing slow from stuck | **Highest, and hardest** |
| `07-when-not-to.md` | Transitions that should not be attempted, and why | Required |
| `08-the-hard-decision.md` | Capability versus position; procedural fairness where roles are at risk | High |
| `09-programme-integration.md` | How the guidance plugs into an adoption programme | Medium |

**The three highest priorities are `01`, `05`, and `06`.** `01` carries the finding that makes the rest coherent. `05` covers the only transition with observed evidence behind it. `06` answers the question every manager actually has and is the one most likely to be got wrong.

## The per-entry template

Every transition entry uses the same structure. Uniformity matters more here than elsewhere, because the set will be read by someone looking up one transition under time pressure.

| Section | Content | Notes |
| --- | --- | --- |
| **Edge** | From position → to position | |
| **Voice** | One line of what the person sounds like before the transition | The engineer-readable anchor used throughout the model |
| **What holds it in place** | The mechanism keeping the person where they are | This determines everything below. Write it first |
| **What backfires** | The intervention people reach for, and why it makes things worse | **Lead with this.** See below |
| **What helps** | Conditions to change, ordered by leverage | Conditions, not persuasion techniques |
| **Who can act** | Person / manager / organisation | Most levers are not the person's. Say so plainly |
| **Reasonable time** | An honest range and what it depends on | Ranges, never point estimates |
| **Signals of movement** | Early and later indicators | Must be observable, not inferred |
| **Signals of non-movement** | Distinguishing needs-longer from not-happening | The hardest section. See below |
| **Cost of forcing** | What happens if the transition is pushed | Usually the most reliable content in the entry |
| **Basis** | Evidence status for the entry's claims | Mandatory. See below |
| **Stop boundary** | Where this stops being a management question | Required for anything touching shock or burnout |

### Lead with what backfires

Negative guidance is substantially more robust than positive guidance. That arguing with a guarded evaluator hardens the position is a claim with support in motivated-reasoning research and in ordinary experience. That a specific intervention reliably produces movement is a much stronger claim with nothing behind it.

**Where an entry can only support the negative half, it should say so and stop.** An entry consisting of "here is what makes this worse, and nothing is known about what makes it better" is honest and useful. An entry that invents a positive intervention to look complete is neither.

### The basis field is mandatory

Transition guidance is prescriptive, which raises the evidential bar rather than lowering it. A description that is wrong costs a slightly misdirected conversation. A recommendation that is wrong costs someone a wasted quarter, or pushes someone toward the outcome the guidance was meant to prevent.

Every entry labels its basis:

| Label | Meaning |
| --- | --- |
| **Established** | Supported in an adjacent literature, cited |
| **Reported** | Observed in practice, with the source and its limits named — including author experience, labelled as such |
| **Reasoned** | Follows from the model's structure, not observed |
| **Conjecture** | Neither observed nor entailed. Offered as a hypothesis |

**Where a recommendation is conjecture, the entry states what happens if it is wrong.** This is the single most important discipline in the set.

## Sourcing

With no validation budget, the honest sources are limited. Naming them prevents the set drifting into invention.

| Source | Use | Limits |
| --- | --- | --- |
| **Adjacent literature** | Primary source. Trust calibration, automation ironies, identity threat, job demands-resources all contain relevant intervention findings | Transfer to this context is untested |
| **Author experience** | Legitimate and should be used, labelled as a single case | N=1, unblinded, and the author built the model. Never generalised from |
| **Practitioner reports** | Coaches and managers who have tried something | Anecdotal, and subject to reporting only successes |
| **Model structure** | What follows from the position definitions | Circular. Cannot confirm anything |
| **Invention** | Not a source | Excluded |

**The recovery entry is the strongest in the set** because it has a reported case behind it, and it should be written first for that reason.

## The two hard documents

### `06-timescales.md`

This answers the question managers actually ask — how long is reasonable — and there is no data.

**How to write it honestly.** Give ranges wide enough to be defensible, name what the range depends on, and state that the numbers are practitioner-grade estimates rather than measured durations. Attach the falsifier: if a transition panel were ever run, these are the numbers it would check.

**The section that matters most is non-movement.** A manager needs to distinguish someone moving slowly from someone not moving, and this is where the guidance could do real damage in either direction — writing off someone who needed another quarter, or waiting indefinitely on someone for whom the role has genuinely changed beyond reach.

**Proposed approach:** define non-movement by the *absence of intermediate signals* rather than by elapsed time. Someone who has not moved position but whose boundary has shifted, or who is testing in a new domain, is moving. Someone with no intermediate change after conditions have genuinely improved is a different case. Time alone is a poor criterion and the document should say so.

### `08-the-hard-decision.md`

Roles are being cut, AI capability is becoming a real role requirement, and managers are making selection decisions with or without a framework. Refusing to engage leaves them with gut feel, which is neither validated nor unbiased.

**The distinction the document must carry:**

> **Capability is a legitimate criterion. Position is a different variable.** Whether someone can do the work the role now requires is answerable with ordinary performance evidence. Position does not measure it — a guarded evaluator may be the strongest engineer on the team, and an enthusiastic integrator may be mediocre.

**What the document should contain:**

- Why position is the wrong input for selection, including the practical exposure: guarded evaluation and scope boundary correlate with tenure and depth of craft, which correlate with age. Position as a selection criterion is a well-formed discrimination claim.
- Where the model genuinely helps: preventing premature write-offs of people in recoverable phases, checking whether the organisation created the conditions it is now selecting against, and recognising that burnout is a recoverable low point rather than a capability ceiling.
- **The reframe: the model's contribution here is procedural fairness, not selection.** It establishes whether the person had a fair chance under fair conditions. That makes the eventual decision defensible and happens to be right.
- What a fair chance consists of, concretely enough to audit.

**This document carries the highest misuse risk in the set and should be written last**, once the surrounding material is stable enough to link to.

## What must not be written

| Excluded | Reason |
| --- | --- |
| Guidance for moving someone out of values refusal | Persuading someone out of an ethical position is not a legitimate organisational objective |
| Guidance for moving someone out of a functioning scope boundary | A stable, productive boundary is not a problem. Only the person can decide it should move |
| Anything framed as a technique for changing a person | The stance permits changing conditions, not people |
| Transition probabilities or success rates | No data. Numbers would be fabricated |
| Clinical intervention for shock or burnout | Outside competence. Stop boundaries instead |
| Guidance implying a target position for an individual | The normative layer applies to organisational purpose, never to a person's trajectory |

## Order of work

| Order | File | Rationale |
| --- | --- | --- |
| 1 | `01-how-transitions-work.md` | The cross-cutting finding. Everything else is an instance of it |
| 2 | `05-recovery.md` | The only material with observed evidence. Highest confidence, highest need |
| 3 | `03-disruption.md` | Highest individual demand |
| 4 | `04-working.md` | Largest organisational surface |
| 5 | `06-timescales.md` | Needs the entries written first to estimate against |
| 6 | `07-when-not-to.md` | Short, and clarifies boundaries for everything above |
| 7 | `02-early.md` | Lower demand |
| 8 | `09-programme-integration.md` | Assembly of existing material |
| 9 | `08-the-hard-decision.md` | Highest risk. Write last, on stable ground |

`00-index.md` is written last, as with any index.

## Acceptance tests

An entry is finished when it passes all of these. An entry that cannot is evidence the edge should be removed from the model.

1. **A manager could act on it tomorrow** without assessing anyone psychologically.
2. **It names what backfires**, specifically enough to recognise.
3. **Every claim carries a basis label**, and conjectures state the cost of being wrong.
4. **It says who holds the lever**, and does not assign it to the person when the organisation holds it.
5. **It does not require classifying anyone** to be useful.
6. **It survives the reversibility test** — if the guidance is wrong, nobody's employment changes as a result.
7. **It gives a range, not a number**, wherever duration appears.

## Open questions to resolve during writing

These are expected to be answered by the act of writing and should be recorded as they resolve.

- **Which edges survive?** The set is a filter. Any edge with no honest guidance attached should be cut from the model, and the resulting list will be shorter than the current graph.
- **Is individual-facing guidance viable at all?** Most levers belong to the organisation. If the individual-facing content across the whole set amounts to a page, that should be stated plainly rather than padded.
- **Does prevention dominate?** Preventing burnout is more tractable than recovering from it, and preventing coerced calibration is more tractable than undoing it. If the useful content is consistently preventive, the set should be reorganised around prevention rather than around edges.
- **Does the normative layer belong here or in the model?** The stated-purpose formulation is currently proposed for this set. If it works, it may belong in the model's front matter and should be promoted.

## Effect on prior conclusions

Two documents need revising once this set exists, and the revisions should be made rather than left implicit.

**[../UseCases/09-verdict.md](../UseCases/09-verdict.md)** states that no observed use case exists. That is no longer accurate — there is a recorded case, and it turned on transition information. The verdict's recommendation to shrink is unaffected, since it rested mainly on the utility finding and on prior art, but the evidence section is wrong as written.

**[../UseCases/02-component-audit.md](../UseCases/02-component-audit.md)** recommends demoting the graph. That recommendation should be qualified by the edge-by-edge resolution above: the graph's diagnostic value remains low, and its prescriptive value is the thing this set will establish or fail to establish.
