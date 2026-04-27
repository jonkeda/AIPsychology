This is a simpler rewrite of [006-practitioner-utility.md](006-practitioner-utility.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Practitioner Utility Review — Model V6 (Plain Language)

## TL;DR

- **Observation markers are half-baked:** The guide works for spotting some state pairs (S2T vs S2D, S3B vs S7M — explained in Finding 1 below). But separating PEN from S2D (two states that look identical in a single conversation) requires weeks of observation, not one meeting. You cannot diagnose fast enough to use this in most real interventions.
- **The psychology literature is vocabulary, not action:** The model says S3E Ego Shock connects to something called self-efficacy collapse. Knowing that label does not tell a manager what to say or do. It is a useful word. It is not a recipe.
- **The dropout reversibility test is clever but requires resources most workplaces do not have:** spare tools, management permission to run an experiment, and time to observe the result.
- **S3X is correctly out of scope:** The model honestly says "this is no longer a psychology problem." Fair. But practitioners are stuck with those people anyway and get no guidance on what to actually do.
- **The model tells you what not to do, but not what to do:** The manager-mistakes table is the most useful thing in V6. It is all negations. There are no prescriptions.
- **Multi-domain people are unhandled:** The model says the same person can be in different states in different areas on the same day. What do you do when you manage that person? Unspecified.
- **The "this is clinical distress" line is a guess:** Claiming that six-plus months in S3E equals clinical distress is plausible but untested. V6 should not state it as fact.
- **V6 works as shared vocabulary, not as a protocol:** If the goal is "my team and I use the same language," V6 delivers. If the goal is "I can diagnose someone and run an evidence-based intervention," V6 is not there yet. Both uses are legitimate. Only one is currently supported.

---

## Findings

### 1. The observation guide works for three state pairs; it fails entirely for PEN vs S2D

The observation markers in the guide are genuinely useful for two pairs:

- **S2T vs S2D** (someone evaluating AI with an open mind versus someone defending their competence by dismissing AI): ask whether they updated their view after seeing new evidence. S2T will have; S2D will not.
- **S3B vs S7M** (someone making a private deal to use AI for some things but not others versus someone in long-term stable maturity): ask which tasks they refuse to delegate. The S3B person names their identity domain; the S7M person names reliability concerns.

These signals work in a real conversation.

For the **S6 states** (four variants of heavy AI use — enthusiastic overuse, dependent overuse, driven-by-pressure overuse, and social overuse), the guide tells you to look at mood, drivers, and what would change the behaviour. A practitioner can probably get it right 60–70% of the time after a few conversations.

For **PEN vs S2D**, the guide explicitly says: "none reliable on a single observation." PEN (Pre-emptive Non-Adoption — someone who decided not to use AI before ever trying it, on values grounds) looks like S2D from the outside. The three signals that separate them — whether the objection applies across domains, whether evidence changes the position, and whether the emotional tone is moral conviction versus anxiety — all require watching the person over multiple weeks and multiple contexts.

In a one-off conversation with someone who says "I have values-based concerns about AI," you cannot reliably tell the difference between a genuine ethical stance and a threatened professional using ethical language as cover. The guide says most real cases are mixed — which is true and important — but that means the honest diagnosis is: "I need to watch this person for four to six weeks." For a manager who needs to know today whether to respect a boundary or address a threat, this does not help.

**Fix:** Reframe PEN diagnostics as longitudinal-only (meaning: they require time across multiple observations, not a single conversation). Remove PEN from any section of the guide that implies single-conversation diagnosis is possible. Add a separate section: "Signals that only emerge over weeks" with a clear timeline estimate of four to six weeks.

### 2. The related psychology literature is vocabulary, not action — knowing the name of a phenomenon does not tell a practitioner what to do

The model reframes its related literature as "vocabulary, not mechanism." For S3E Ego Shock (the panic and identity-threat state, grounded in ideas about self-efficacy collapse — the feeling that you are no longer good at your job — and terror management, which is the psychology of how people react when something threatens their sense of identity), S6E Enthusiastic Overuse (grounded in ideas about variable reward structures, where unpredictable positive results keep a behaviour going), and S7M Maturity (grounded in ideas about metacognitive calibration — knowing accurately what you know and do not know), the academic references are:

- Correct as descriptive frames.
- Readable for people with psychology training.
- Useless for a manager trying to figure out what to say in a one-to-one conversation.

A manager who learns that S3E Ego Shock involves self-efficacy collapse does not thereby know: should I reassure this person? Push them to try again? Give them a smaller task? Leave them alone? The literature anchor tells you what kind of phenomenon S3E is. It does not say how to respond to it.

The manager-mistakes table in the observation guide is more useful than all the related literature combined — it tells you what not to do. But the model has no "what to do" table, because it describes states rather than prescribing responses.

**Fix:** Acknowledge in the main model file that related literature is useful for cross-disciplinary communication and for future empirical grounding — not for practitioners in the moment. Add a note: "For action-focused practitioners, see the manager-mistakes table in the observation guide. V6 does not yet provide intervention protocols for what to do in each state."

### 3. The dropout reversibility test is conceptually clean but out of reach for most workplaces

The reversibility test is simple in principle: give someone who quit AI a tool that demonstrably solves the problem they cited. If they restart using AI, the practical barrier was the real driver. If they do not restart, the emotional driver was dominant.

In practice, running this requires:
- A tool that actually fixes the specific problem the person named. Not always available.
- Permission from leadership to run a test with one person and track the outcome. Rare in most organisations.
- Time to observe whether they restart. Days to weeks.
- A person willing to re-engage after they have already walked away. High friction.

Worse: the model admits that the 0–10 scoring axes (practical severity and emotional severity) have not been tested for consistency between practitioners. Two practitioners scoring the same dropout case could land in opposite corners and both claim the model supports their view. The test is labelled as testable. But the scoring underneath it is not validated. Without validated scoring, the test result can mean almost anything.

**Fix:** Add a section to the dropout file: "Operational constraints on the reversibility test." List the required resources, the time horizon, and the prerequisite scoring calibration. Mark the 0–10 axes explicitly as **Conjecture — scoring reliability not established**.

### 4. S3X Structural Displacement is correctly out of scope; the result is that practitioners have no handle on a real population

The model correctly identifies S3X Structural Displacement (a translator's market collapses because AI now does translation; a paralegal's document-review role is eliminated) as a structural and economic problem, not a psychological one. The identity crisis is real, but the root problem is economic: there is no viable adaptation within the domain because no viable role remains.

The observation markers — person describes the problem in economic terms, failed attempts to narrow the role to something AI cannot do, question shifted from "how do I adapt?" to "what work is left?" — are accurate and usable.

But then the model steps back. It correctly says: "this is no longer a psychology problem." Three possible transitions are named (moving to a new occupation, principled exit, adversarial advocacy against AI) but not developed. For a manager with an S3X person on their team, V6 offers clear diagnosis and no guidance. What do you actually do with this person? The model defers to labour protection and economic redistribution and says nothing about the person in front of you.

This honesty is correct. The model should not prescribe economic interventions it is not equipped to handle. But it is incomplete. A working tool for practitioners would either extend S3X guidance to include transition support, or describe somewhere what practitioners should do when they identify S3X.

**Fix:** Add a section to the usage file: "When you identify S3X Structural Displacement" with concrete referral pathways — career services, retraining programs, severance negotiation support, economic transition counseling. This does not make V6 prescriptive; it makes it complete by pointing practitioners toward the right domain experts.

### 5. PEN vs S2D collapses in real conversations — both states look the same from the outside until weeks of observation

This extends Finding 1 with more detail on why the collapse matters in practice.

PEN Pre-emptive Non-Adoption is a values-grounded refusal before ever testing the tool. S2D Defensive Resistance is identity-protection — refusing AI and dismissing evidence, because acknowledging AI's capability feels threatening.

The three distinguishing signals:
1. **Cross-domain consistency:** Does the objection apply even in domains where the person's professional identity is not at stake?
2. **Evidence response:** Does the position hold when the stated concern is demonstrably addressed?
3. **Emotional register:** Anxiety points toward S2D; moral conviction points toward PEN.

The model admits all three are unreliable in a single conversation. All three require four to six weeks of observation across multiple contexts.

A person who says "AI training data practices are exploitative and I won't use it" could be:
- **Genuine PEN:** a stable ethical stance applied consistently across domains, including low-stakes ones where identity is not at risk.
- **S2D with ethical language:** protecting competence, having learned that ethical framing sounds more defensible than admitting fear.

You find out by watching: does this person refuse AI for travel planning too? For recipes? If yes, it is probably PEN. If they happily use AI in low-stakes domains and wall it off only from their core work, it is probably S2D.

For a manager in a first conversation, this is not actionable. You have to guess. The cost of guessing wrong is high in both directions: treat it as PEN and you miss a threat that needs support; treat it as S2D and push back on the ethics, and you damage trust with someone who had a legitimate stance.

**Fix:** Reframe the PEN vs S2D section of the observation guide as explicitly longitudinal. Add: "First-conversation diagnosis is unreliable. Note the objection. Watch the next four weeks. Do not try to resolve this in the first conversation."

### 6. The model tells you what not to do by state, but not what to do — it is half an intervention framework

The manager-mistakes table is the most practically useful piece of V6:
- Do not skip S1 Initial Encounter and jump straight to a mandate.
- Do not argue with S2D Defensive Resistance's evidence; it hardens the position.
- Do not reassure someone in S3E Ego Shock; it feels dismissive.
- Do not reward output volume in S6E Enthusiastic Overuse.
- Do not make AI use publicly visible if someone is in S6S Social Overuse.

These are **negations.** They prevent the most common harm. The model does not provide what to do instead.

For S3E Ego Shock, the guide says: do not bring data, do not reassure, do not rush. What should you do? The model is silent. Presumably: sit with the person, acknowledge the threat, go slow, work on identity recovery. V6 does not say this, so practitioners infer it or make it up.

For S6D Dependent Overuse, the guide says: do not praise AI-augmented output without acknowledging the person's own contribution. What should you do? Presumably: rebuild independent confidence, give tasks where they have to rely on their own judgment, celebrate solo work. Again, inference required.

A working intervention framework needs both the negative (what stops harm) and the positive (what creates improvement). V6 provides the negative. Building the positive requires empirical testing or practitioner input that the model does not yet have.

**Fix:** In the usage file, add a section: "What V6 does not provide — the next layer." State explicitly: "V6 identifies states and tells practitioners what responses will worsen the situation. It does not yet provide prescriptive protocols for what to do in each state. Developing those requires empirical testing or practitioner input." Then list what a V7 intervention layer should address.

### 7. The model handles multi-domain people as a concept but provides no guidance for managing them in practice

V6 explicitly says: states are per-domain. The same person can be S2D Defensive Resistance about writing, S5 Understanding about email, and S7M Maturity about travel planning — all on the same day.

This is true and important. It correctly rejects the idea that a person has one single fixed state.

In practice, this creates a coordination problem the model does not address. Consider a manager with an employee who is:
- S2D about AI in their core domain (writes client case law).
- S5 Understanding about AI for research and document retrieval.
- S6E Enthusiastic Overuse of AI for routine coding tasks.

The model says the three states are independent. So the manager should apply S2D handling to writing, let S5 run freely, and watch for burnout in the S6E coding domain.

But these domains are not independent in real life. A confidence win in S6E coding might reduce the identity stakes in writing and push S2D toward S2T. An identity threat in writing might poison the confidence in the S5 and S6E domains. If the manager applies a different strategy in each domain, does that feel incoherent or manipulative to the employee?

The model has no answer to these questions. It correctly identifies that people are **multi-domain.** It does not address the cross-domain spillover — wins and setbacks in one domain bleeding into others — that happens with real people.

**Fix:** Add a section to the social context or usage file: "Multi-domain coordination and cross-domain transfer." Cover: how a confidence win in one domain can reduce identity stakes in another; how an identity threat in one domain can amplify defensiveness in others; and whether applying a consistent communication strategy across all domains (for coherence) is better or worse than tailoring to each domain (for optimality). The model does not need to answer these questions. It needs to name them.

### 8. The "clinical distress" boundary is a reasonable guess stated as a fact

The healthiness file maps states to a sustainability frame:
- **Sustainable:** S7M Maturity, S5 Understanding, S3B Bargaining.
- **Sustainable with cost:** S6E Enthusiastic, S6R Driven, S6S Social.
- **Transitional only:** S3E Ego Shock, S2T Trust Evaluation, S2D Defensive Resistance, S1 Initial Encounter.
- **Recovery:** S7B Burnout.
- **Corrosive:** S6D Dependent, sustained S2D.
- **Legitimate, not pathological:** S3X.

This is sensible. It avoids over-pathologising normal variation and correctly identifies that S3B and S7M are stable places, not end states to rush toward.

But the model states: "Sustained S3E (six-plus months unresolved) is within the range of clinical distress." This is plausible. Six months of identity threat with no progress is painful and can produce clinical symptoms. But the model has not tested this. V6 says it is descriptive and untested. Claiming a clinical threshold without testing it is a step toward pathologising people that V6 should not take without evidence.

Similar problem: "S6R and S6S are sustainable only as long as external pressure does not exceed personal capacity." True. But at what workload does S6R flip to unsustainable? The model does not say.

**Fix:** Rewrite the clinical statement in the healthiness file as **Conjecture:** sustained S3E beyond six months is plausibly within a range that matches clinical distress presentations, but this boundary has not been validated. Change "is within the range" to "is plausibly within the range." Apply the same change to any other healthiness claim that asserts a specific threshold.

### 9. V6 works as vocabulary, not as a protocol — the gap between the two is larger than the model acknowledges

The usage file lists what V6 can and cannot be used for.

**Can be used for:** recognition, shared vocabulary, intervention mapping (knowing what not to do), dropout triage, anticipating regression, organisation design conversations.

**Cannot be used for:** diagnosis (no validated test), prediction (no transition probabilities), quantitative measurement (scoring reliability not established), universal claims (untested), clinical therapy, performance management.

That second list is long. The gap between "shared vocabulary" and "working protocol" is wide.

If the goal is "my team and I use the same language for states" — V6 delivers. A manager can read it in a day, start using the terms in one-to-one conversations, and have clearer conversations. That is real value.

If the goal is "I can diagnose where someone is in under one conversation and plan an evidence-based intervention" — V6 does not deliver. The observation guide helps but does not eliminate uncertainty. The dropout axes are useful but not scored reliably. The intervention guidance tells you what not to do but not what to do. Multi-domain reality is acknowledged but not navigated. PEN vs S2D requires weeks.

The model acknowledges all of this. It is honest about what it does not know. But this honesty should lead practitioners to a clear conclusion: V6 is a **map**, not a protocol. Maps are useful. They orient you. They prevent catastrophic wrong turns. They are not enough to navigate by alone.

**Fix:** Reframe the header of the usage file: "What V6 is: A shared vocabulary and conceptual map." In the main text: "V6 is designed to help practitioners recognise patterns and avoid harm. It is not yet designed to support diagnosis or empirical intervention protocols. Until V6 has been tested and scored for reliability, treat it as a conversation tool and orientation guide — not as a diagnostic instrument."

---

## Recommendations

Listed in priority order:

1. **Reframe PEN diagnostics as longitudinal-only (Finding 5).** The current framing implies single-conversation diagnosis is possible; it is not. Add a clear four-to-six-week observation timeline. This prevents misdiagnosis in high-stakes situations.

2. **Add a "What V6 does not provide" section to the usage file (Finding 6).** Explicitly state that the model gives negations (what not to do) but not prescriptions (what to do). This prevents the frustration of reading the model and finding no intervention protocols.

3. **Add multi-domain coordination guidance to the social context or usage file (Finding 7).** Acknowledge cross-domain spillover. Raise the question of whether to apply a consistent strategy across domains. This prevents practitioners from treating state transitions as independent when managing real people.

4. **Revise the related-literature framing to make clear it is not intervention guidance (Finding 2).** Add: "For practitioners seeking intervention guidance, see the manager-mistakes table in the observation guide. Related literature is for cross-disciplinary communication and future empirical grounding, not for action in the moment."

5. **Revise the clinical boundary in the healthiness file from claim to conjecture (Finding 8).** Change "sustained S3E is within the range of clinical distress" to "sustained S3E is plausibly within the range of clinical distress — this boundary is untested."

6. **Add operational constraints to the dropout file for the reversibility test (Finding 3).** List resources required, time horizon, scoring prerequisites. Mark the 0–10 axes as **Conjecture — scoring reliability not established**.

7. **Add referral pathways to S3X guidance in the usage file (Finding 4).** Create a section "When you identify S3X Structural Displacement" with concrete next steps: career services, retraining budgets, economic transition counseling.

8. **Clarify in the main model file that V6 is a map, not a protocol (Finding 9).** In the "What kind of model this is" section, add: "This is a conceptual map and shared vocabulary. Until it is tested and scored for reliability, it is not a diagnostic instrument or treatment protocol. Use it to recognise patterns and avoid harm. Use it for conversation. Do not use it alone to diagnose or plan interventions."
