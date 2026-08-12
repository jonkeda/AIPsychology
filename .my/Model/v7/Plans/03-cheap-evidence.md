# Cheap Evidence

What can be learned about the model without money, participants, or institutional access — and, equally important, what cannot.

The funded programme in [Design/20-testing.md](../Design/20-testing.md) remains the right programme. This document describes what is achievable in its absence, ordered by cost. Several of these studies are genuinely informative. None of them substitutes for the real thing, and the document is explicit about the difference at every point.

## The distinction that organises everything

Two questions are constantly conflated:

1. **Is the model internally coherent?** Are its positions distinguishable from one another, are its descriptions specific enough to apply consistently, does it contradict itself?
2. **Is the model true?** Do its positions correspond to anything real in people, and does it predict anything?

**Question 1 can be answered for free.** It requires no participants, because it is a question about the documents. It is also the question that most often has a bad answer, and answering it early can save all subsequent effort.

**Question 2 cannot be answered without participants, ground truth, and time.** Nothing in this document answers it. What the cheap studies can do is produce results that are *consistent or inconsistent* with the model being true — weak evidence, honestly labelled.

A model that fails Question 1 does not deserve Question 2.

---

# Tier 1 — Free, immediate, no participants

## C1. Blind discriminability of the position descriptions

**Cost:** an afternoon and a modest number of tokens.

**Question.** Can a reader who does not know which description is which tell the positions apart?

**Method.**

1. Write 40 to 60 short vignettes, each constructed to be an unambiguous instance of exactly one position. Write them from the position's entry conditions and observable signals, not from its name.
2. Strip all position names and codes from the model's descriptions.
3. Present a rater with the anonymised descriptions and one vignette at a time, and ask for a match plus a confidence rating.
4. Use several independent raters. Large language models are adequate here and cost almost nothing. Use more than one model family, in separate sessions with no shared context, so that agreement is not an artefact of a single system's habits.
5. Build a confusion matrix.

**What a good result looks like.** A strong diagonal, with confusions concentrated in the pairs the model already flags as hard — `OE` Open Evaluation against `GE` Guarded Evaluation, `SB` Scope Boundary against `IP` Integrated Practice: mastery.

**What a bad result means.** Systematic confusion between two positions is evidence they are one position. Diffuse confusion across many positions means the descriptions are not specific enough to apply, which is a writing problem before it is a theory problem.

**The honest limitation, stated plainly.** This tests whether the *documents* are internally separable. The vignettes were written from the model, so the model is being graded on its own material — a circularity that cannot be removed at this cost. A pass is weak evidence. **A fail is strong evidence**, because a model that cannot separate its own hand-written best cases will certainly not separate messy real ones. The asymmetry is what makes the study worth running.

**Why this is the first thing to do.** It is the only study that can invalidate the entire project before any effort is spent on publishing or building. It should be run with a genuine willingness to get a bad answer.

## C2. Adversarial self-critique

**Cost:** tokens.

**Question.** What are the strongest available objections to the model, and does it survive them?

**Method.** The V6 review corpus already demonstrates this works: assign a critic the role of a hostile specialist — an organisational psychologist, a measurement theorist, a labour economist, a practitioner who thinks the whole thing is repackaged common sense — and require a review that assumes the model is wrong and looks for the reason.

For V7, the reviews worth commissioning that V6 did not have:

| Reviewer role | Attack to invite |
| --- | --- |
| Measurement theorist | Are these constructs even the kind of thing that can be measured? Is the position graph a category error? |
| Occupational health specialist | Does `BO` Burnout as described conflict with the established burnout literature in a way that matters? |
| Labour economist | Is `SD` Structural Displacement doing psychological work that should be economic? |
| Practitioner sceptic | Which parts would change any decision, and which are decoration? |
| Agentic-workflow engineer | Is `OL` Oversight Load real, or an artefact of a badly designed pipeline? |

**Value.** High, and not only for the critique. Writing a defensible response to a strong objection is how the model's boundaries get found. The V6 adversarial response and its change plan were among the most productive documents in that version.

**Limitation.** Self-critique through a proxy is still self-critique. It finds internal inconsistency and missing literature. It cannot find the thing the author does not know they do not know. That requires readers, which is Track A of [01-way-forward.md](01-way-forward.md).

## C3. Literature reconciliation

**Cost:** time, plus search access.

**Question.** Has someone already described this, and does the existing work contradict it?

**Method.** For each position and axis, search systematically for prior work and record three outcomes: consistent, contradictory, or already-described. The last outcome is the valuable one — a position that duplicates an existing well-supported construct should be replaced by that construct and cited, not renamed.

**Areas where prior work is most likely to bite:**

- Technology acceptance and resistance research, for the entire Stance family.
- Occupational identity and identity threat, for the Disruption family.
- Burnout and job demands-resources research, for `BO` Burnout and for the Verification Burden axis.
- Automation research on complacency, trust calibration, and monitoring — this literature is decades old, developed for aviation and process control, and is directly relevant to `OL` Oversight Load and to `OU` Overuse: anxiety. It is the most likely source of *the model has reinvented something* findings.
- Cognitive offloading and skill retention, for the delegation axis.

**Why this ranks high despite being unglamorous.** Discovering that an established literature already contains a better-supported version of one of the model's constructs is a large gain: it removes an unvalidated element and replaces it with a validated one, at zero cost. Several of the model's weakest constructs may be repairable this way.

## C4. Internal consistency audit

**Cost:** time, or an agent.

**Question.** Does the model contradict itself?

**Method.** Mechanical checks across the document set: every position reachable, every edge appearing in both the graph and the relevant position descriptions, every attribute defined once, no claim marked as conjecture in one place and asserted in another, every falsifier actually falsifying its claim.

**Value.** Moderate but cheap, and it is the kind of error that damages credibility disproportionately. This is well suited to automation and should be a standing check rather than a one-off.

---

# Tier 2 — Cheap, requires people, small numbers

## C5. Think-aloud protocol testing

**Cost:** the goodwill of five to eight people.

**Question.** Do the interview questions elicit what they are supposed to elicit?

**Method.** Ask a small number of professionals to answer the interview questions while narrating what they are thinking. Record where a question is ambiguous, where it prompts a socially desirable answer, where it is heard as an accusation, and where the answer is fluent but empty.

**What it produces.** A better instrument. This is the single highest-value activity per participant in the whole plan, because instrument problems propagate into everything built later. Running the website in [06-website-platform.md](06-website-platform.md) on untested questions would be the most expensive possible way to discover the questions are bad.

**What it cannot produce.** Anything about the positions. This tests the questions, not the theory.

## C6. Case corpus from field use

**Cost:** zero marginal, if the model is being used anyway.

**Question.** Do real cases fit the positions?

**Method.** Every practitioner use — coaching conversation, team discussion, the author's own workplace — recorded in a fixed structured format: domain, stakes evidence, quoted responses, position assigned, confidence, and, critically, **whether the case fitted comfortably**.

**The field that matters most is the discomfort flag.** A corpus of comfortable fits proves nothing, because the model is expressive enough to describe anyone. A corpus that records where classification was forced identifies the gaps. Recording only successes converts the corpus from evidence into a testimonial.

**What it can support.** Base rate impressions, identification of positions that never occur in practice, discovery of patterns with no home in the graph. Positions that are never assigned in a substantial corpus are candidates for removal.

**What it cannot support.** Anything comparative or quantitative. The sample is whoever the author happened to talk to, the classifier is the author, and the author knows the hypotheses. This is the weakest possible evidential position short of making it up, and results should be described as illustrations rather than findings.

## C7. Two-rater agreement on real cases

**Cost:** one willing colleague.

**Question.** Do two people classify the same case the same way?

**Method.** The genuinely difficult constraint is independence. Both raters must work from the same evidence — a transcript or a structured record — without discussion, without seeing each other's judgement, and ideally without the second rater knowing the first rater's hypothesis about the case.

Even ten cases with two independent raters is informative, because the failure mode of interest is systematic rather than marginal. Disagreement concentrated on the `SB` Scope Boundary against `IP` Integrated Practice: mastery pair is a specific, actionable finding.

**A cheap augmentation.** Use a language model as a third rater working from the same transcript with the coding manual and no other context. Disagreement between the human and machine raters localises ambiguity in the manual, which improves the manual regardless of what it says about the model.

---

# Tier 3 — Free at scale, but heavily compromised

Everything in this tier becomes available if the website in [06-website-platform.md](06-website-platform.md) attracts users. It looks like the most valuable data in the plan and is in fact the most dangerous, because volume creates an appearance of rigour that the sampling does not support.

## C8. Item analysis

**Question.** Do the questionnaire items behave sensibly?

**What large-N self-selected data genuinely supports.** Response distributions, items nobody understands, items everybody answers identically, items that correlate with everything, completion and drop-off points, and internal consistency within each hypothesised construct.

**Why this is legitimate despite the sampling problem.** Item behaviour is a property of the instrument. An item that is uninterpretable is uninterpretable regardless of who answered it. This is real, usable evidence and it improves the instrument directly.

## C9. Structure recovery

**Question.** Does the position structure appear in the data on its own?

**Method.** Cluster or factor analysis on responses, run without imposing the model's structure, then compared against it.

**Why this is the most interesting cheap study available.** If people's answers naturally group into clusters resembling the model's positions, that is evidence the positions describe something — evidence that does not depend on anyone applying the model correctly, because the structure was not imposed.

**Why it is weaker than it appears.** The items were written from the model, so its structure is partly built into the input. A clean recovery is suggestive rather than confirmatory. A **failure** to recover the structure is the more informative outcome, and it should be reported if it happens.

## C10. Test-retest stability

**Question.** Does the same person get the same result twice?

**Method.** Invite return visits after an interval and compare, recording any intervening capability release, mandate, or tool change.

**Why this is worth the effort.** Instability without an intervening event is a reliability problem. Stability across a major capability release would contradict the model's regression claims. Both outcomes are informative, and the study needs nothing but a returning-user mechanism.

**The contamination that cannot be removed.** Anyone returning has been exposed to the model's framing. Their second response is partly a memory of their first.

## Constraints that apply to everything in Tier 3

- **The sample is self-selected** toward people interested enough in AI and psychology to complete a questionnaire about it. It generalises to nobody.
- **Everything is self-report,** and the positions the model most cares about — `OU` Overuse: anxiety, `OL` Oversight Load with rubber-stamping — are precisely the ones people cannot report accurately about themselves.
- **Every respondent has been exposed to the framing** by the act of answering.
- **Any published result must carry these constraints in the same breath as the finding,** not in a limitations section at the end that nobody reads.

---

# What remains impossible

Stated so that no cheap substitute is mistaken for these.

| Question | Why it stays out of reach |
| --- | --- |
| Do positions predict anything? | Requires longitudinal tracking with outcomes |
| Does verification burden predict burnout better than volume? | Requires workflow telemetry from an organisation |
| Does skill atrophy under sustained delegation? | Requires repeated blind-scored unaided performance testing over years |
| Does Identity Stakes predict the stance fork? | Requires sealed pre-measurement and controlled first exposure |
| Does any of it hold across cultures? | Requires samples large enough to separate culture from sector and role |

Each requires a collaborator with access the project does not have. That is the purpose of Phase 6 in [01-way-forward.md](01-way-forward.md), and it is the honest answer to why publishing early matters: **a published model with a working tool and a case corpus is a proposition someone might join. A private folder is not.**

# Recommended order

| Order | Study | Why here |
| --- | --- | --- |
| 1 | **C1** Blind discriminability | Can invalidate everything downstream. Free |
| 2 | **C3** Literature reconciliation | May replace weak constructs with validated ones before anything is published |
| 3 | **C2** Adversarial critique | Finds the objections before reviewers do |
| 4 | **C4** Consistency audit | Cheap, and errors here cost credibility disproportionately |
| 5 | **C5** Think-aloud testing | Fixes the instrument before it is built into anything |
| 6 | **C6** Case corpus | Begins with first use and compounds |
| 7 | **C7** Two-rater agreement | Needs the corpus and the manual |
| 8 | **C8–C10** | Only after the site exists and the items have survived C5 |

The first four cost nothing but time and tokens, and together they constitute a real programme of work. A model that has been through all four is in materially better shape than one that has not, and is worth publishing. That is the achievable standard.
