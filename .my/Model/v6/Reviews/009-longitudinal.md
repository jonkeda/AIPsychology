# 009-longitudinal.md

## TL;DR

- V6 explicitly declines to specify numerical transition probabilities, dwell times, or cycle frequencies. This is an honest epistemic choice and prevents fabricated numbers. But it leaves practitioners without answers to time-critical questions.
- Dwell time in S3E (Ego Shock, where the person confronts replaceability) is the foundational dynamics question. A practitioner cannot decide whether to intervene now, wait, or refer without knowing how long people typically stay there.
- Five dynamics questions would change how the model is used: S3E dwell time, S5 regression rate on capability jumps, S2T success split between S5 and S2D, time-to-burnout from S6E/S6R, and S3X stability over years. All five are testable with longitudinal panels.
- A minimum viable study to establish dwell times in S3E, S5, and S6E/S6R spans 18–24 months across two major model releases, ~150 knowledge workers tracked quarterly, ~80–120k budget. This is the first wedge into V7 numerics.

---

## Findings

### 1. V6 has no dwell-time estimates, making intervention timing impossible — not yet tested

V6 explicitly declines numerical dynamics. The `limits-of-operationalization.md` file lists "numerical transition probabilities and dwell times" under "Deliberately not in V6" with the justification: "adding fabricated numbers is worse than admitting they don't exist."

That is honest and correct. But the honesty creates a practitioner-facing problem.

When a practitioner observes someone in **S3E Ego Shock** (the state where the person confronts the fact that AI can replicate the skill their professional identity is built on), the model says:

- S3E is transitional only. Healthy as a passage; harmful as a residence. Sustained S3E without movement within weeks to months warrants attention.

But "weeks to months" is a gloss, not a number. A manager facing an employee in S3E cannot answer: "Do I give them two weeks to work through this, two months, or is this the start of a six-month crisis?" The model describes what happens *after* the person exits S3E (bargaining, direct integration, structural displacement). It does not describe *when* that exit happens.

Similarly, S3E is reachable as a regression from any later state. Without regression rates, a practitioner cannot estimate: "Of my team at S5 Understanding, what fraction will fall back to S3E after the next capability jump?" That is not an academic question. It determines whether S5 is a stable working state or a temporary platform before the next shock.

**Fix:** Commission an 18-month longitudinal panel across two model releases to establish dwell-time distributions for S3E, S5, and S6 states. Report medians, quartiles, and failure modes. See Recommendation 1.

---

### 2. S3E dwell time is the load-bearing question — testable

Among the five priority dynamics questions (listed in Prompt I), dwell time in S3E is first because it is decision-critical and highest-leverage.

S3E is also the most identity-intense state. A person who has not moved by month three is at risk of clinical distress. A person who has not moved by month six is likely in crisis. A practitioner needs:

- Median dwell time (e.g., "most people take 4–8 weeks to reach S3B or S5").
- Probability of non-exit via regression or dropout after X weeks (e.g., "15% of people in S3E for >6 weeks drop out emotionally").
- Correlation with Identity Stakes. High-stakes domains likely have longer dwell times; low-stakes domains faster exits.
- Triggers for extended S3E. Repeated capability jumps? Loss of domain boundaries? Peer comparisons?

The `observation-guide.md` file says practitioners should look for whether the person is "moving through S3E (transitioning toward S3B or S5 within weeks to months) or staying (identity disruption unresolved after six or more months)." That heuristic is reasonable. But it is based on qualitative observation, not data. A study can replace the hand-wavy range with an empirical distribution.

**Fix:** Make S3E dwell time the primary outcome of the first dynamics study. Oversample high-stakes domains (engineering, law, translation, creative writing) where the model predicts longer stays. Report stratified medians.

---

### 3. S5 "stability" cannot be claimed without regression rates — testable

V6 describes S5 Understanding as "the first stable state" and lists it as "sustainable" in the healthiness layer. But "stable" without dwell-time data is an assumption, not a finding.

S5 stability depends on what happens when the AI environment changes. The state graph shows S3E regression edges: "Regression is a property of every transition, not a destination. Any state in S5 through S7 can be pushed back to earlier states by changes in the AI environment."

The triggers are listed: capability changes, access changes, tooling shifts, workplace changes, personal experience. Capability changes are the most common. Without data, V6 cannot answer:

- What fraction of S5 people regress to S3E on a capability jump in their domain?
- How long does the regression last? Do they re-stabilize at S5, or drop out?
- Is S5 a stable state or a "stable until the next shock" state?

A practitioner redesigning their support program needs to know whether S5 is an end state or a platform that requires re-stabilization every 6–12 months (i.e., every model release).

**Fix:** Embed regression rates in the second-year analysis of the longitudinal panel. Track cohorts across at least two major AI capability releases. Report fraction regressing, dwell time in regression, and return-to-S5 rates.

---

### 4. The S2T (Trust Evaluation) fork outcome ratios are unmeasured — testable

V6 describes a critical fork after S1 Initial Encounter:

- **S2T Trust Evaluation** (low-stakes, non-defensive testing)
- **S2D Defensive Resistance** (high-stakes, protective stance)

S2T can convert to S2D if "testing reveals a capability that newly threatens identity in a way the person did not anticipate going in." But V6 has no data on:

- What fraction of S2T testers actually reach S5 Understanding (trust established)?
- What fraction convert to S2D (threat surfaces during testing)?
- What fraction drop out as "practical-flavoured" (fails quality/reliability standards)?
- How long is the S2T testing period?

These ratios matter because they determine triage urgency and intervention strategy. If 80% of S2T testers reach S5, then S2T is a functional evaluation period and the model can afford to be patient with them. If 40% convert to S2D and only 30% reach S5, then S2T is higher-risk than the model implies and needs earlier intervention gates.

**Fix:** Add S2T outcome tracking to the longitudinal panel. Follow cohorts for 8–12 weeks from first exposure and classify endpoint: S5, S2D, dropout (practical), dropout (emotional). Report proportions stratified by Identity Stakes.

---

### 5. S6E (Enthusiastic Overuse) and S6R (Driven Overuse) have no burnout timeline — testable

V6 describes **S6E Enthusiastic Overuse** as "dopamine-driven experimentation. The person is energised, productive, and uncritical" and says it is "healthy short-term, costly long-term" but does not specify how short or how long.

Similarly, **S6R Driven Overuse** is "productivity-pressure-driven" and "sustainable with cost only as long as external pressure does not exceed personal capacity. Past that point, S7B Burnout follows."

But without time-to-burnout data, neither the practitioner nor the person in these states knows what "short-term" and "only as long as" mean. Is S6E sustainable for four weeks? Four months? Four years?

The healthiness layer says: "The duration of healthy S6E before it becomes corrosive is qualitatively understood (weeks to months) but not numerically established." This is exactly the gap V7 needs to close.

Burnout is the observable endpoint: usage collapses, the person withdraws, affect becomes cynical or depleted. Time-to-burnout is the critical denominator for:

- Estimating the size of at-risk population at any moment.
- Designing intervention windows (e.g., "check in with high-volume users monthly to catch early burnout signals").
- Advising people on sustainability of their current pace.

**Fix:** Establish time-to-burnout distributions from S6E and S6R by tracking monthly usage volume and affect measures for people in these states. Report median time to exit (either S7B or S5 regression), failure modes, and correlation with Identity Stakes and Delegation Level.

---

### 6. S3X (Structural Displacement) stability is unmeasured — testable

V6 introduces **S3X Structural Displacement** as a distinct state, reached when "viable AI-collaborative work no longer exists in their domain." It is described as "a state reached when a person concludes — or is confronted with the reality — that their economic position is gone."

But the model does not specify:

- How long do people stay in S3X before reaching one of the three resolutions (occupational transition, exit from knowledge work, adversarial advocacy)?
- How stable is the S3X conclusion? Do people re-enter S3B Bargaining after months of S3X, finding new niches?
- What fraction reach each resolution?
- How long is occupational transition (S3X → new domain S0/S1)?

These matter because they determine whether S3X is a state or a label for "the model no longer applies." If most people in S3X transition within 6 months, S3X is a brief phase. If they stay for 2+ years, S3X is a stable long-term state and warrants deeper study.

The file says: "the three-resolution structure (transition, exit, advocacy) covers observed responses but has not been validated against a representative sample of displaced workers." This is honest but limits the model's utility for organizations supporting displaced workers.

**Fix:** Recruit a cohort of 40–60 people in documented S3X (role eliminated, clients no longer paying for human work, or person has concluded viability is gone). Follow for 18–24 months. Track which resolution they pursue, time to resolution, any returns to earlier states, and economic outcomes. Report stratified by domain, age, and access to reskilling resources.

---

### 7. Regression triggers and rates lack temporal specificity — testable

V6 lists regression triggers (capability changes, access changes, tooling shifts, workplace changes, personal experience) but provides no rate data. For example:

- "A junior colleague outperforming with AI re-triggers S3E from later states."

Does that mean a single observation of peer outperformance triggers S3E? Or sustained performance gap? Or visibility of the gap to one's manager? And what fraction of people actually regress versus rationalize?

Similarly, "A model release that overruns prior rebuttals" is a capability trigger, but V6 does not specify:

- Which types of capability jumps trigger regression? (e.g., a new modality in a domain the person had bounded, vs. incremental improvement in the same modality)
- Are there threshold effects? (e.g., regression happens only if the new capability exceeds prior calibration by >X%?)
- What is the regression rate for a typical capability jump? (e.g., "20% of S5 people regress on capability jump, 5% drop out, 75% stay")

Without these, practitioners cannot predict the impact of a model release or major feature launch on their user population.

**Fix:** Instrument the longitudinal panel to capture all trigger events (capability jumps, team changes, metrics rollouts, performance feedback) with specificity and quantify regression rates per trigger type. Use version tracking and release notes to measure capability jump magnitude. Report regression rates with confidence intervals.

---

### 8. The "most people cycle through the model more than once" claim is still unquantified — testable

V6 inherits from V5 the claim: "People cycle through the model more than once because the AI environment keeps changing, not because the person is unstable."

This is marked as **Conjecture** in the limits file: "'Most people cycle through the model more than once' remains qualitative. V6 makes no numerical claim about cycle frequency."

But practitioners and researchers need actual numbers:

- What is the average number of cycles per person over a 24-month window?
- Does cycle frequency correlate with domain volatility, role tenure, or Identity Stakes?
- Are certain people "chronic cyclers" (more than three cycles per year) and if so, what predicts that pattern?
- Does cycling increase burnout risk or is it orthogonal?

The model assumes cycling is the baseline expected behavior and not a sign of instability. Quantifying cycle frequency tests that assumption.

**Fix:** Compute cycle frequency for all panel cohorts. Define a cycle boundary using state-transition events (entering a new major state, regressing, exiting). Report mean, median, and distribution of cycles per person per year, stratified by domain and Identity Stakes.

---

## Minimum Viable Study: Establishing V7 Dynamics

### Scope

Establish dwell-time distributions and transition rates for S3E, S5, S6E/S6R, and S3X across one full 18–24-month window spanning two major model releases.

### Design

**Cohort:** 150 knowledge workers tracked from initial AI exposure or from current state (if already mid-model).

Stratify recruitment:

- High-stakes domains: 80 people (software engineering, medicine, law, creative writing, research, translation).
- Low-stakes domains: 70 people (business analysis, financial forecasting, customer support, administrative work).

Ensure representation across role levels (individual contributor, manager, senior) and tenure in domain (0–3 years exposure to AI in their domain).

**Tracking:**

- **Quarterly surveys:** state classification (self-reported + behavior markers from observation guide), usage volume, perceived sustainability, intention to continue, any major work changes.
- **Event logging:** capture all capability jumps (model releases, new features in their domain), workplace changes (team reorg, new manager, new metrics), and personal events (performance feedback, peer comparisons, burnout signals).
- **Usage telemetry (optional):** if accessible from tools (e.g., ChatGPT, Copilot, Claude), log monthly delegation levels and frequency, by user consent.

**Duration:** 18–24 months minimum, covering at least two major model releases (e.g., GPT-4 → GPT-4 Turbo, or Copilot feature expansion).

### Instruments

- **State classification:** trained raters apply `observation-guide.md` markers quarterly. Achieve inter-rater agreement >0.75 (Cohen's kappa).
- **Dwell-time calculation:** for each state transition, measure duration from entry to exit date.
- **Regression tracking:** flag all transitions to earlier states; record trigger event if identifiable.
- **Dropout scoring:** two-axis (practical 0–10, emotional 0–10) per `dropout.md` at exit.

### Primary outcomes

- Median dwell times (with IQR) for S3E, S5, S6E, S6R, and S3X stratified by Identity Stakes.
- Transition rates: S2T → S5, S2T → S2D, S2T → dropout, S5 → regression rates on capability jump, S6E/S6R → S7B, S3E → S3B vs S3E → S5.
- Cycle frequency per person per year.

### Cost estimate

- Recruitment & screeners: $8k
- Quarterly surveys, 150 people × 6–8 contacts: $20k (at ~$30/person/contact for incentives + admin)
- Rater training and inter-rater audits: $5k
- Telemetry integration (optional): $10–15k
- Analysis, reporting, validation: $15k
- Contingency (15%): $12k

**Total: ~80–120k over 24 months.**

### Risk mitigation

- Attrition: oversample by 20% at start; track dropouts as a subgroup.
- Rater drift: audit inter-rater agreement every quarter; re-train if drifts below 0.70.
- Self-report bias: cross-check survey states against telemetry and event logs where possible.
- Seasonality: capture seasonal patterns (e.g., burnout spikes before deadlines) in the full 24-month window.

---

## Recommendations (prioritized by impact and tractability)

### R1. Establish S3E dwell-time baseline (Year 1 of longitudinal study)

**Priority: Critical.** Dwell time in S3E determines intervention timing and referral decisions. This is the single highest-leverage dynamics question.

- Recruit 40–50 people entering S3E during the study window.
- Track weekly or bi-weekly state markers (identity-level questions vs. capability-level questions, affect stability, domain withdrawal).
- Compute median and quartile dwell times overall and stratified by Identity Stakes.
- Identify predictors of extended S3E (>12 weeks): age, domain, prior AI exposure, access to peer support, management awareness.
- Deliver: dwell-time distribution and a practitioner heuristic (e.g., "check in weekly if >2 weeks in S3E; refer if >8 weeks unresolved").

**Effort:** ~25k. Timeline: 18 months.

---

### R2. Quantify S2T outcome split and dwell time (concurrent with R1)

**Priority: High.** Triage decisions depend on knowing what fraction of S2T testers will successfully reach S5 vs. convert to S2D vs. drop out.

- Track all S2T entrants for 8–12 weeks to outcome classification.
- Measure dwell time in S2T (median ~4 weeks expected; validate or revise).
- Stratify outcomes by Identity Stakes and domain.
- Deliver: outcome proportions (e.g., "60% → S5, 25% → S2D, 15% → dropout") and dwell time by stratum.

**Effort:** ~10k. Timeline: concurrent with S3E work.

---

### R3. Measure time-to-burnout from S6E and S6R (Year 1)

**Priority: High.** This tells practitioners and people in S6 states whether their pace is sustainable.

- Recruit people explicitly in S6E or S6R (high usage, high energy or high pressure, respectively).
- Track monthly usage and burnout signals (withdrawal, cynicism, fatigue, decreased output quality) for 12+ months or until exit.
- Compute median time to S7B or dropout, with confidence intervals.
- Correlate with workplace metrics rollouts, release cycles, and personal workload peaks.
- Deliver: "typical S6E person burns out in 3–6 months; S6R in 2–4 months; here is how to recognize early warning signs."

**Effort:** ~15k. Timeline: 18 months (need full duration for S6R data).

---

### R4. Establish S5 regression rates on capability jumps (Year 1–2)

**Priority: High.** This validates or refutes whether S5 is genuinely "stable" or just a platform before the next shock.

- Identify capability jumps (model releases, new modalities or features in tracked domains) during the study window.
- For each jump, classify cohort members: stay in S5, regress to S3E, regress to earlier state, drop out.
- Compute regression rate and time-to-regression per capability jump.
- Stratify by type of capability jump (in-domain replication vs. new domain opened vs. edge-case improvement).
- Deliver: "regression rate on typical capability jump is X%; regression typically resolves within Y weeks" and conditional probabilities by jump type.

**Effort:** ~12k. Timeline: requires two major releases in study window.

---

### R5. Measure S3X stability and resolution pathways (Year 2)

**Priority: Medium.** Supports workers transitioning out of roles and organizations managing displacement.

- Recruit a separate cohort of 40–60 people in documented S3X (role being eliminated, clients no longer paying, or person has concluded viability is gone).
- Follow for 18–24 months or until resolution.
- Classify resolution: occupational transition (identify new domain), exit (leave knowledge work), advocacy (pursue regulatory or labor-protection activities).
- Measure time to resolution and intermediate states (e.g., does person cycle back to S3B mid-transition?).
- Deliver: "X% transition to adjacent domain within Y months; Z% exit; A% pursue advocacy" and predictors of each outcome (age, domain, access to reskilling, support network).

**Effort:** ~20k (separate cohort). Timeline: 18–24 months.

---

### R6. Build a V7 Dynamics Annex with numerical transition tables

**Priority: Medium.** After R1–R5 are complete, synthesize findings into a companion document to V6.

- Create transition-rate tables (rows: origin state, columns: destination state, entries: rates with confidence intervals).
- Add dwell-time medians and IQR ranges per state and per identity-stakes stratum.
- Include regression rates per trigger type (capability jump, workplace change, personal event, peer comparison).
- Provide practitioner-facing decision trees (e.g., "if in S3E >6 weeks, refer; if <2 weeks and moving toward S3B, monitor weekly").
- Publish as: `.my/Model/v7/Dynamics/01-transition-rates.md`, `.my/Model/v7/Dynamics/02-dwell-times.md`, `.my/Model/v7/Dynamics/03-practitioner-tools.md`.

**Effort:** ~8k (synthesis only, after data is in hand). Timeline: post-study.

---

### R7. Establish baseline inter-rater reliability on state classification (before main study)

**Priority: Critical for validity.** The observation-guide markers must be reliable before using them to classify 150+ people.

- Recruit 10–15 raters (practitioners, researchers, coaches who work with AI-adapting professionals).
- Use video clips, transcript excerpts, and behavioural vignettes from the `observation-guide.md`.
- Have each rater independently classify state and dwell-time assessment.
- Compute Cohen's kappa per state and per rater. Target >0.75 overall; retrain if <0.70.
- Publish the validated markers and rater training materials as part of V7.

**Effort:** ~5k. Timeline: 2–3 months, before main study launch.

---

## Glosses

- **S3E Ego Shock:** the state where the person confronts the fact that AI can replicate a skill central to their professional identity; characterized by identity-level questions ("what does this make me?") rather than capability-level questions.
- **S5 Understanding:** the first stable state, where the person has a working mental model of what AI is and isn't, knows where human judgment matters, and uses it pragmatically.
- **S2T Trust Evaluation:** non-defensive testing of AI on known problems, comparing outputs and evaluating reliability.
- **S2D Defensive Resistance:** high-stakes, protective stance where threat is perceived and the person tests defensively, looking for reasons not to trust.
- **S6E Enthusiastic Overuse:** dopamine-driven experimentation, energized, uncritical, routing everything through AI.
- **S6R Driven Overuse:** productivity-pressure-driven, common in high-performance cultures, using AI to chase ever-higher efficiency.
- **S7B Burnout:** withdrawal from AI use after a period of high engagement, temporary or permanent.
- **S3X Structural Displacement:** reached when the person concludes viable AI-collaborative work no longer exists in their domain; the problem is structural (no position to adapt to), not psychological.
- **Dwell time:** duration spent in a state before transitioning to another state.
- **Regression:** transition backward in the model (e.g., from S5 to S3E) triggered by environmental change.
- **Identity Stakes:** the degree to which a skill or domain is central to the person's professional self-concept.
- **Delegation Level (D1–D4):** how much cognitive authority the person hands to AI in a single interaction; D1 is information gathering, D4 is autonomous partnership.

---

## Signposts

Here is the chain of reasoning:

1. V6 is descriptive, not predictive, and explicitly excludes numerical dynamics. This is honest and prevents fabricated numbers.
2. But practitioners making intervention decisions cannot operate without timing estimates. "Weeks to months" is not actionable guidance.
3. Dwell times are the first-order dynamics needed: how long do people stay in each state? That question is testable with a longitudinal panel across model releases.
4. Five specific questions would change how the model is used: S3E dwell time (intervention timing), S5 regression rate (is it really stable?), S2T outcome split (triage decision), burnout timeline (sustainability), and S3X stability (is it a state or just a label?).
5. A minimum viable study requires 150 people tracked for 18–24 months, quarterly assessment, event logging, and ~80–120k budget. It is feasible and high-leverage.
6. The study should begin with inter-rater reliability on the observation-guide markers, then proceed to the main panel. V7 would then incorporate the numerical findings as a "Dynamics" annex alongside the descriptive V6 model.

---