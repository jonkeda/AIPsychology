# Slice 06 — Scope and Populations

Covers source item **13** (scope statement, AI-native pathway, non-knowledge work, accessibility, delegation ceiling, and economic-access note from slice 04 overflow).

## Item 13a — Scope statement

### What the source asks for

Put a scope statement at the top of V6. Who the model is for. Who it is not.

### Concrete change

First section of `Model6.md`, before any axis or state content:

```markdown
## Scope

This model describes psychological adaptation to AI for **knowledge workers and creatives** who encounter AI *after* building a meaningful professional identity in their domain.

It applies when:

- The person's first substantive exposure to AI happens in adulthood.
- Identity is at stake because skill, expertise, or craft is being replicated by AI.
- The person has a viable economic position (the role can still exist in an AI-collaborative form, even if that form is uncertain). For people whose economic position is not viable, see `populations.md`.

It does **not** describe:

- AI-native users (first meaningful exposure before professional identity formed).
- Non-knowledge-work domains (manual work, physical care, service roles where AI is an economic threat but not an identity-replication threat).
- Emotional or relational AI use (companion apps, support tools, AI therapy).
- AI as assistive technology (users who rely on AI as an access tool, not as a productivity tool competing with their existing skill).
- Users who are already AI experts (AI researchers, engineers, ML practitioners whose professional identity is *about* AI).
- Users facing permanent economic displacement through AI (see `populations.md`).

These populations are not "out of scope" in the sense of being unimportant. They are out of scope because the model's mechanisms (identity-protection cognition, self-efficacy collapse, metacognitive calibration) are designed around the identity-replication threat. Applying those mechanisms to people who face economic replacement without identity replication, or who have no professional identity yet invested in the domain, risks misdiagnosis.
```

---

## Item 13b — Delegation ceiling

### What the source asks for

Re-add the Delegation Ceiling concept from V4, but framed as a *per-person* ceiling on delegation level, separate from current state.

### Concrete change

Add to `01-axes.md` as a third axis, after Identity Stakes and Task Delegation Level:

```markdown
## Delegation Ceiling

A third property of the person (not of the interaction). The maximum Task Delegation Level a person can accept for AI involvement in their core identity domain, given their current state and history.

| Ceiling level | Description |
| --- | --- |
| **D1** | Will accept AI only for information retrieval. Any task execution feels threatening. |
| **D2** | Will accept task execution but not creative delegation. |
| **D3** | Will accept creative delegation but not autonomous partnership. |
| **D4 (unbounded)** | No hard ceiling on delegation for AI in core domain. |

The Delegation Ceiling is **independent of state**. A person in S5 Understanding can still have a D2 ceiling if their prior S3E Ego Shock was severe. A person in S3B Bargaining can have a D3 ceiling for low-stakes domains while maintaining D1 for their core craft.

The ceiling is not fixed. It changes through:

- Sustained skill-building (seeing one's own contribution survive alongside AI)
- Readiness work (therapy, coaching, peer support)
- Natural ceiling shifts following capability exposure

Forcing delegation beyond a person's current ceiling is the mechanism behind *coerced S5 Understanding* — the person appears to integrate but has not changed their ceiling; the underlying resistance re-surfaces later.

Note: The Delegation Ceiling is a **descriptive** concept. No measurement instrument currently exists for it.
```

---

## Item 13c — AI-native pathway

### What the source asks for

Add a separate pathway for users whose first real AI exposure comes before or alongside forming professional identity. These people can bypass the Initial Encounter → shock sequence entirely.

### Concrete change

Add to `populations.md`:

```markdown
## AI-Native Users

Users whose substantive exposure to AI comes *before* they form domain identity are increasingly common. This population includes:

- Students who used AI throughout their education and are now entering the workforce.
- Early-career workers whose first professional tools included AI from day one.
- People whose domain identity is still forming when AI enters their professional life.

### How the model applies differently

These users often bypass S1 Initial Encounter, S2D Defensive Resistance, and S3E Ego Shock in the classic sense. There is no prior-competence identity to be threatened — the identity is forming with AI already in it. Their path is more likely:

- S0 Baseline → S5 Understanding (direct, because no identity is being displaced)
- S0 Baseline → S7I Identity Expansion (forming a professional identity that includes AI from the start)

S2D Defensive Resistance and S3E Ego Shock can still appear for AI-native users — but typically when they try to learn a skill *without* AI and discover they cannot, or when a new AI capability arrives in a domain they have now built identity in (so the model applies to later iterations, not the first encounter).

### What this means for the model

The model's full arc is an adult-transition model. AI-native users may experience fragments of the arc, in different order, or not at all. The core mechanisms (identity protection, self-efficacy, metacognitive calibration) are still present; the trigger and sequence differ.

V6 does not attempt to model the AI-native trajectory in full. This note marks the gap.
```

---

## Item 13d — Non-knowledge-work subsection

### Concrete change

Add to `populations.md`:

```markdown
## Non-Knowledge-Work Domains

In physical care roles, manual trades, and routine service work, AI's primary threat is economic (replacement risk) rather than psychological (identity threat through skill replication). The model's mechanism layer sits differently:

- **Task Delegation Level maps differently.** D1 Information (diagnostic tools, scheduling) and D2 Task Execution (automation of routine decisions) are the relevant levels. D3 Creative Delegation and D4 Autonomous Partnership rarely apply.
- **S3E Ego Shock manifests as economic fear, not identity disruption.** The discomfort is "will there be work for me?" not "if AI can do this, what does that make me?" The distinction matters for intervention: identity work is the wrong prescription.
- **S3B Bargaining is less available.** Bargaining requires a bounded domain to retreat to. In work where AI replaces the entire role rather than a skill, there is no residual domain to bargain around.
- **S2D Defensive Resistance can be more durable.** Without a viable integration path, resistance is rational, not defensive.

The model can still describe *what the psychological experience looks like* for these workers. It cannot tell them whether integration is possible. That is an economic question, not a psychological one.
```

---

## Item 13e — Accessibility / assistive-tech note

### Concrete change

Add to `populations.md` and add a callout in `states/S5-understanding.md`:

```markdown
## AI as Assistive Technology

This model assumes the user's baseline capability exists and AI is matching (replicating) an existing skill. Users who rely on AI as assistive technology — for whom AI provides access to tasks they could not otherwise perform, not competition with tasks they already perform — are outside the model's mechanism layer.

For these users:

- S3E Ego Shock is typically absent. The tool provides capability, not competition.
- S7I Identity Expansion is common. AI is constitutive of what they can do, not threatening.
- S2D Defensive Resistance rarely applies, unless the AI tool fails to perform its assistive function.

This use case requires separate analysis. Applying the identity-threat model to assistive-tech users risks misframing what is happening to them.
```

---

## Item 13f — S0 Baseline includes never-AI users

### What the source asks for

S0 Baseline is currently framed as "before first encounter" — implying everyone eventually moves to S1. In practice, S0 also covers people who have never used AI and never will. This is a stable, valid endpoint, not a transitional state.

### Concrete change

Add to `states/S0-baseline.md`:

```markdown
## Two readings of S0 Baseline

S0 Baseline applies to two distinct populations:

1. **Pre-encounter users.** People who have not yet had a substantive AI exposure but are likely to. For these users, S0 is transitional — S1 Initial Encounter is the next step.
2. **Permanent non-users.** People who have not used AI and will not. They have made — or had made for them — a stable lifelong stance of non-use. For these users, S0 is a terminal state, not a transitional one.

The second population includes people whose work, life context, or personal preference keeps them outside the AI adoption trajectory entirely. They are not in S2D Defensive Resistance (which requires having considered and rejected AI on identity-threat grounds) nor in PEN Pre-emptive Non-Adoption (which requires an active values-based rejection). They are simply outside the system.

### What this means for the model

- S0 is not exclusively a launching pad. For some people it is the entire model.
- The trigger that moves someone from S0 to S1 is contact, not exposure-in-the-abstract. Reading about AI does not move a person from S0 to S1; using or being asked to use it does.
- S0 → S1 is not inevitable. The model should not be read as predicting that everyone will eventually engage.

This reading is a clarification, not a structural change. No new states or edges are introduced.
```

Add to `populations.md`:

```markdown
## Permanent Non-Users

Some people will never use AI. The reasons vary — work context that does not involve AI, life situation that places AI outside daily relevance, or personal preference. They sit permanently in S0 Baseline.

This population is in scope for the model only in the sense that S0 has a defined meaning for them. The rest of the model does not apply: there is no transition path to model, no defensive structure to analyse, no integration to support. They are outside the system, and the model should not be used to characterise them as "stuck" or "resistant" — they have not engaged at all.

A practitioner using this model should be careful not to mistake permanent non-use for S2D Defensive Resistance. The signal: ask whether the person has formed a stance about AI. S2D requires an active stance defended against evidence; permanent non-use requires no stance at all.
```

---

## Item 13 overflow — Economic access barriers

Overflow from slice 04, item 8: some people are held in S2D Defensive Resistance or S3B Bargaining not for psychological reasons but because they cannot access the tools that would let them progress.

### Concrete change

Add to `populations.md`:

```markdown
## Economic Access Barriers

The model assumes the person can access AI tools. When access is blocked by cost, organisational gatekeeping, or geographic availability, the psychological states can persist for structural rather than psychological reasons:

- A person in S3B Bargaining may remain there indefinitely not because of identity protection but because they cannot afford the model that would have changed their view.
- S7B Burnout can result from cost cycles: access to good tools → integration → cost increase → access withdrawn → disrupted workflow.
- S2T Trust Evaluation stalls when the person cannot evaluate the tools they have read about but cannot use.

Interventions for structurally-held states should address access before psychology.
```

---

## Verification checklist

- [ ] `Model6.md` opens with the scope statement.
- [ ] `01-axes.md` contains the Delegation Ceiling as a third axis.
- [ ] `populations.md` exists with all six sections: AI-native, non-knowledge-work, assistive tech, permanent non-users, economic access, economic displacement (from slice 07).
- [ ] `states/S0-baseline.md` distinguishes pre-encounter from permanent non-user readings.
- [ ] S5 Understanding file has an assistive-tech callout.
- [ ] Scope statement is readable on its own — a practitioner can tell in 30 seconds whether the model applies to their situation.
