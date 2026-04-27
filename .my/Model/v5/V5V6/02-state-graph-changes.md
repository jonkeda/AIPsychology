# Slice 02 — State Graph Changes

Covers source items **2** (S2T → S2D edge), **4** (S3E → S5 edge), and **5** (state occupancy rules).

## Item 2 — S2T Trust Evaluation can convert to S2D Defensive Resistance

### What the source asks for

The V5 fork after S1 Initial Encounter splits people into S2T or S2D based on Identity Stakes. The source asks for an additional edge: S2T → S2D, fired when testing reveals a capability that newly threatens the person's identity.

### Concrete change

Update `states/S1-initial-encounter.md` to read:

> Low-stakes encounters typically move to S2T Trust Evaluation. High-stakes encounters typically move to S2D Defensive Resistance. The split is a tendency, not a deterministic rule — a person with high stakes who is psychologically secure may enter S2T, and a person with apparently low stakes may discover during testing that the stakes were higher than they realised.

Update `states/S2T-trust-evaluation.md`:

- Description line: change to *"Non-defensive evaluation. Can convert to defensive evaluation if testing reveals a threat the person had not anticipated."*
- Add transition: `S2T → S2D — when testing reveals a capability that threatens identity in a way the person did not anticipate going in.`

Update `states/S2D-defensive-resistance.md`:

- Add inbound edge from S2T to the transitions list.
- In the description, note that some S2D occupants arrived from S1 directly (the typical high-stakes path) and some arrived via S2T (testing surfaced a threat).

### Mermaid update

Already shown in slice 01. The relevant edges:

```
S1 -->|low stakes| S2T
S1 -->|high stakes| S2D
S2T -->|threat surfaces| S2D
```

### Why this matters

V5 implies the fork is a one-time decision at S1. In practice, people sometimes start S2T thinking the stakes are low, run a few tests, and discover the tool is good at something they cared about. That is a different psychological event from "started S2D from the beginning" and the model should describe it.

---

## Item 4 — Direct S3E Ego Shock → S5 Understanding edge

### What the source asks for

V5 routes S3E Ego Shock to S5 Understanding only via S3B Bargaining. The source asks for a direct S3E → S5 edge for the rare case where a person resolves the identity threat without bargaining.

### Concrete change

Update `states/S3E-ego-shock.md`:

- Add transition: `S3E → S5 — rare. Requires the person to face the identity threat directly without defense or compromise and rebuild self-concept on the spot. Most people who appear to do this are actually doing accelerated S3B Bargaining and revisiting it later.`

The "rare" qualifier matters. Adding this edge is honest, but the model should not invite readers to aim for it as the preferred path. Most people route through S3B Bargaining for a reason.

### Mermaid update

Add the edge:

```
S3E --> S5
```

Already in the diagram in slice 01.

### Open question

How does the implementer distinguish "direct S3E → S5" from "fast S3E → S3B → S5"? In practice they are observationally indistinguishable on a single observation. Note this in `limits-of-operationalization.md`: the direct path is a theoretical possibility; whether anyone actually takes it cleanly is unverified.

---

## Item 5 — State occupancy and coexistence rules

### What the source asks for

Spell out which S6 states can coexist with each other, and which can coexist with which S7 states. The current model implies parallel multiple-occupancy without saying which combinations are stable.

### Concrete change

Add a new section in `02-state-graph.md` titled **State Occupancy**, immediately below the diagram:

```markdown
## State Occupancy

States in this model can be **mutually exclusive**, **stably coexisting**, or **transitionally co-occurring**. The rules below are descriptive; they describe what tends to be observed, not what is logically forbidden.

### S6 states (parallel, with constraints)

- **S6E Enthusiastic Overuse and S6D Dependent Overuse are mutually exclusive.** They have opposite affect: S6E is energised and uncritical, S6D is anxious and self-doubting. A person can transition from one to the other (typically S6E → S6D after a confidence-eroding event) but does not stably occupy both.
- **S6R Driven Overuse and S6S Social Overuse can coexist.** In high-pressure cultures where being productive *is* the conformity, the two reinforce each other.
- **S6E Enthusiastic Overuse and S6R Driven Overuse can coexist** in startup-flavored environments where personal enthusiasm aligns with productivity pressure.
- **S6D Dependent Overuse and S6S Social Overuse can coexist** in compliance-heavy environments where the person uses AI both because they doubt themselves and because everyone is watching.
- **S6E Enthusiastic Overuse + S6D Dependent Overuse and S6R Driven Overuse + S6S Social Overuse are unstable** — the affective profiles do not match.

### S7 states (parallel, intentionally overlapping)

Any S7 state can coexist with any other S7 state. The most common combinations:

- S7M Maturity + S7E Ethical Integration (reflective practitioner)
- S7I Identity Expansion + S7V Evangelism (creative leader)
- S7M Maturity + S7V Evangelism (steady mentor)
- S7I Identity Expansion + S7E Ethical Integration (creator wrestling with what they are creating)

S7B Burnout co-occurs with the others as a phase, not a stable coexistence — when a person is in S7B Burnout they are typically *not actively occupying* their other end states; those resume on return.

### S6 to S7 transitions (not coexistence)

- **S6E Enthusiastic Overuse** can transition to **S7M Maturity** or **S7I Identity Expansion** but does not stably coexist with either. Maturity and enthusiasm-without-criticism are not compatible long-term residences.
- **S6D Dependent Overuse**, **S6R Driven Overuse**, **S6S Social Overuse** all lead most often to **S7B Burnout** as their primary exit. Direct routes from these to S7M Maturity are rare and usually require a structural change (new role, new manager, illness forcing re-evaluation).

### Cross-cutting

- **Dropout** is reachable from every state.
- **S3E Ego Shock** is reachable as a regression from every S5–S7 state.
- **S3X Structural Displacement** (see slice 07) is reachable from S3E Ego Shock when economic non-viability is established.
```

### Why this matters

V5 says "S7 states overlap" but does not say which S6 states overlap and which do not. Practitioners reading the model end up guessing. Spelling the rules out makes the model usable as a coaching reference.

### Open question

The S6E + S6R and S6D + S6S coexistence claims are based on observation of two cultural archetypes (startup, compliance-heavy). They are not directly tested. Mark them as conjecture in `limits-of-operationalization.md`.

---

## Verification checklist

- [ ] `S1`, `S2T`, `S2D` files reflect the new fork-and-convert wording.
- [ ] `S3E` file has the direct S3E → S5 edge with the "rare" qualifier.
- [ ] `02-state-graph.md` contains the State Occupancy section.
- [ ] Mermaid diagram shows the new edges.
- [ ] Conjectural occupancy claims are flagged in `limits-of-operationalization.md`.
