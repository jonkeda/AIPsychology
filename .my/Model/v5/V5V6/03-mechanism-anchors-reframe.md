# Slice 03 — Mechanism Anchors Reframe

Covers source items **6** (mechanism anchors don't diagnose) and **12** (rename to "Related literature").

## What the source asks for

Two related changes:

1. Stop calling them "Mechanism anchors." The label suggests the cited mechanism *causes* the state, when the connection is conceptual and unproven. Rename to **Related literature**.
2. Add a sentence saying the related literature is an explanation, not a diagnostic tool. Practitioners cannot identify someone's state by checking which mechanism applies.

## Concrete changes

### Global rename

In every state file, rename the heading:

- From: `**Mechanism anchor:**`
- To: `## Related literature`

The colon-style inline emphasis becomes a proper subsection heading. This matches the per-state file shape in slice 01.

The body of each section can stay almost identical; only the framing language changes.

### Reframe the language inside each section

V5 uses sentences like:

> **Mechanism anchor:** **identity-protection cognition** — the tendency to evaluate evidence in ways that defend a valued self-concept.

Change to:

> Conceptually related to **identity-protection cognition** (the tendency to evaluate evidence in ways that defend a valued self-concept). This is offered as a frame for thinking about S2D Defensive Resistance, not as a tested causal claim. The state is named for the observed behavior; the literature offers a vocabulary for why such behavior is plausible.

The pattern: replace "Mechanism anchor: X — Y" with "Conceptually related to X (Y)." Then add a one-sentence reminder that this is conceptual, not diagnostic.

### Add a one-time diagnostic disclaimer

Once, prominently, in `Model6.md` (the entry point), add:

```markdown
## Related literature is conceptual, not diagnostic

Each state in this model is connected to one or more concepts from psychology and adjacent fields. These connections are **vocabulary**, not **mechanism**. Knowing that S3E Ego Shock is conceptually related to self-efficacy collapse (Bandura) tells you what kind of phenomenon S3E belongs to. It does not let you diagnose S3E in a person, and it does not commit the model to the claim that self-efficacy collapse is the cause of S3E.

The model uses related literature to:

- Anchor each state in existing thinking, so the reader knows the construct is not invented from scratch.
- Provide a starting point for further reading.
- Make the conceptual content of each state more legible to a reader with academic background.

The model does **not** use related literature to:

- Predict what a person will do.
- Identify which state a person is in.
- Claim a causal mechanism without empirical support.
```

This block lives once in `Model6.md` and is referenced from each state file rather than repeated.

### Cite the major borrowings by name (item 14a)

V5 hides borrowings inside parentheticals. Per source item 14a, V6 should name the borrowings explicitly. Specifically:

- **Technology Acceptance Model (Davis, 1989)** — borrowed for S2T Trust Evaluation: adoption is driven by perceived usefulness and perceived ease of use.
- **Diffusion of Innovations (Rogers)** — borrowed for S5 Understanding: adoption depends on perceived compatibility with existing practice.
- **Transtheoretical Model / Stages of Change (Prochaska and DiClemente)** — borrowed for the cycling property: people revisit earlier states, change is non-linear.
- **Gartner Hype Cycle** — borrowed for the S6E Enthusiastic Overuse → S5 Understanding regression: the "trough of disillusionment" structure.
- **Cognitive dissonance (Festinger)** — already cited; keep but make the borrowing explicit in S3B Bargaining.
- **Identity-protection cognition (Kahan)** — already cited; keep for S2D Defensive Resistance.
- **Self-efficacy (Bandura)** — already cited; keep for S3E Ego Shock and S6D Dependent Overuse.
- **Conformity research (Asch)** — already cited; keep for S6S Social Overuse.
- **Generativity (Erikson)** — already cited; keep for S7V Evangelism.
- **Extended self (Belk)** — already cited; keep for S7I Identity Expansion.

Format inside each state file:

```markdown
## Related literature

This state borrows from **[Construct]** ([Author], [year if useful]) — [one-sentence plain-English gloss]. The borrowing is conceptual: the model uses [Construct] as vocabulary for the phenomenon, not as a tested causal mechanism for the state.

[If the state borrows from more than one construct, repeat the paragraph for each.]
```

The change from V5 is: each citation gets a one-sentence gloss, the author is named explicitly, and the conceptual-not-causal disclaimer is repeated per state.

## Risks / open questions

- **Repetition.** If every state file repeats "the borrowing is conceptual, not causal," the document becomes tedious. Mitigation: state the rule once in `Model6.md`, then in each state file say it briefly: *"Borrowed conceptually from X."*
- **Loss of cleverness.** Some V5 mechanism descriptions are well-written ("a secondary mechanism is **terror management** in the loose sense"). Don't strip the substance to satisfy the rename. Keep the content; change the framing.
- **TAM / Rogers / TTM / Gartner are dated.** Naming them by name is correct per the source request, but each one has its own debates and limitations. The one-sentence gloss should be neutral and not endorse the framework as a whole.

## Verification checklist

- [ ] No file contains the heading "Mechanism anchor."
- [ ] Every state file has a "Related literature" section.
- [ ] `Model6.md` contains the one-time conceptual-not-diagnostic disclaimer.
- [ ] TAM, Rogers, TTM, and Gartner are named explicitly somewhere they are borrowed from.
- [ ] Every related-literature citation has a one-sentence plain-English gloss.
