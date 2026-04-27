# Slice 09 — Front Matter and Meaning

Covers source items **11** (pick a lane: descriptive), **14b** (lead with Identity Stakes × TDL), **14d** (move limits warning to front), **14e** (relationship to prior frameworks), **14g** (describe, don't prescribe), **15** (what does the model mean), **16** (healthiness), and the usage part of **17**.

## Item 11 — Commit to descriptive framing

### What the source asks for

V5 sits between "testable" and "descriptive." The source picks a lane: V6 is **descriptive**. It is a thinking tool and shared vocabulary, not a causal model. Testability pathways are documented but the model does not claim to be empirically grounded.

### Concrete change

In `Model6.md`, after the scope section, add:

```markdown
## What kind of model this is

This model is **descriptive**. It provides:

- Names for recognisable psychological patterns
- A graph of transitions between those patterns
- Modulating factors that change how intensely a pattern is experienced

It does **not** provide:

- Causal mechanisms (the related literature sections indicate conceptual connections, not tested causes)
- Empirical predictions (transition probabilities are not specified)
- Diagnostic instruments (no validated test places someone in a state)
- Treatment protocols

A model can be useful without being empirically tested. This one offers vocabulary for conversations that previously had no shared language, a map for practitioners who are trying to orient themselves, and a set of hypotheses for future research. Until testing occurs, treat every state description as a well-grounded hypothesis, not an established fact.

Where the model makes a claim that goes beyond what has been observed, it marks this explicitly as: **Conjecture —** awaiting data.

Where a claim could be tested with a defined study, it marks this as: **Testable —** see `limits-of-operationalization.md`.
```

---

## Item 14b — Lead with Identity Stakes × Task Delegation Level as the headline contribution

### What the source asks for

The two-axis modulation is what V5 added to V4. V6 should make this the headline before the state descriptions, so readers know upfront what is genuinely new.

### Concrete change

In `Model6.md`, before the link to `01-axes.md`:

```markdown
## What this model adds

The state-graph structure (recognisable patterns with transition rules) appears in prior frameworks, notably the Technology Acceptance Model (Davis, 1989) and diffusion of innovations (Rogers). What this model adds is **two modulating axes** that change the *intensity* of each state rather than changing which state a person is in:

1. **Identity Stakes** — how central the skill AI is replicating is to the person's professional self-concept. High stakes amplify every state; low stakes compress or skip the difficult ones.
2. **Task Delegation Level** — how much cognitive authority the person hands to AI in a single interaction. D4 autonomous partnership in a high-stakes domain is the most psychologically activating combination.

These two axes are independent, per-domain, and per-interaction. They do not put people on a track — they change the texture of wherever they are.

A third property — **Delegation Ceiling** — describes the maximum delegation level a person can accept in their core domain given their history, separate from their current state. See `01-axes.md`.
```

---

## Item 14d — Limits warning moved to front; inline conjecture markers

### What the source asks for

V5 has a comprehensive "Limits of operationalization" section at the end. V6 moves the warning to the front and adds inline markers at each unproven claim.

### Concrete change

In `Model6.md`, near the top (after "what kind of model this is"):

```markdown
## How to read the claims in this model

Three levels of epistemic confidence appear throughout:

- **(no marker)** — an established or widely observed pattern with reasonable grounding in related literature.
- **Conjecture** — a claim the model makes because it is a useful frame, not because it is observed. Each conjecture is marked where it appears.
- **Testable** — a claim that could be falsified with a defined study. Marked where they appear; full protocols in `limits-of-operationalization.md`.

Everything the V5 "Limits of operationalization" section listed as conjecture is still conjecture in V6. A summary lives in `limits-of-operationalization.md`. The reader does not need to reach the end of the document to know the model's epistemic status.
```

In every state file, add inline markers next to each claim that V5 already listed as conjecture. For example, in `states/S3B-bargaining.md`:

> The proposed distinguishing signal between S3B and S7M is a **Conjecture** — it requires longitudinal observation across multiple model releases and is contaminated by self-report.

---

## Item 14e — Relationship to prior frameworks

### Concrete change

In `00-relationship-to-prior.md`:

```markdown
# Relationship to Prior Frameworks

This model is an extension of prior frameworks, not a replacement. Understanding what it borrows and what it adds clarifies when to use it instead of, or alongside, its predecessors.

## Technology Acceptance Model (Davis, 1989)

TAM says adoption is driven by perceived usefulness and perceived ease of use. It is a snapshot model: it explains whether someone will adopt, not what happens to their psychology over time if adoption is difficult. This model picks up where TAM stops — it describes the psychological arc that follows the initial adoption decision, especially when that decision is complicated by identity stakes.

## Diffusion of Innovations (Rogers)

Rogers describes how innovations spread through populations over time — from early adopters through late majority and laggards. That is a population-level model, not an individual-level one. This model is individual-level: it describes one person's trajectory, not a population curve. The two are compatible; Rogers tells you where someone sits in the adoption distribution, this model tells you what is happening psychologically to the person at that position.

## Transtheoretical Model / Stages of Change (Prochaska and DiClemente)

TTM describes behavior change as moving through pre-contemplation, contemplation, preparation, action, and maintenance, with the possibility of relapse at any stage. This model borrows the relapse-is-normal framing and the multi-state structure. It differs in that the states here are not motivational stages toward a goal — someone in S3B Bargaining is not "pre-contemplating" S7M Maturity; they are in a legitimate stable position that may persist for years. Progression through the model is not the goal.

## Gartner Hype Cycle

The Hype Cycle describes a technology's trajectory through inflated expectations, disillusionment, and eventually a plateau of productivity. It maps loosely onto this model: the S6E Enthusiastic Overuse state resembles the Peak of Inflated Expectations, the S3E Ego Shock / S6D Dependent Overuse period resembles the Trough of Disillusionment, and S7M Maturity resembles the Plateau. The Gartner model is a population-level technology-maturity model; this model is an individual-level psychological model. They describe similar shapes from different vantage points.

## V4 of this model

V5 renamed V4's S1.5 Trust Evaluation and S2 Defensive Resistance to S2T and S2D respectively, added mechanism anchors, refined dropout into two severity axes, and added a limits of operationalization section. V6 removes the mechanism-anchor framing (replacing it with related literature), adds four new path elements (S2T → S2D edge, direct S3E → S5, S3X Structural Displacement, PEN Pre-emptive Non-Adoption), explicitly commits to descriptive framing, and splits into separate files per state.
```

---

## Item 14g — Describe, don't prescribe

### Concrete change

In `Model6.md` scope section or in the "what kind of model this is" section, add:

```markdown
This model describes observed paths, not recommended paths. It should not be used to push people through transitions faster, or to set a target state as a goal for someone. Its value is in helping practitioners understand where someone is, not in helping them engineer where that person goes next. The right outcome for any individual depends on their situation, domain, values, and economic position — not on reaching any particular state in this model.
```

---

## Item 15 — What does the model mean (from 3-Questions.md / 1-Answers)

### Concrete change

A dedicated section in `Model6.md` drawn from 1-Answers-Model5.md section A.1:

```markdown
## What this model is

This model is a map of how a person's relationship with AI changes over time. It is a directed graph of **states** — labeled snapshots of how someone is currently relating to AI — with rules about how they move between those states.

Read it as three things stacked together:

1. **A vocabulary.** Names for recognisable patterns — Ego Shock, Bargaining, Maturity, Burnout. Once you know the names, you can say "she is in S2D Defensive Resistance about her writing but S5 Understanding about her email" and another reader knows what you mean.
2. **A graph of transitions.** Arrows that describe which states tend to follow which. These are tendencies, not laws.
3. **Two modulating axes.** Identity Stakes and Task Delegation Level change the intensity of whatever state the person is in.

What the model is **not**:

- **Not a stage theory.** People do not march from S1 Initial Encounter to S7 in order. They loop, regress, and occupy multiple states at once across different domains.
- **Not a diagnosis.** No test places someone in a state. It is a frame for thinking, not a clinical instrument.
- **Not a value judgment.** S7B Burnout and S3B Bargaining are not failures. They are legitimate places to be.
- **Not a prescription.** The model describes paths; it does not recommend them.
```

---

## Item 16 — Healthiness

### Concrete change

Create `healthiness.md` with the framing from 1-Answers-Model5.md section B:

```markdown
# Healthiness

The model does not use the word "healthy" anywhere in its state descriptions. This section is an interpretive layer — a reading of the model through a healthiness lens. It is flagged as interpretation, not direct claim.

## Healthiness levels

| Level | Description | States |
| --- | --- | --- |
| **Sustainable** | Can persist indefinitely without psychological cost | S7M Maturity, S7I Identity Expansion, S7E Ethical Integration, S5 Understanding, S3B Bargaining (for many people) |
| **Sustainable with cost** | Can persist but draws on resources | S6E Enthusiastic Overuse, S6R Driven Overuse, S6S Social Overuse, S7V Evangelism |
| **Transitional only** | Healthy as a passage, harmful as a long-term residence | S3E Ego Shock, S2T Trust Evaluation, S2D Defensive Resistance, S1 Initial Encounter |
| **Recovery** | Signals that something upstream broke | S7B Burnout |

## Per-state healthiness summary

- **S7M Maturity** — calibrated, bounded, evidence-driven. The cleanest sustainable state.
- **S7I Identity Expansion** — sustainable; growth is built in.
- **S7E Ethical Integration** — sustainable; reflection is built in.
- **S5 Understanding** — functional and stable; healthy, if less integrated than S7M.
- **S3B Bargaining** — healthy for the right person in the right phase. The model explicitly says: not a failure state, many people remain productive here for years.
- **S7V Evangelism** — healthy when grounded in genuine depth of experience; collapses toward S6E or S6S flavors when not.
- **S6E Enthusiastic Overuse** — healthy short-term, costly long-term.
- **S6R Driven Overuse** and **S6S Social Overuse** — sustainable only as long as external pressure does not exceed personal capacity.
- **S2D Defensive Resistance** and **S6S Dependent Overuse** — sustainable but corrosive; person fights their own judgment.
- **S3E Ego Shock** — healthy as a transition, unhealthy as a residence.
- **S7B Burnout** — a legitimate recovery state, not a failure. Living there permanently means cost outran value.

## What a healthy state looks like for an individual

- **Calibrated use.** The person knows when AI helps and when it does not, and routes work accordingly.
- **Stable identity.** Their sense of who they are is not under active threat from the tool.
- **No reactive override.** Decisions about AI use come from evidence, not from peer pressure, panic, or the need to defend a self-image.
- **Recoverable from regression.** A capability jump can knock them back temporarily; they have the resources to climb back.
- **Sustainable energy budget.** They are not running so hot that burnout is the next step.

## What a healthy organisation looks like

- **A wide spread, not a forced cluster.** People are at different states for legitimate reasons.
- **Few people stuck in S2D Defensive Resistance, S3E Ego Shock, or S6S Dependent Overuse.** These are corrosive long-term and signal the org's framing is creating unnecessary identity threat.
- **No incentives that manufacture S6R Driven Overuse or S6S Social Overuse.** Productivity dashboards that count AI use, leaderboards, public AI metrics — these create S6R and S6S.
- **Recovery slots available.** S7B Burnout is not career-ending.
- **Real S7V Evangelism voices.** Internal evangelists have genuine depth of engagement, not just early enthusiasm.
- **Domain-aware.** The org recognises that the same person can be in S5 Understanding for one task and S3E Ego Shock for another.
```

---

## Usage section

Create `usage.md`:

```markdown
# Usage

## What the model can be used for

- **Recognition.** Naming what is happening to you or someone else.
- **Vocabulary in a 1:1.** Shared language that keeps a conversation from collapsing into pro-AI vs anti-AI.
- **Mapping interventions to states.** The right response to S3E Ego Shock is wrong for S6E Enthusiastic Overuse, and vice versa.
- **Triage of dropouts.** The two severity axes plus the reversibility test separate fixable practical dropouts from identity-driven dropouts.
- **Anticipating regression.** The model predicts that capability jumps push S5 and S7 people back to S3E. Knowing this lets you prepare.
- **Org-design conversations.** Distribution across states is diagnostic. A workforce clustered in S2D Defensive Resistance has a different problem from one clustered in S6E Enthusiastic Overuse.

## What the model cannot (yet) be used for

- **Diagnosis.** No validated test places someone in a state. Self-report is unreliable once someone has read the model.
- **Prediction.** The model has no transition probabilities. It describes which transitions are legal, not which are likely.
- **Quantitative measurement.** The dropout severity axes are 0–10 but inter-rater reliability has not been established.
- **Universal claims.** Cultural variability is hypothesized, not tested. Claims about "most people" are qualitative.
- **Clinical therapy.** The model is not a treatment protocol.
- **Performance management.** Using the model to grade or rank people is a category error.

## Until testing occurs

Until the model's testable claims are tested (see `limits-of-operationalization.md`), treat every state description as a well-grounded hypothesis. The model's value is in conversations and decisions, not in measured outcomes. It is a shared vocabulary before it is anything else.
```

---

## Verification checklist

- [ ] `Model6.md` contains: scope, what kind of model, what it adds, how to read claims, describe-don't-prescribe, what this model is (meaning).
- [ ] `00-relationship-to-prior.md` exists with TAM, Rogers, TTM, Gartner, and V4 sections.
- [ ] `healthiness.md` exists with the per-state table and individual/org markers.
- [ ] `usage.md` exists with can/cannot split.
- [ ] Inline **Conjecture** and **Testable** markers added to first pass of state files.
- [ ] `limits-of-operationalization.md` is a summary pointing to inline markers, not the only place they appear.
