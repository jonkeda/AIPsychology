# Manager and HR Guide

How people with organisational authority can use the model. This is a different problem from practitioner use, because a manager or HR professional cannot have a purely observational relationship with an employee. Everything they learn sits next to a power asymmetry, and the model has no safeguards of its own.

[Design/30-practitioner-use.md](../Design/30-practitioner-use.md) covers technique. This document covers the constraints that apply when the person using the model can affect the other person's employment.

## The core problem

The model produces something that looks like an assessment of an individual. Organisations are built to act on assessments of individuals. Nothing in the model prevents its output being routed into a performance system, and every organisational instinct pushes in that direction.

That routing must not happen, for three separate reasons that each independently prohibit it:

1. **The model is unvalidated.** Employment decisions based on an untested psychological framework are indefensible if challenged, and they should be.
2. **The constructs are not performance constructs.** No position in the model describes how well someone does their job. A person in `GE` Guarded Evaluation may be the most careful reviewer on the team. A person in `IP` Integrated Practice: mastery may produce mediocre work efficiently.
3. **Measurement destroys the signal.** The moment a position affects reward, people learn which positions are rewarded and report those. The model stops describing anything, including for the honest uses.

The third reason is the one that persuades organisations, because it is a self-interest argument rather than an ethical one. It is also true.

## The separation rule

**Development and evaluation must never share a data path.**

| Development context | Evaluation context |
| --- | --- |
| Voluntary | Mandatory |
| Confidential to the participant | Recorded |
| Aggregated before it leaves the room | Attributed to individuals |
| Purpose is understanding | Purpose is decision |
| Model may be used | Model must not be used |

Where a single person occupies both roles — as most line managers do — the separation must be temporal and explicit, and the burden of making it credible falls on the manager. In practice this means a manager who has a genuine evaluative relationship with someone should be cautious about running a structured assessment at all, and should default to using the model to shape their own thinking rather than to produce an output.

**The safest managerial use of the model is one that produces no record.**

## What a manager can legitimately do

### Use it on the situation, not the person

The model's most defensible managerial application inverts the usual direction. Rather than asking what position each team member is in, ask what the environment is producing.

| Observation | Question it should prompt |
| --- | --- |
| Several people are guarded about the same domain | What is actually at stake in that domain? Is their assessment correct? |
| Usage is high and quality complaints are rising | Is the incentive structure rewarding volume over judgement? |
| People are spending most of their time reviewing | Has the workflow changed without anyone planning for the review load? |
| The rollout looked successful and results are drifting | Was delegation mandated above what people accept? |
| One person is enthusiastically advocating and the team is hardening | Is the advocacy making adoption harder? |

Every one of these is an organisational diagnosis. None requires classifying an individual, none creates a record about a named person, and all of them are actionable by the manager rather than by the employee. This is the highest-value managerial use of the model and it happens to be the safest.

### Use it on their own reasoning

A manager can use the model privately to interrogate their own conclusions before acting:

- *Am I treating a domain-specific position as a general attitude?*
- *Am I reading compliance as agreement?*
- *Is this a person problem or a workload problem?*
- *Am I about to push someone past a limit they have not agreed to move?*

This produces better decisions and no data.

### Use it to design conditions

The model's axes describe things a manager actually controls: what tasks are allocated to whom, what delegation level is expected, how much review volume arrives, and what the incentives reward. See [09-adoption-programme.md](09-adoption-programme.md).

## What a manager must not do

| Prohibited | Why |
| --- | --- |
| Record a position against a named employee in any system | It will outlive its context and be read as fact |
| Mention the model or a position in a performance review, calibration, or promotion discussion | Unvalidated framework, non-performance construct |
| Use a position to justify a decision already made | The model becomes an authority-laundering device |
| Assess someone without telling them what is happening | Consent is not optional |
| Assess someone who reports to them without a genuine opt-out | An opt-out that carries a cost is not an opt-out |
| Present the model as established | It is not |
| Use it to decide who gets AI tooling, training, or opportunity | Screening. Direct employment consequence |
| Diagnose distress | `IS` Identity Shock at severity, and `BO` Burnout, are clinical territory. Refer, do not assess |

## HR-specific considerations

### Data protection

Where an organisation records anything from a model-based assessment against an identifiable person, that record is personal data. It concerns the person's psychological response to their work, which places it at the sensitive end of ordinary personal data even where it does not meet a special-category threshold. In a European context, several obligations follow immediately: a lawful basis that is not consent — because consent obtained from an employee by an employer is rarely freely given — purpose limitation, retention limits, subject access, and a data protection impact assessment for anything systematic.

**The practical conclusion is to avoid the entire problem.** If individual results are never recorded, most of these obligations do not arise. A design that aggregates before storage, retains no free text against a name, and produces no individual output is dramatically simpler to run and dramatically harder to misuse.

### Employee representation

In jurisdictions with works councils or equivalent bodies, systematic assessment of employees is normally subject to consultation or co-determination. Introducing a psychological framework across a workforce without that consultation is both a legal exposure and a fast route to justified mistrust. Early engagement is cheaper than retrofitted engagement, and a representative body that has reviewed the safeguards is a useful ally when someone later proposes putting the results into a performance system.

### Aggregation thresholds

Where team-level results are reported:

- **Minimum group size.** No breakdown reported for a group small enough to identify individuals. Five is a common floor; eight is safer for anything sensitive.
- **No intersectional slicing** that reduces a cell below the threshold.
- **No manager access to individual responses,** ever, including their own team's.
- **No time-series comparison of small teams,** which can re-identify individuals through change.

### Anonymity that is actually anonymous

Employees are correct to be sceptical of organisational anonymity guarantees. If free-text responses are collected, they will identify people regardless of whether names are attached. Two options work: collect no free text, or process free text through summarisation before any human in the organisation sees it, with the raw text discarded.

## Team assessment: a defensible design

If an organisation wants a team-level picture, the following design keeps it honest. Each element exists to close a specific failure.

| Element | Purpose |
| --- | --- |
| Participation genuinely voluntary, with visible non-participation normalised | Prevents coerced disclosure |
| Run by someone outside the reporting line | Removes the power asymmetry from the room |
| Individual responses never seen by anyone in management | Prevents the record from existing |
| Results reported only at group level, above the threshold | Prevents re-identification |
| Domains defined by the team, not by management | Prevents the framing being imposed |
| Findings presented as questions about the environment, not conclusions about people | Keeps the output actionable by the right party |
| Explicit written commitment that no result enters any performance process | Makes the misuse a visible breach rather than a drift |
| A stated expiry after which results are deleted | Prevents accumulation into a longitudinal record nobody agreed to |

**The output of such an exercise should be a list of organisational questions**, not a distribution of people across positions. If the deliverable is a chart showing how many people are in each position, the design has failed, because that chart will be shown to someone who wants to know which people.

## What HR gets that is genuinely valuable

The constraints above are heavy. It is fair to ask what remains.

**A vocabulary for a conversation that currently has none.** The prevailing organisational vocabulary for AI adoption has two words, adopter and resister, and both are wrong. Being able to distinguish someone carefully evaluating a genuine threat from someone complying without judgement from someone drowning in review volume is a large improvement, and it requires no assessment at all — only the language.

**A diagnosis for a specific expensive failure.** The rollout that succeeds and then unravels is a real and costly pattern, and the model explains it: delegation forced above what people accept produces compliance that resembles adoption, and it resurfaces later as disengagement, resentment, or exit. An HR function that can anticipate this has something useful.

**An early warning that is not about individuals.** Rising verification burden is measurable from workflow data, requires no psychological assessment, and precedes the burnout it predicts. This is the most actionable thing the model offers an organisation, and it is entirely non-invasive.

**A reason to separate two things that get conflated.** Whether someone uses AI, and whether someone is good at their job, are different questions. Organisations under adoption pressure routinely merge them. The model provides an articulated argument for keeping them apart.

## Questions HR can ask, and questions it cannot

**Can ask, of the organisation:**

- Where is verification burden rising, and who is absorbing it?
- Which mandates are producing compliance rather than judgement?
- Where has delegation been required above what people accept?
- Which domains carry the highest stakes, and is the rollout treating them the same as low-stakes ones?
- Are the incentives rewarding volume in ways that will produce quality failures later?

**Cannot ask, of individuals, in any recorded form:**

- Which position is this person in?
- How does this person feel about AI?
- Is this person resistant?
- Who on this team is likely to struggle?

The second list is the one organisations want answered. The correct response is that the model does not answer it, and that any tool claiming to answer it about named employees should be treated as a liability rather than a capability.
