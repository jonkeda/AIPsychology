# Discussion 04 — Domains: Identification, Stakes, and Multi-Domain Reporting

Working notes. The model's most original claim is that a person is not in one state — they are in different states for different domains simultaneously. This document works through the practical questions that claim raises: how do you find a person's domains, how do you identify the high-stakes ones, what else matters about a domain, and how do you show a person's cross-domain picture.

---

## 1. What is a domain?

The model uses "domain" without defining it precisely. A working definition:

> A **domain** is a bounded area of professional skill in which a person has invested enough time to form expectations about their own competence, and in which AI is now capable of doing some or all of the same work.

That definition has four components:

- **Bounded** — it has a name and rough edges. "Writing" is a domain. "Long-form essay writing" is a sub-domain. "Knowledge work" is too broad to be a domain.
- **Professional skill** — the person has learned it deliberately. Hobbies can qualify if the person's identity is invested.
- **Invested time** — enough that the person has expectations about their own quality and speed. A week of dabbling does not qualify.
- **AI threat** — an AI system can now produce work that competes with what the person produces. No threat, no relevant stakes.

If a person works entirely in one domain (a specialist surgeon, a full-time copywriter), one domain analysis is sufficient. If their work spans multiple skill areas (a consultant who writes, facilitates, designs, and analyses), multiple domains are needed.

---

## 2. How to find a person's domains

### Step 1 — Work history scan

Ask: "Walk me through what you actually produce in a week." Focus on *outputs*, not job titles. A content strategist might produce: long-form articles, social posts, client briefs, slide decks, workshop facilitation. Each is a potential domain.

Useful probe questions:
- "What would you say is your core skill — the thing you are known for?"
- "What did you train in, formally or informally?"
- "What do you do that you think takes real expertise?"
- "What could you not have someone junior do instead of you five years ago?"

The last question is especially useful — it surfaces the things the person has built identity around, not just the things they happen to do.

### Step 2 — Consolidation

Raw output lists tend to be too granular (thirty-seven tasks) or too vague (two job descriptions). Consolidate by skill family:

- Group tasks that use the same underlying skill ("social posts" + "long-form articles" = writing).
- Split tasks where the skill is genuinely different ("data analysis" is not the same domain as "data storytelling" for someone whose identity is built around one but not the other).

Aim for two to six domains per person. More than six is hard to analyse; fewer than two risks missing the multi-domain dynamic.

### Step 3 — Verify with the person

Present the domain list back. Ask: "Does this feel like the right way to carve up what you do? Is there anything you'd split or merge?"

Verification also starts revealing stakes — people tend to correct domains they care about more carefully.

---

## 3. How to identify the high-stakes domains

After domains are listed, Identity Stakes needs to be assessed per domain — and, per the measurement note in `01-axes.md`, **before** observing which state the person is in.

### Indicators of high Identity Stakes

These can be assessed in interview or via a short self-report instrument:

| Indicator | Question | Signal |
|---|---|---|
| **Time invested** | "How many years have you been developing this skill?" | 10+ years = likely high stakes |
| **Training depth** | "Did you train formally in this? Degree, certification, apprenticeship?" | Formal training = stronger identity investment |
| **Income centrality** | "What proportion of your income depends on this skill?" | >50% = typically high stakes |
| **Identity claim** | "Is this how you introduce yourself professionally?" | Yes = high stakes |
| **Reputational exposure** | "Do others know you for this skill?" | Yes, especially if publicly — high stakes |
| **Substitutability anxiety** | "How would you feel if someone else did this part of your job instead?" | Discomfort without context = stakes present |

No single indicator is definitive. A person with ten years in a domain but who views it as "just a job" may have low stakes. A person with two years in a domain they have wrapped their entire identity around may have high stakes.

### The stakes scale

V6 uses a binary (high / low). A three-point scale is more practical:

| Level | Meaning |
|---|---|
| **Low** | Skill is incidental. Could stop doing it tomorrow without identity disruption. |
| **Moderate** | Skill matters professionally but is not the core of self-concept. Disruption would be uncomfortable, not destabilising. |
| **High** | Skill is central to professional identity. Disruption activates strong defensive or shock responses. |

Moderate is the useful middle ground that the binary misses — it predicts S2T rather than automatic S2D, and S3E if disruption occurs but at lower severity.

---

## 4. What else matters about a domain

### Delegation Ceiling per domain

The Delegation Ceiling (maximum AI involvement a person can accept) is also per-domain. A person may have:

- D4 (no ceiling) in low-stakes domains (scheduling, research summaries).
- D2 (task execution only) in moderate domains (client emails, presentations).
- D1 (information only) in high-stakes domains (their core craft).

The ceiling in the core domain is the diagnostic one — it tells you how much the person has actually integrated AI into their identity-central work, not just their peripheral work.

### Domain age

A newer domain tends to have lower stakes than an established one, even if the person is capable. Someone who has been a data analyst for twelve years and started facilitating workshops six months ago will almost certainly have higher stakes in analysis than facilitation, even if both are now in their job description.

Domain age is a rough proxy for stakes when the person has not self-reported clearly.

### Domain overlap / AI substitution degree

Domains vary in how directly AI threatens them. Some domains face near-total substitution (certain kinds of writing, basic code generation, image creation), others face partial substitution (strategy, facilitation, physical craft), others face minimal substitution (relationship-intensive work, novelty work).

Higher substitution degree amplifies the stakes — a high-stakes domain with high substitution is the most likely S3E entry. Low substitution softens even high-stakes domains: a surgeon whose domain is not currently automatable may have high identity stakes but low threat activation.

### Domain isolation vs. integration

Some people have one dominant domain and several peripheral ones. Others have several roughly equal domains. The configuration matters:

- **Single dominant domain:** the model applies primarily there. Peripheral domains can be ignored or noted as low-stakes comparators.
- **Multiple equal domains:** the person may be in genuinely different states across them, and the cross-domain picture is the main insight.
- **Compound domain** (where the person's identity is built on the combination, not on any single skill): the model may need to treat the compound as the unit. A "creative director" whose identity is the integration of writing + visual + strategy may not respond to AI threats to any single sub-skill in the same way as someone for whom one skill is the identity anchor.

---

## 5. Visualizing and reporting multi-domain state profiles

The model's most original claim is also its hardest to communicate: the same person is in different states for different domains at the same time. A single state label misrepresents them.

### The domain-state matrix

The simplest representation is a table:

| Domain | Stakes | Ceiling | Current State |
|---|---|---|---|
| Long-form writing | High | D2 | S3B Bargaining |
| Data analysis | High | D1 | S2D Defensive Resistance |
| Client facilitation | Moderate | D3 | S5 Understanding |
| Email / admin | Low | D4 | S6 Integration (Mastery) |
| Visual design | Low | D4 | S0 Baseline |

This is the baseline reporting format. It answers "where is this person?" for each domain in one view.

### The radar / spider chart

For a single person over time or across a team, a radar chart maps state position on an axis from "early / resistant" to "integrated". States would need an ordinal score (e.g. S0=0, S1=1, S2D/S2P=2, S3E=3, S3B=4, S4=5, S5=6, S6=7, S7B/S7X=-1) with one spoke per domain. The shape shows where integration is leading and where it is lagging.

Caution: the ordinal encoding implies earlier = worse, later = better. That is the descriptive-vs-prescriptive problem from Discussion 03. Use it only in explicitly prescriptive settings where the goal is integration.

### The timeline view (longitudinal)

For tracking a person across time, a swimlane chart works well:

- One horizontal lane per domain.
- State shown as a coloured segment per time period.
- State transitions shown as segment boundaries.
- Key events (capability releases, role changes, employer mandates) marked vertically.

This makes visible:
- That domains move at different speeds.
- Regression events — where an S6 domain returns to S3E after a capability jump.
- Plateau — where a domain has been in S3B for years with no movement.

### Team view

When applying the model to a team rather than an individual, a heat map works:

- Rows = team members.
- Columns = shared domains (the team's primary capabilities).
- Cell = state for that person in that domain.
- Color = integration level (early/resistant in red, integrated in green, terminal in grey).

This shows the team's profile at a glance: who the integration leaders are in each domain, where resistance is concentrated, and whether the team has any domain it has collectively not engaged with.

---

## 6. The measurement problem revisited

All of the above assumes domains can be identified and stakes assessed before states are observed. The adversarial review (004) correctly identified that post-hoc domain assessment is circular: you cannot declare a domain high-stakes because the person showed up in S2D there.

The practical protocol for practitioners:

1. Identify domains from work history before any state observation.
2. Assess stakes per domain from structural indicators (years, income, identity claim) before any state discussion.
3. Record domains and stakes.
4. *Then* observe or assess states per domain.

If stakes were assessed correctly before observation, the state profile is not circular. If this order is not followed, the stakes labels are post-hoc rationalisation and the multi-domain picture is not falsifiable.

This is the most important procedural point in working with the model in practice.

---

## Open questions

- **Sub-domains:** when does a domain need to be split? There is no principled answer yet. Current practice: split when the person has a meaningfully different identity investment in the parts. A writer who writes fiction and non-fiction may need them split; one who writes for different clients probably does not.
- **Compound domains:** how to handle identities built around a skill cluster rather than a single skill. Unresolved.
- **Domain obsolescence:** what happens when a domain stops being relevant (job change, retirement, total automation)? The model currently treats this as S7X entry. That needs verification.
- **Minimum domain count:** can the model apply to someone with a single domain? Yes, but the multi-domain insight is absent. The model reduces to a single-state snapshot.
