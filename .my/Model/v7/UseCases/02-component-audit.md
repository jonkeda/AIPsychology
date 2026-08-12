# Component Audit

Every part of the model, assessed on what it contributes and what it risks. This is the document that carries the argument.

Each component is scored on four dimensions:

- **Utility** — does it change a decision?
- **Novelty** — is it available elsewhere? (Detail in [03-prior-art.md](03-prior-art.md))
- **Robustness** — how badly does it fail if the model turns out to be wrong?
- **Risk** — what harm does it enable?

## Summary

| Component | Utility | Novelty | Robustness | Risk | Verdict |
| --- | --- | --- | --- | --- | --- |
| **Domain-specificity** | High | Low–Moderate | High | Low | **Keep. Lead with it** |
| **Verification burden** | High | Very low | High | Low | **Keep. Ground in prior work** |
| **Delegation levels D1–D5** | High | Very low | High | Low | **Keep. Ground in prior work** |
| **Identity stakes** | Moderate–High | Moderate | Moderate | Low | **Keep** |
| **Delegation ceiling** | Moderate | Moderate | Moderate | Low | **Keep, as part of stakes** |
| **The prohibition set** | High | Moderate | High | Negative risk | **Keep. Under-recognised** |
| **Coerced calibration** | Moderate–High | Low | Moderate | Low | **Keep** |
| **Open vs guarded evaluation** | Moderate | Low | Low | Moderate | **Keep as vocabulary only** |
| **Identity shock** | Moderate | Low | Moderate | Moderate | **Keep as vocabulary only** |
| **Scope boundary** | Moderate | Low | Low | Moderate | **Keep as vocabulary only** |
| **Oversight load as a position** | Low | Very low | Low | Low | **Fold into the axis** |
| **Overuse drivers** | Low–Moderate | Low | Low | Moderate | **Demote to a checklist** |
| **Integration styles** | Low | Low | Low | Moderate | **Cut** |
| **The transition graph** | Low | Moderate | Very low | High | **Demote to background** |
| **Position classification** | Negative | — | Very low | Very high | **Cut** |
| **Cultural variability** | Very low | Low | Very low | Moderate | **Cut** |
| **Advocacy overlay** | Very low | Low | Low | Low | **Cut** |
| **Cohort property** | Low | Low | Low | Moderate | **Cut for now** |

Four components in the top block carry most of the value. Everything from *oversight load as a position* downward is either better expressed another way or actively harmful.

---

# The components that earn their place

## Domain-specificity

**The claim.** A person does not have one relationship with AI. They have several, one per area of their work, and the areas can be very far apart.

**Why it is the strongest thing in the model.** It changes a conversation immediately and at almost no cost. The default organisational framing — adopter or resister, enthusiastic or reluctant — is not merely imprecise, it is wrong about most people most of the time. Replacing "she is against AI" with "she is guarded about illustration and fluent about everything else" alters what happens next.

**Counterfactual.** Some people arrive here on their own. Many do not, and organisations almost never do, because organisational instruments are built to produce one score per person. The framing is genuinely under-applied relative to how obvious it is once stated.

**Robustness.** Very high. This claim survives even if every position in the model is wrong. It commits to almost no theory.

**Risk.** Minimal. The worst outcome is a slightly longer conversation.

**Verdict: this is the model's headline. It should lead every article, every explanation, and the model itself.**

## Verification burden

**The claim.** When output arrives faster than it can be checked, verification becomes the work and then stops being possible, forcing a choice between approving unchecked work, refusing volume, or quietly lowering the standard.

**Why it matters now.** It names something people are currently living through without a name for it, and it points at a fix that is organisational rather than personal. It is also the most measurable construct in the model — review-to-production ratio comes out of ordinary workflow data with no psychological assessment at all.

**The prior-art problem, which is severe and turns out to be an opportunity.** This is not new. It is close to a restatement of Bainbridge's *Ironies of Automation* — automating production leaves people monitoring, humans monitor badly, and the skills needed to intervene decay through disuse. That analysis is from 1983 and has four decades of supporting work behind it in aviation, process control, and more recently vehicle automation.

**Why that is good news.** A construct with forty years of evidence is worth far more than an invented one. Reframing this component as *the ironies of automation, arriving in knowledge work* converts the model's newest and least supported idea into its best supported one, at zero cost. See [03-prior-art.md](03-prior-art.md).

**Verdict: keep, ground in the automation literature, and stop presenting it as new.**

## Delegation levels D1–D5

**The claim.** How much cognitive authority is handed over in a single interaction, from information retrieval through to unobserved autonomous execution.

**Why it works.** It is concrete, immediately usable, and requires no belief in anything else in the model. It gives people a way to be precise about something they currently discuss vaguely. The D4-to-D5 distinction — whether the person watched the work happen — is a real line and it lands with anyone who has used an autonomous agent.

**The cost alignment is a genuine find.** Delegation level correlates closely with token cost. Choosing the level deliberately is simultaneously the psychological discipline and the economic one. That is a useful, non-obvious, immediately actionable observation and it belongs in the model's front matter rather than buried in a plans document.

**Prior art.** Levels-of-automation scales have existed since the late 1970s and are well developed. The model's version is an application to generative AI, not an invention. It should say so.

**Verdict: keep. Cite the lineage. Emphasise the cost alignment, which is the genuinely current contribution.**

## Identity stakes

**The claim.** How central the affected skill is to professional self-concept determines how intensely the whole situation is experienced.

**Why it earns its place.** It is the model's actual explanatory idea — the thing that distinguishes it from a technology adoption framework. It explains why the same tool produces indifference in one domain and distress in another for the same person, which adoption models cannot.

**The weakness.** It is hard to measure without circularity, and the model knows it. The measurement-independence rule is the right response and it is demanding enough that it will frequently be skipped in practice.

**Verdict: keep. It is the theoretical core. Combined with domain-specificity it constitutes the model's genuine contribution.**

## The prohibition set

**The claim.** Do not track individual AI usage. Do not mandate a delegation level. Do not put any of this in a performance process. Do not assess employees with an untested framework.

**Why this is undervalued.** It is filed as a caveat and is in fact one of the most useful things the model produces. Organisations are actively doing these things now, at cost, and the model supplies a reasoned argument against each — including a self-interested one, since tracking individual usage destroys the organisation's own ability to tell whether its investment is working.

**Robustness.** High. The prohibitions hold even if the model is wrong, because they follow from the model being *unproven* rather than from it being correct.

**Verdict: keep, and promote it from caveat to deliverable. For an HR audience this may be the most valuable single output.**

## Coerced calibration

**The claim.** Forcing delegation above what someone accepts produces compliance that looks like adoption and resurfaces later as disengagement, quality problems, or exit.

**Why it earns its place.** It explains a specific, expensive, recognisable failure — the rollout that succeeds and then unravels — and it does so in advance rather than in hindsight. It also implies a concrete design rule: mandate exposure, not delegation level.

**Prior art.** Compliance-versus-commitment is well established in organisational change research. The contribution is the application and the ceiling mechanism, not the observation.

**Verdict: keep. High practical utility, moderate originality.**

---

# The components that survive only as vocabulary

These describe recognisable patterns and are useful as words. None of them supports classifying a person, and each carries some risk of being used that way.

## Open versus guarded evaluation

**Value as vocabulary.** Real. Distinguishing a person carefully evaluating a genuine threat from a person refusing to engage is worth doing, and the asymmetric-updating description gives it teeth. Reframing "resistance" as something other than obstruction is a genuine improvement on the prevailing organisational vocabulary.

**Value as diagnosis.** Near zero. The model concedes the two are indistinguishable in a single conversation and require repeated observation. Almost no practitioner will do repeated structured observation. In practice this means the distinction will be applied on insufficient evidence every time it is used.

**Risk.** Moderate. "He is in guarded evaluation" is exactly the kind of label that hardens into a fact about a person.

**Verdict: keep the description, drop the codes, never claim to identify which one someone is in.**

## Identity shock

**Value.** The naming has genuine worth, and this is the one place where naming alone does real work. A person experiencing an abrupt collapse in the felt value of accumulated skill usually cannot label it, and often interprets it as a personal failing. Being told that this is a recognised, describable, temporary response is a real intervention — normalisation is a genuine mechanism, not a placebo.

**Prior art.** Identity threat under occupational disruption is a developed literature. The model's version is an application.

**Risk.** Moderate. Amateur application to genuine distress. The referral guidance exists and needs to be prominent rather than parenthetical.

**Verdict: keep as vocabulary, with the clinical boundary stated firmly.**

## Scope boundary

**Value.** The reframing is the useful part: a person who has drawn a firm line about where AI is permitted in their work is not failing to adapt, they are occupying a stable and frequently sensible position. That reframing is worth having in an organisational context where any limit is read as resistance.

**Weakness.** Its diagnostic partner — distinguishing an identity-drawn boundary from a competence-drawn one — is the model's hardest judgement and is unlikely to be made reliably by anyone.

**Verdict: keep the reframing, abandon the distinction as a practical tool.**

---

# The components that should go

## Oversight load as a separate position

The phenomenon is real and important. Making it a *position* rather than a level of the verification burden axis adds a node, adds a set of transition claims, and adds nothing a practitioner uses. The axis already carries the information, and the axis is measurable while the position is not.

**Verdict: fold into the axis. This was the right call to flag as a decision, and the decision should go the other way.**

## Overuse drivers

As a checklist of reasons someone might be using AI more than their judgement supports — reward, anxiety, throughput pressure, social visibility, mandate — this is a reasonable prompt for a conversation.

As five sub-states with distinguishing diagnostics, it is unsupportable. The model concedes that the driver is invisible in behaviour and that the most consequential driver, anxiety, is the one people are least able to report. A distinction that cannot be observed and cannot be self-reported is not a distinction anyone can use.

**Verdict: demote to a discussion checklist. Remove the diagnostic apparatus.**

## Integration styles

Three styles that the model itself says routinely co-occur in the same person, distinguished by observations requiring twelve-month follow-up. Nothing acts on this.

**Verdict: cut.**

## The transition graph

This is the hardest call, because the graph is the model's structural centrepiece and represents most of the effort.

**What it contributes.** A defensible claim that positions are re-enterable and that regression is normal rather than a failure. That claim is worth making and it does not need thirty specified edges to make it.

**What it costs.** Every edge is an unvalidated empirical claim. The graph invites forecasting — *she is here, so she will go there* — which the model explicitly disclaims and the diagram implicitly promises. The V6 experience with ordinal numbering demonstrated that notation defeats disclaimers, and a directed graph promises trajectory in exactly the same way that numbering promised order.

**Counterfactual.** No scenario in [04-individuals.md](04-individuals.md) through [07-coaches-and-clinicians.md](07-coaches-and-clinicians.md) required the graph. Every one was resolved by the axes and the vocabulary.

**Verdict: demote to background material. Retain the re-entrance and regression claims as prose. Remove the diagram from anything practitioner-facing.**

This is uncomfortable, because the graph is where the work went. It is also the clearest instance in the audit of effort not tracking value.

## Position classification

**Verdict: cut entirely.**

This is the only component with negative utility. It is unsupported, it is the mechanism by which every identified harm occurs, and no scenario in the audit needed it. The assessment agent design in [Plans/05-assessment-agents.md](../Plans/05-assessment-agents.md) is methodologically careful and is careful about something that should not be built yet.

Its research value — generating agreement data as a byproduct — is real but depends on a corpus that does not exist and a user base that does not exist. It is an answer to a problem the project does not have.

## Cultural variability, the advocacy overlay, the cohort property

All three are conjecture with no supporting observation, and none appears in any scenario. They make the model look comprehensive, which is the opposite of what it needs.

**Verdict: cut. Record as open questions rather than model content.**

---

# What this leaves

Stripped to what survives:

**Two framing ideas.** Relationships with AI are per-domain. Identity stakes determine intensity.

**Two measurable conditions.** Delegation level, which is also the cost lever. Verification burden, which is the early warning.

**A small vocabulary.** Guarded evaluation. Identity shock. Scope boundary. Coerced calibration. Overuse.

**A prohibition set.** What not to measure, what not to mandate, what not to record.

That is a short document. It is perhaps a tenth of the current model, and it is very likely more useful than the whole, because it can be read, retained, and applied by someone who is not its author.

**The uncomfortable conclusion is that the full model was necessary to find this and is not necessary to deliver it.** The work was not wasted — the distillate could not have been written first — but continuing to elaborate the parts that did not survive would be.
