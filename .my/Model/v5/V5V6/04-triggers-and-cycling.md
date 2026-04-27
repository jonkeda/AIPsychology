# Slice 04 — Triggers and Cycling

Covers source items **7** (⚡ on S3B overstated), **8** (cycling has multiple causes), and **9** (drop "stable evangelists were once shaken" as fact).

## Item 7 — Drop "primary" from S3B Bargaining ⚡ marker

### What the source asks for

V5 reads:

> ⚡ Primary destabilizer: model releases.

The word "primary" overclaims. Model releases accelerate movement out of S3B Bargaining; they are not the only or always-primary cause.

### Concrete change

In `states/S3B-bargaining.md`, change:

- From: `⚡ Primary destabilizer: model releases.`
- To: `⚡ Accelerated by: model releases. Other accelerators include capability demonstrations from peers, internal evidence that AI now handles cases the bargain had excluded, and changes in workplace expectations. Model releases are the most visible accelerator but not the only one.`

The marker stays — the rule from the reviews instruction file says ⚡ applies if any named external event materially changes the probability of the transition. Model releases qualify. The "primary" claim is what gets dropped.

---

## Item 8 — Cycling has multiple drivers, not just new models

### What the source asks for

V5 says people cycle through the model more than once. It implies new model releases are the main reason. The source asks to broaden this: changes in cost, tooling, access, organizational expectations, and other AI-environment shifts can also push someone back through the cycle.

### Concrete change

In `Model6.md` or wherever the "Regression and Cycling" section lives, replace:

- From: *"Most people cycle through the model more than once as AI evolves."*
- To:

```markdown
## Regression and cycling

Regression is a property of every transition, not a destination. Any state in S5 Understanding through S7 can be pushed back to earlier states by changes in the AI environment. The triggers vary:

- **Capability changes.** A new model release that breaks the person's mental model. A capability jump in a domain the person had bounded. A high-profile AI failure that re-validates earlier fears.
- **Access and cost changes.** A price increase that makes the tools the person relied on unaffordable. Loss of access (the org pulls a tool, the API is deprecated, the seat is reassigned). A new tool the person cannot afford to evaluate.
- **Tooling shifts.** Better tooling that makes a previously closed domain feel newly relevant. Worse tooling that makes a previously stable workflow break.
- **Workplace changes.** New mandates, new managers, new peer groups, new performance metrics that change which AI uses are visible or rewarded.
- **Personal experience.** Being outperformed by a peer using AI. A failure that was caused by AI use the person had been confident in.

People cycle through the model more than once because the AI environment keeps changing, not because the person is unstable. Cycling is the model's expected behavior, not a deviation.
```

This widens the cycling claim to match how AI adoption actually plays out — capability is one axis among several.

### Open question

Item 8 in the source includes the bullet "no access to better tooling" — the case where someone *would* be in a higher state if they had access but is held back by cost or organizational decisions. This is worth flagging as its own pattern: a person trapped in S2D Defensive Resistance or S3B Bargaining not for psychological reasons but because they cannot afford or access the tools that would let them progress. Add a short note in `populations.md` (slice 06) covering this.

---

## Item 9 — Drop "stable evangelists were once shaken" as fact

### What the source asks for

V5 says:

> Most stable when the person has previously passed through S3E [Ego Shock]. Lived experience of Ego Shock is what makes them credible to others currently in it; without that experience, the advocacy tends to be naive (S6E flavor) or compelled (S6S flavor) and collapses under the first hostile question.

The source asks to remove this as a factual claim. Lived S3E experience is *one* trigger for stable S7V Evangelism, but other triggers exist (deep interest, generativity drive, professional role, organisational appointment). The model should not state the S3E prerequisite as fact.

### Concrete change

In `states/S7V-evangelism.md`, replace the prerequisite claim with:

```markdown
## Origins of stable S7V Evangelism

People reach stable S7V Evangelism through multiple paths:

- **Through S3E Ego Shock.** Lived experience of identity disruption is one common origin. People who have been through Ego Shock often become credible guides for others currently in it.
- **Through S7I Identity Expansion.** People who have built a new generative identity around AI sometimes channel that into helping others build theirs.
- **Through professional role.** Educators, consultants, and team leads can occupy stable S7V because the role demands it, with or without prior S3E experience.
- **Through generativity drive.** Some people are oriented toward helping others develop in any domain they themselves have worked through, and AI is just the latest instance.

The S3E Ego Shock path is *one* origin, not the only origin. V5 implied otherwise; that claim is downgraded in V6 to: stable S7V is *more common* among people with prior S3E experience, but stable S7V without prior S3E also exists.

A claim that V6 still makes: S7V Evangelism that is **only** S6E Enthusiastic Overuse flavor (uncritical promotion without any depth of prior engagement) tends to collapse under hostile questioning. This is about the depth of engagement, not specifically about S3E.
```

### Why this matters

The original V5 phrasing turned a useful observation (people who have been shaken make better guides) into a near-certainty (stable evangelists were once shaken). The source review work flagged this as overclaiming. The V6 rewrite keeps the useful observation as a tendency and removes the load-bearing claim.

### Knock-on effect on testability

V5's `limits-of-operationalization.md` listed *"The S7V-without-S3E collapse claim"* as currently conjecture. After this change, the claim is no longer made in this form. Update the limits document to reflect the softened version: the testable claim becomes "S7V Evangelism without depth-of-engagement collapses under hostile questioning," which is observable across multiple speaking events but is a different and weaker claim than the V5 version.

---

## Verification checklist

- [ ] S3B Bargaining ⚡ no longer says "primary."
- [ ] Cycling section lists capability, access/cost, tooling, workplace, personal experience as drivers.
- [ ] S7V Evangelism description lists multiple origins, not just S3E.
- [ ] Limits-of-operationalization document reflects the softened S7V claim.
- [ ] No remaining "stable evangelists were once shaken" wording.
