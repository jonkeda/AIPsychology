# Testing the Model

Ideas for turning V7 from a set of plausible descriptions into something that can be shown to be wrong. Nothing here has been run. The purpose is to specify what would count as evidence before anyone has a stake in the answer.

The governing principle: **a model that cannot fail is not describing anything.** Every study below is designed around a stated condition under which part of the model is discarded or collapsed.

## What has to be true before anything else is worth measuring

Three problems undermine every study in this area. They are stated first because a design that ignores them produces numbers that mean nothing.

### Problem 1 — Positions are unobservable

Positions are internal. Every measurement is a proxy, and the proxies vary enormously in quality. Any study design should state, per construct, which of these it is relying on:

| Access route | Reliable for | Unreliable for |
| --- | --- | --- |
| **Behavioural observation** | `NE` No Engagement, `FC` First Contact timing, `OU` Overuse presence, `OL` Oversight Load burden, `DX` Disengagement, delegation level of a specific interaction | Every driver, every style, `OE` Open Evaluation versus `GE` Guarded Evaluation, `SB` Scope Boundary versus `IP` Integrated Practice: mastery, Identity Stakes |
| **Interview** | Internal framing, reasoning behind a boundary, `VR` Values Refusal grounds, `SD` Structural Displacement framing, retrospective `IS` Identity Shock | `OU` Overuse: anxiety, `IS` Identity Shock during the episode, `OL` Oversight Load: rubber-stamping — all ego-threatening to report |
| **Workflow telemetry** | Volume, review-to-production ratio, domain distribution, revision and correction rates, session structure | Stakes, affect, reasoning, anything internal |
| **Structural facts** | Predicting stakes before observation: tenure, income share, public identity, mandate presence, peer adoption | Classifying a current position |

Structural facts are for **prediction before observation**, never for classification after it. That constraint is what keeps Identity Stakes falsifiable.

### Problem 2 — Contamination

Once a person knows the model, self-report becomes a performance of it. There is no statistical correction for demand characteristics of this size.

**Rules for every validation study:**

- Participants must be **model-naive**. This window closes as the model circulates, which is an argument for running the foundational studies early.
- Instruments must **describe behaviour and feeling, never name positions**. No item may contain a position name or code.
- Participants must never be asked to **self-classify**. They are asked what they did and what it felt like; raters do the classifying.
- Where the model must be explained — practitioner-facing work — the data is treated as practice evidence, not validation evidence.

### Problem 3 — Mandated environments contaminate behaviour, not just report

Where AI use is measured and enforced, usage volume stops being evidence of adoption and self-reported enthusiasm stops being evidence of enthusiasm. Any organisational study must record mandate status as a covariate, and results from mandated and non-mandated settings should not be pooled.

---

# Stage 1 — Can two people agree?

Nothing else matters until this is answered. It is also the cheapest work in the programme and the most likely to force a structural change.

## T1.1 — Inter-rater reliability on position classification

**Question.** Given the same evidence about the same person, do two trained raters assign the same position?

**Design.** Assemble 60–80 case vignettes from transcribed interviews with model-naive practitioners across several domains. Strip all self-classification language and all stated reasons for `SD` Structural Displacement versus `DX` Disengagement. Two raters, trained on the model, blind to each other, classify each case by domain. Compute Cohen's kappa overall and per position pair.

**The pairs that matter.** Overall agreement will be inflated by easy cases. Report these separately:

| Pair | Why it is hard | Threshold |
| --- | --- | --- |
| `OE` Open Evaluation vs `GE` Guarded Evaluation | Identical in a snapshot; only the updating pattern separates them | κ ≥ 0.6 or collapse per D-B3 |
| `SB` Scope Boundary vs `IP` Integrated Practice: mastery | Both are confident selective use | κ ≥ 0.6 or the distinction is unusable in practice |
| `VR` Values Refusal vs `GE` Guarded Evaluation: ethical-overlay | Same vocabulary, different grounds | κ ≥ 0.6 or demote `VR` Values Refusal per D-B4 |
| `SD` Structural Displacement vs `DX` Disengagement high-practical | Both are exits attributed to AI | κ ≥ 0.6 or demote `SD` Structural Displacement |
| `OU` Overuse drivers | Same behaviour, different motives | κ ≥ 0.5 per driver or drop the driver |

**Falsifier.** Any pair below 0.6 means the model asserts a distinction that cannot be made reliably. The correct response is to collapse the pair, not to retrain the raters until they agree — trained agreement on an unreliable distinction measures training, not the distinction.

**Why first.** Every study below assumes classification is possible. If it is not, they are all measuring noise.

## T1.2 — Vignette discrimination

**Question.** Do the model's descriptions actually pick out distinct patterns, or do practitioners find every description plausible for every case?

**Design.** Construct vignettes designed to be unambiguous instances of single positions. Present position descriptions with names and codes removed. Ask experienced practitioners to match. A model with genuinely distinct constructs produces a strong diagonal.

**Falsifier.** Systematic off-diagonal confusion between two positions is evidence they are one position, independent of what raters do with real cases.

**Value.** Cheap, fast, requires no participant recruitment, and can be run before anything else.

---

# Stage 2 — Do the axes measure anything?

## T2.1 — Identity Stakes as an independent predictor

**Question.** Does Identity Stakes, measured before any AI observation, predict the stance fork?

**Design.** This is the study that determines whether the model's central claim is falsifiable at all, so the ordering is the entire design.

1. Recruit practitioners with no substantive AI use in a target domain.
2. **Before any AI discussion**, assess Identity Stakes from structural indicators only: years in the domain, income share, training depth, public identity, and whether the person names the skill unprompted when describing their work. Record and seal.
3. Provide a standardised `FC` First Contact — the same task, the same tool, the same quality of output.
4. Observe and classify stance at 30 minutes, 30 days, 90 days.
5. Compare against the sealed stakes assessment.

**Prediction.** High stakes predicts `GE` Guarded Evaluation; low and moderate predict `OE` Open Evaluation.

**Falsifier.** No association means the model's primary modulating axis does not modulate the thing it was introduced to modulate. This would be the most damaging single result available and should be run early for exactly that reason.

**What makes it valid.** The sealing. Any stakes assessment made after the fork is observed is unusable, and a study that permits it has demonstrated nothing.

## T2.2 — Verification Burden versus usage volume as a burnout predictor

**Question.** Does verification burden predict `BO` Burnout better than raw usage volume?

**Design.** In organisations with instrumented workflows, compute per person over 6–12 months: review-time to production-time ratio, output volume received versus output volume plausibly reviewable at a stated standard, and total AI usage volume. Track burnout indicators — sustained withdrawal, sick leave, role change, validated burnout instrument. Compare predictive power.

**Prediction.** Burden at `exceeded` outperforms volume.

**Falsifier.** If volume predicts as well or better, `OL` Oversight Load is not carrying its weight and collapses into `OU` Overuse per D-A3.

**Why this is the most tractable study in the set.** It uses data organisations already have, requires no instrumenting of the person, and has a clean quantitative comparison. It is also the one most likely to produce a result an organisation acts on, which makes it the easiest to fund.

## T2.3 — Delegation Ceiling: domain-specific or tool-specific?

**Question.** Does a ceiling raised with one tool transfer to its replacement?

**Design.** Identify people whose primary tool was deprecated or substantially changed. Establish the pre-change ceiling from refusal events and stated limits. Measure the ceiling with the replacement tool at 2 weeks and 3 months.

**Prediction under the V7 conjecture.** Partial reset, with recovery over weeks, rather than full transfer.

**Falsifier.** Full immediate transfer means the ceiling is purely domain-specific and D-C5 resolves to the V6 definition.

## T2.4 — Does D5 differ qualitatively from D4?

**Question.** Is objective delegation a different experience or a more intense one?

**Design.** Within-subject. The same practitioners complete comparable high-stakes tasks at D3, D4, and D5. Measure after each: felt authorship, felt responsibility, ability to identify their own contribution, and affect. **Prediction:** authorship and contribution-identification drop discontinuously at D5 while responsibility does not — the separation that [03-axes.md](03-axes.md) claims is the new stressor.

**Falsifier.** A smooth gradient across D3–D5 on all measures means D5 is more of D4 and the axis does not need a fifth step.

---

# Stage 3 — Do the positions behave as described?

Each position carries one falsifiable claim. These are the studies for the claims that are tractable; the rest are recorded in the position files.

## T3.1 — The updating signature

**Question.** Does `OE` Open Evaluation update symmetrically and `GE` Guarded Evaluation asymmetrically?

**Design.** Classify participants at baseline. Run five standardised interactions with a fixed ratio of good and poor outputs — the same outputs for everyone, so the evidence is held constant. Capture the stated assessment after each, and the attribution for each outcome.

**Prediction.** `OE` Open Evaluation moves in both directions. `GE` Guarded Evaluation incorporates failures and attributes successes to prompting skill, task ease, or luck.

**Falsifier.** If `GE` Guarded Evaluation-classified participants update symmetrically at a substantial rate, the criterion does not separate the positions and they collapse.

**Why this design is strong.** Holding the evidence constant across participants removes the main confound — that people testing different things reasonably reach different conclusions.

## T3.2 — Driver removal for `OU` Overuse

**Question.** Is each `OU` Overuse driver actually sustaining the behaviour?

**Design.** For each driver, remove the sustaining condition for 30 days and measure usage change against a matched group with a different dominant driver.

| Driver | Removal | Prediction |
| --- | --- | --- |
| `efficiency` | Suspend throughput tracking | Substantial drop |
| `social` | Solo work with no visibility | Substantial drop |
| `mandate` | Lift the requirement | Immediate drop |
| `reward` | Flatten the reward schedule | Gradual drop |
| `anxiety` | Cannot be ethically removed — measure distress on brief unavailability instead | Distress disproportionate to task difficulty |

**Falsifier.** A driver whose removal changes nothing is not a driver and should be dropped from the attribute set.

**Ethical constraint.** The `anxiety` arm cannot use removal. Withdrawing a tool from someone whose self-trust has transferred to it is a harm, not a manipulation.

## T3.3 — Boundary basis for `SB` Scope Boundary

**Question.** Do scope boundaries track identity centrality or measured tool unreliability?

**Design.** Elicit boundaries from `SB` Scope Boundary-classified practitioners in their own words. Independently measure (a) the identity centrality of the protected sub-domain and (b) the tool's actual failure rate on it, benchmarked separately. Correlate.

**Prediction.** Boundaries correlate more strongly with centrality than with failure rate. `IP` Integrated Practice: mastery shows the reverse, which is the same study run on both groups and the cleanest available separation of the two.

**Falsifier.** A reversed correlation refutes the `SB` Scope Boundary characterisation directly.

## T3.4 — `VR` Values Refusal stability under threat removal

**Question.** Does values refusal persist when the identity threat is removed?

**Design.** Follow `VR` Values Refusal-classified practitioners who move into roles where AI does not compete with their core skill, through natural role change rather than assignment. Measure position at 6 and 12 months.

**Prediction under the V7 position.** The refusal persists.

**Falsifier.** Substantial resolution means the position was `GE` Guarded Evaluation with ethical language, and `VR` Values Refusal demotes to an attribute per D-B4.

## T3.5 — `SD` Structural Displacement versus `DX` Disengagement blind discrimination

**Question.** Is structural displacement distinguishable from severe disengagement without the person's stated reason?

**Design.** Recruit people who left a domain citing AI. Present raters with behavioural and situational evidence, stated reasons removed. Classify.

**Falsifier.** Agreement below 0.6, or reasons indistinguishable from high-practical `DX` Disengagement in most cases, demotes `SD` Structural Displacement.

---

# Stage 4 — Does the graph predict?

Longitudinal work. Expensive, slow, and only worth starting once Stages 1 and 2 have not refuted the foundations.

## T4.1 — Transition observation panel

**Design.** A cohort of 150–300 practitioners across several domains and all three cohort types, assessed at 3-month intervals for at least two years, with the assessment protocol from [30-practitioner-use.md](30-practitioner-use.md) and workflow telemetry where available. Capability releases, mandates, tool deprecations, and access changes recorded as dated `⚡` events.

**What it answers.**

- Which edges are actually taken, and which specified edges are never observed.
- Whether unspecified transitions occur — the most informative possible result, because an unmodelled edge is a hole in the graph.
- Whether regression follows `⚡` events on the claimed timescale.
- Dwell time distributions, which the model currently refuses to specify.
- Whether the multi-domain claim holds — whether people genuinely occupy different positions across domains, or whether positions correlate strongly within a person and the per-domain claim is overstated.

**The most valuable single output** is the list of specified-but-never-observed edges. Those are where the model is inventing.

## T4.2 — Regression after capability release

**Design.** Identify a major capability release in a specific domain in advance. Measure domain-specific self-efficacy and position in high-stakes and low-stakes practitioners at 2 weeks before, 2 weeks after, and 8 weeks after.

**Prediction.** High-stakes practitioners show measurable self-efficacy decline and elevated `IS` Identity Shock classification; low-stakes practitioners do not.

**Falsifier.** No differential effect means the `IS` Identity Shock mechanism anchor overstates what happens, and the position needs re-describing.

**Why this is feasible.** Releases are announced. The pre-registration writes itself, and the natural-experiment structure is stronger than anything achievable by assignment.

## T4.3 — The skill maintenance question

The model's largest open question, per D-E2.

**Question.** What happens to underlying capability under sustained D4/D5 delegation, on what timescale, and does it recover?

**Design.** Longitudinal, with a domain-specific unaided performance task administered at 6-month intervals — the person completes representative work without AI, scored by blind domain experts. Compare across delegation-level groups. Include a recovery arm in which sustained high-delegation participants work unaided for a defined period before re-testing.

**Why the model has no position.** Stating one without this data would be the model's most consequential overclaim, and the outcome is genuinely uncertain — practice effects, motivation effects, and the possibility that the relevant skill has changed rather than decayed all cut across the simple prediction.

**Design difficulty, stated honestly.** The confound is severe. People who delegate more may differ from those who delegate less in ways that predict performance independently. Within-subject designs with pre-delegation baselines are the only credible route, and they require identifying participants before they adopt.

## T4.4 — Cohort transfer

**Question.** Does the Working family transfer across cohorts while the Disruption family does not?

**Design.** Apply the full protocol across `pre-AI`, `concurrent`, and `AI-native` practitioners in comparable roles. Compare classification rates and rater confidence per family.

**Prediction.** `OU` Overuse, `OL` Oversight Load, `IP` Integrated Practice classify at comparable rates and confidence across cohorts. `IS` Identity Shock and `SB` Scope Boundary classify rarely, or with low confidence, in the `AI-native` group.

**Falsifier.** Comparable Disruption-family rates across cohorts means the family is not cohort-dependent and the scope claim in [01-model-v7.md](01-model-v7.md) is wrong.

---

# Instruments to build, in order

| Order | Instrument | Purpose | Precondition |
| --- | --- | --- | --- |
| 1 | **Structured interview protocol** | Consistent elicitation without naming positions | None |
| 2 | **Rater training pack and coding manual** | Makes T1.1 possible; forces every construct to be operationalised | Protocol exists |
| 3 | **Structural stakes pre-assessment** | Sealed, pre-observation stakes measurement for T2.1 | None |
| 4 | **Telemetry specification** | Defines review-to-production ratio, delegation level, and domain distribution from workflow data | None |
| 5 | **Behavioural indicator checklist** | Practitioner-facing; observation rather than inference | Rater manual |
| 6 | **Self-report questionnaire** | Scale. Deliberately last, per D-D3 | Reliability established |

The rater manual is the highest-value item, and not only for research. Writing it forces every construct to be stated in terms a second person can apply, which is the discipline the model most needs. Constructs that cannot survive that exercise should not be in the model.

---

# What cannot be tested

Stated so no one designs a study for it.

- **Whether a position is good for a person.** Outside the model's competence and outside the descriptive stance in D-B1.
- **Whether the graph is complete.** Absence of an observed transition is weak evidence. The panel can show which edges are used, not that no others exist.
- **Mechanism.** Every mechanism anchor is vocabulary. Testing whether self-efficacy collapse *causes* `IS` Identity Shock requires manipulating self-efficacy in people whose careers are at stake, which is not ethically available.
- **Cultural variability.** V6 carried an extensive cultural section with no data. It remains conjecture, and a study would need cross-cultural samples large enough to separate culture from domain, sector, and mandate status. Nothing smaller is worth running.
- **Long-run outcomes.** Whether any position leads anywhere over a career horizon. The timescale exceeds the stability of the technology being adapted to.

---

# A minimum credible programme

If only three studies are ever run:

1. **T1.1 — inter-rater reliability.** Without it, nothing else means anything.
2. **T2.1 — Identity Stakes as a sealed prior predictor.** The model's central claim, and its most damaging possible refutation.
3. **T2.2 — Verification Burden versus volume.** The most tractable, most fundable, and the fastest route to a result that changes practice.

Together these test whether the model can be applied consistently, whether its main axis predicts anything, and whether its newest construct earns its place. A model that passes all three is worth investing in. A model that fails T1.1 should be simplified until it passes.
