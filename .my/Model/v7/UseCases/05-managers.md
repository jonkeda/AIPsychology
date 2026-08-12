# Use Cases — Managers

Scenarios for line managers and team leads. Same structure as [04-individuals.md](04-individuals.md): situation, counterfactual, contribution, honest verdict.

Managers are the group where the model's value is most uneven. It is genuinely useful for designing conditions and genuinely dangerous for assessing people, and the same manager will want to do both.

---

## S1. Two people who look the same and are not

**Situation.** Two engineers are described as not on board. One has produced a detailed list of cases where the tool generated plausible and wrong code. The other has not tried it.

**Without the model.** Both receive the same response — encouragement, a training session, a nudge in a one-to-one. The first is insulted, because he has done more evaluation than anyone else on the team and is being treated as uninformed. The second is unaffected, because nothing addressed why he has not started.

**What the model supplies.** These are different situations. The first is careful evaluation of a genuine threat, and the useful move is to engage with the findings — some of which are probably correct and valuable to the team. The second requires understanding what is in the way, which may be time, confidence, or a values position.

**What changes.** The manager stops applying one response to two problems, and starts by asking what each person has actually found.

**Is the difference real?** Yes. The conflation is common, and the cost of getting it wrong with the first engineer is high — that is exactly the person whose evaluation the team needs, and treating them as an obstacle is how an organisation loses its best sceptic.

**Which component did the work.** The open-versus-guarded distinction, used as vocabulary rather than as classification. Notably, the manager does not need to determine which one anyone is in; the useful move is to ask, and the model's contribution is knowing that the question exists.

---

## S2. The rollout that unravelled

**Situation.** Adoption hit ninety percent. Six months later, defect rates are up, two senior engineers have left, and code review has become perfunctory.

**Without the model.** Explained after the fact as change fatigue, or as unrelated attrition. No mechanism, so no prevention next time.

**What the model supplies.** Two mechanisms, both specified in advance. Delegation was mandated above what people accepted, producing compliance without judgement — which measures as success at exactly the point where it should have been detected. And generation capacity rose without verification capacity, so review became either exhausting or nominal.

**What changes.** Substantially, and in advance. Mandate exposure rather than delegation level. Instrument the review-to-production ratio before the push, not after. Read ninety percent adoption with a flat engagement survey as a warning rather than as a result.

**Is the difference real?** Yes, and this is the model's strongest managerial case. It converts a post-hoc explanation into a design rule and a leading indicator.

**Which component did the work.** Coerced calibration and verification burden. No positions, no graph.

---

## S3. The request the model should refuse

**Situation.** A manager wants to know which of his people are behind, so he can direct support.

**Without the model.** He forms an impression anyway, from usage dashboards and enthusiasm in meetings. Both are poor signals. The impression is unreliable and unexamined, and it will influence assignments.

**What the model supplies.** A reasoned refusal, and a redirection. Usage measures usage. Under any mandate or visible tracking it does not measure adoption, understanding, or capability. And enthusiasm in meetings measures how visible someone wants to be.

The redirect: the useful questions are about the environment. Where is review load concentrating? Which domains carry high stakes and are being treated like low-stakes ones? Is refusal safe enough that anyone would say so?

**What changes.** The manager stops trying to rank people and starts examining conditions. Whether this is accepted is another matter — it is not what was asked for.

**Is the difference real?** Yes, but it is harm prevention rather than capability. The model's value here is in what it stops, and it only works if the manager accepts the refusal instead of finding a tool that will answer the original question.

**A caution.** This is where the model's assessment machinery becomes a liability. A manager who has read the position descriptions and the observation guide has been handed something that looks exactly like an instrument for answering the question he was just told not to ask. The existence of the classifier undermines the refusal.

---

## S4. Allocating the review load

**Situation.** Two senior engineers are absorbing most of the review of agent-generated work, because they are the most trusted reviewers. Their own output has fallen. They have not complained.

**Without the model.** Read as a productivity dip in two individuals, possibly raised in a performance conversation. The actual cause is invisible because review time is not tracked anywhere.

**What the model supplies.** Review burden concentrates on the most conscientious and most senior people by default, it is invisible in output metrics, and it produces exactly this pattern. It is a workload distribution problem, not a performance problem.

**What changes.** Review is tracked, rotated, and budgeted. Two people are not managed for a problem the workflow created.

**Is the difference real?** Yes. Making an invisible workload visible is a straightforward intervention with a clear payoff, and the misattribution it prevents is one that damages people who did nothing wrong.

**Which component did the work.** Verification burden alone.

---

## S5. The enthusiast who is not helping

**Situation.** One team member advocates constantly, demonstrates unprompted, and is visibly frustrated by colleagues. Adoption on that team is below average.

**Without the model.** The advocate is treated as an asset and given more visibility, on the reasonable assumption that enthusiasm spreads.

**What the model supplies.** Advocacy grounded in enthusiasm rather than in demonstrated practice tends to harden the people it is aimed at, particularly those with more at stake in the domain. The advocate is producing the opposite of the intended effect.

**What changes.** The advocacy is redirected — into building something useful rather than persuading colleagues — and the enthusiast's own depth of experience is examined before amplifying them further.

**Is the difference real?** Moderate. The observation is plausible and matches common experience, but it is unvalidated conjecture and the model does not disguise that. A manager acting on it is acting on a hunch with a name.

**Honest verdict:** low-to-moderate value. Worth knowing as a possibility, not worth acting on confidently.

---

## S6. Sequencing a rollout

**Situation.** A manager is introducing tooling across a team covering several kinds of work.

**Without the model.** Uniform rollout. Everyone gets the same tools, the same training, the same expectations, on the same schedule.

**What the model supplies.** The same rollout produces calm calibration where stakes are low and acute disruption where they are high. Starting in low-stakes domains builds a real evidence base about the tool's reliability that people can carry into the domains they care about.

**What changes.** Sequencing. Low-stakes first, not because it is easier but because it produces judgement that transfers.

**Is the difference real?** Yes, and it costs nothing. This is a scheduling decision that a manager makes anyway, and the model changes which way it is made.

**Which component did the work.** Identity stakes and domain-specificity.

---

# Assessment for this group

## Where the value is

| Contribution | Strength | Component |
| --- | --- | --- |
| Explaining the unravelling rollout, in advance | Strongest | Coerced calibration |
| Making review load visible and distributable | Strong | Verification burden |
| Sequencing rollouts by stakes | Strong, and free | Identity stakes |
| Separating evaluation from non-engagement | Moderate–strong | Vocabulary only |
| Refusing to rank people, with reasons | Strong, as prevention | The prohibition set |

Every one of these is about **conditions the manager controls**, not about the psychological state of individuals. That is the pattern, and it is consistent enough to be the recommendation: the model earns its place in a manager's hands as a design tool and loses it as an assessment tool.

## Where it is dangerous

The manager is the single most dangerous reader of this model, for a structural reason. A manager cannot have a purely observational relationship with a report. Whatever they conclude sits next to decisions about assignment, opportunity, and evaluation, and no amount of disclaimer changes that.

The specific hazards:

- **The observation guide reads as a diagnostic manual.** It is written carefully, with hedges throughout. It will be used as a checklist, because that is what it looks like.
- **Position labels are memorable and stick.** *Guarded evaluation* will survive in a manager's mental model of a person long after the evidence for it is forgotten.
- **The framework can launder a decision already made.** A manager who has decided someone is a problem now has a vocabulary that makes the judgement sound analytical.
- **Assessment overwhelms design.** Given both, most managers will reach for the assessment, because assessing a person feels more actionable than redesigning a workflow.

## The honest summary

**For managers the model is two products in one package, and the wrong one is more attractive.**

The design product — sequence by stakes, mandate exposure rather than delegation level, instrument review load, do not track individual usage — is genuinely valuable, actionable, and low-risk. It needs no assessment of anyone.

The assessment product — positions, observation guides, classification — is unsupported, hazardous in this specific relationship, and did not contribute to a single scenario above.

**The implication for what to build is direct.** A manager-facing version of the model should contain the conditions, the prohibitions, and the vocabulary, and should not contain the position descriptions, the observation guide, or anything resembling a classification procedure. Shipping the full model to managers means shipping the dangerous half to the audience least able to hold it safely.
