# Slice 05 — Identity-Domain Scoping

Covers source items **10** (defensiveness only fires inside identity-threatened domains) and **18** (S3B Bargaining vs S7M Maturity rewrite from 3-Answers).

## Item 10 — Defensive evaluation is domain-scoped

### What the source asks for

V5 describes S2D Defensive Resistance as if it were a global stance toward AI. In practice, the same person is S2D about AI in their core domain and not S2D at all about AI in adjacent domains. The graphic designer who is S2D about AI for design may be perfectly relaxed about AI for writing emails.

### Concrete change

Update `states/S2D-defensive-resistance.md`. Add a section near the top:

```markdown
## Domain scoping

S2D Defensive Resistance is **per-domain**, not per-person. The same individual can be S2D in one domain and S2T Trust Evaluation, S5 Understanding, or S7M Maturity in another.

The defensive response fires only in domains where the person's identity is on the line. Identity Stakes determine whether the domain qualifies. A senior craftsperson can be:

- S2D Defensive Resistance about AI in their craft (high stakes)
- S2T Trust Evaluation about AI for adjacent professional tasks (moderate stakes)
- S5 Understanding about AI for travel planning (low stakes)
- S7M Maturity about AI for research summarisation (long-evaluated, low stakes)

This means a single person occupies multiple states at the same time, one per relevant domain. The model is a graph of states a *person-in-domain* can be in, not a graph of states a *person* can be in.

When practitioners use this model, they should ask "which domain are we talking about?" before asking "which state are they in?"
```

This needs a corresponding short note in `Model6.md`'s axes section and in the entry-point reading guide:

> The model describes states of *a person in a specific domain*, not states of a whole person. Most people occupy several states at once across different domains.

### Knock-on effect

Update the Identity Stakes axis description to make this explicit:

> Identity Stakes is a property of the person *relative to a domain*. The same person can have low Stakes in one domain and high Stakes in another. The model's behavior in any given situation depends on which domain is in play.

V5 already says this once; V6 should say it loudly enough that no reader misses it.

---

## Item 18 — S3B Bargaining vs S7M Maturity rewrite

### What the source asks for

The substantive content for this rewrite is in [3-Answers-Model5.md](../../Questions/3-Answers-Model5.md), section A.1. The headline points:

1. The current V5 distinction (boundaries move reactively in S3B, evidence-driven in S7M) is real but incomplete.
2. The missing dimension is *where* the boundary sits. S3B draws it around the identity-threatened domain. S7M draws it at the competence line.
3. The intuition that "S3B = lower-D tasks" is correct in practice but the operative axis is Identity Stakes, not Task Delegation Level. Identity-threatened domains tend to contain higher-D work, so S3B users end up confined to lower-D tasks as a consequence.
4. The two states feel different from the inside: S3B feels like protecting something; S7M feels like routing.

### Concrete change

In `states/S3B-bargaining.md`, add or update the **Heuristic distinction from S7M Maturity** section:

```markdown
## Heuristic distinction from S7M Maturity

S3B Bargaining and S7M Maturity both look like "uses AI for some things, not others" from outside. They differ on two axes:

### Where the boundary sits

The boundary in S3B Bargaining is drawn **around the identity-threatened domain**. AI is allowed everywhere except where it would touch the skill the person built their self-concept around. Inside that protected domain, even small uses feel wrong; outside it, even large uses feel fine.

The boundary in S7M Maturity is drawn **at the competence line**. The S7M user uses AI inside their core domain when capability evidence supports it, and refuses AI outside their core domain when capability evidence does not. The level of identity engagement does not determine the boundary — the quality of AI on the specific task does.

A working heuristic: if the boundary maps cleanly onto the person's professional identity, it is S3B. If the boundary maps onto where AI is and isn't reliable, it is S7M.

### How the boundary moves

In S3B, boundaries are renegotiated **under capability pressure**. When a new model release crosses one of the self-imposed lines, the line moves quickly without documented testing.

In S7M, boundaries move **only after measured evidence** — a benchmark, a real-world failure, a controlled comparison.

### How they feel from the inside

S3B feels like protecting something. The restriction has emotional weight — *this is the stuff I won't let AI touch*.

S7M feels like routing. The restriction is pragmatic — *AI is not good enough at this yet*, or *the cost of checking its work exceeds the benefit*.

### Why "S3B = lower-D, S7M = all D-levels" is roughly true but misleading

Identity-threatened domains tend to be where the person does their higher-D work — their core craft, the thing they trained for. So S3B users in practice often confine AI to lower-D tasks. But the operative axis is Identity Stakes, not Task Delegation Level. An S3B user in a high-stakes domain will refuse AI even at D1 Information level inside that domain (asking AI to summarise their own portfolio feels wrong) while happily using AI at D3 Creative Delegation in a low-stakes domain (drafting a vacation itinerary).
```

In `states/S7M-maturity.md`, add the mirror text:

```markdown
## Heuristic distinction from S3B Bargaining

(See `S3B-bargaining.md` for the full discussion.)

S7M Maturity differs from S3B Bargaining in two axes: where the boundary sits (competence line, not identity line) and how it moves (on measured evidence, not under capability pressure). The S7M user asks "Is AI reliable enough at this specific task?" The S3B user asks "Does this task feel too important to delegate?"

S7M behavior in practice: the user delegates at high D-levels in their core domain when AI is reliable enough there, and refuses to delegate at low D-levels outside their core domain when AI is not reliable enough there. The identity engagement does not determine the choice; the quality of AI does.
```

### Why this matters

V5's distinguishing signal between S3B and S7M is the heuristic about boundary movement. That heuristic is fragile — it requires longitudinal observation across multiple model releases. Adding the *where the boundary sits* dimension gives practitioners a second observable that can be checked from a single conversation: ask the person which tasks they delegate and which they don't, and see whether the pattern aligns with their identity domain or with where AI is competent.

This makes the S3B vs S7M distinction more practically usable, even if it remains genuinely difficult to call from a snapshot.

### Open question

The two heuristics (where the boundary sits, how it moves) can disagree. Someone might draw the boundary at the identity line (looks like S3B) but move it only on evidence (looks like S7M). What is that? The model should acknowledge this as a transitional position — someone who has the identity-driven boundary but is in the process of rebuilding it on evidence. Add a short note in S5 Understanding noting that this is a typical transition shape from S3B to S7M.

---

## Verification checklist

- [ ] S2D Defensive Resistance file contains the per-domain scoping section.
- [ ] Identity Stakes axis description spells out per-domain explicitly.
- [ ] `Model6.md` reading guide notes that states are per-domain.
- [ ] S3B Bargaining file contains the two-axis distinction from S7M.
- [ ] S7M Maturity file contains the mirror reference.
- [ ] Transitional position (identity-line boundary moving on evidence) is noted in S5 Understanding.
