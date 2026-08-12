# Environment Shift Since V6

V6 was written against an AI environment that has since changed in ways that alter which parts of the model carry weight. This document records what changed, what it does to the model, and what the model still cannot describe.

Everything here is **New in V7 —** and none of it has been through a review cycle. It is the least settled material in the design set. It is also the material most likely to matter, because a model of adaptation to a moving target has to move.

## The five changes that matter

### 1. Delegation stopped topping out at partnership

V6's delegation scale ended at D4, "autonomous partnership" — the person and the tool working through something together, with the person present for each step. That was the ceiling of what tooling supported.

Long-horizon autonomous execution changed the shape. A person can now specify an outcome, leave, and return to completed work they did not watch being produced. The scale needs a fifth step, and the fifth step is not simply more of the fourth.

**What it changes in the model:**

- **D5 added to the delegation axis** ([03-axes.md](03-axes.md)).
- **A new intensity row under `IS` Identity Shock** — at D5 the person cannot locate their contribution at all, which is a qualitatively different experience from having a small contribution.
- **Authorship becomes an attribute.** `OL` Oversight Load carries `authorship: retained | ambiguous | lost`. V6 had no vocabulary for this, because at D4 and below authorship was never genuinely in question.

**What the model still cannot describe:** whether repeated D5 delegation erodes the underlying skill, and on what timescale. This is the most commercially and personally consequential question in the whole area, and the model has nothing to say about it beyond noting that people are worried.

### 2. Verification became the work

When output arrived at roughly human production speed, checking it was a step inside the task. When a system produces more in an hour than a person can carefully read in a day, checking becomes the task and then stops being possible.

This is the single largest gap in V6. The model had a rich vocabulary for the psychology of *producing less* and none at all for the psychology of *checking more*.

**What it changes in the model:**

- **Verification Burden added as a fourth axis** ([03-axes.md](03-axes.md)), with the `exceeded` level as the significant one.
- **`OL` Oversight Load added as a position** ([06-states-working.md](06-states-working.md)).
- **A new `BO` Burnout trigger:** `verification-collapse`.
- **A new route to burnout** that does not pass through the person's own overuse. V6 could only explain burnout as a consequence of the person's own usage choices. Much current burnout is not that.

**The specific psychological content** V6 could not name: approving work one has not adequately checked, while knowing it. This is not overwork and it is not imposter feeling. It is a sustained low-grade integrity compromise, and it appears to be widespread.

### 3. Adoption became mandatory

V6 treated workplace mandates as one external trigger among several. Mandates tied to evaluation, compensation, and headcount decisions are now a routine condition of knowledge work rather than an event that happens to some people.

**What it changes in the model:**

- **`OU` Overuse: mandate added as a driver**, separated from `efficiency`. Under `efficiency` the person has internalised the target. Under `mandate` they have not. The behaviour is identical and the psychology is not.
- **Coerced `CU` Calibrated Use promoted from a footnote to an attribute** (`origin: coerced`). It was a marginal case in V6 and is now common enough to need first-class treatment.
- **The Stance family compresses.** Mandated `FC` First Contact gives people less room to form a stance at all, which routes more of them to `GE` Guarded Evaluation and more of them to compliance that looks like `CU` Calibrated Use.

**What this does to measurement:** it contaminates almost everything. In an environment where non-use is a performance problem, self-reported enthusiasm is not evidence of enthusiasm, and usage volume is not evidence of adoption. Any organisational assessment run under a mandate needs to treat both as compromised. See [20-testing.md](20-testing.md).

### 4. Tools now disappear

People build workflows around specific models and specific tools, and those get deprecated, repriced, restricted, or replaced. The experience of losing a tool that a working identity had been rebuilt around is a disruption V6 did not anticipate, because at the time the direction of travel was assumed to be monotonic accumulation.

**What it changes in the model:**

- **A new `⚡` trigger:** model or tool deprecation ([04-state-graph.md](04-state-graph.md)).
- **`GE` Guarded Evaluation gains an `object` attribute** with an `access` value. Regression arrivals in `GE` Guarded Evaluation are frequently not defending identity — they are defending against a supplier whose behaviour has become unpredictable.
- **The Delegation Ceiling becomes less stable.** A ceiling raised through sustained positive experience with one tool does not automatically transfer to its replacement. **Conjecture —** ceilings are partly tool-specific rather than purely domain-specific, which if true is a real change to the axis definition.

### 5. The AI-native cohort arrived

V6 excluded AI-native users from scope on the grounds that they were a future population. They are now colleagues, and the exclusion has become impractical — a team assessment that has nothing to say about a third of the team is not usable.

**What it changes in the model:**

- **The exclusion becomes a cohort property** ([01-model-v7.md](01-model-v7.md)): `pre-AI`, `concurrent`, `AI-native`.
- **The Disruption family is claimed to be cohort-dependent.** `IS` Identity Shock requires a baseline competence to be threatened. Where the competence was formed alongside the tool, there is no clean baseline to lose.
- **The Working family is claimed to be cohort-independent.** `OU` Overuse, `OL` Oversight Load, and `IP` Integrated Practice describe usage patterns that do not depend on when the person learned to work.

**Conjecture —** both claims. The second is the more surprising one and the more useful if true, because it means most of the practically applicable machinery transfers.

**A new question the model cannot answer:** AI-native practitioners may encounter their own `IS` Identity Shock later, when they attempt to build a skill the tool already performs and discover that the motivation to acquire it is difficult to sustain. That is a different phenomenon with the same affect, and the model does not describe it.

## What did not change

Stating this is as important as the changes, because the temptation with a moving subject is to rewrite everything each time.

- **Identity threat still drives the difficult positions.** More capability has intensified this rather than altering it.
- **Position is still per-domain.** If anything more so, since capability now varies more sharply between domains than it did.
- **Regression is still routine** and the triggers are broadly the same ones with two additions.
- **The Stance family is unchanged.** Open versus guarded evaluation, and the asymmetric-updating signature that separates them, describes current behaviour as well as it described V6-era behaviour.
- **`SB` Scope Boundary is still stable and still works.** The prediction that better tooling would dissolve scope boundaries has not obviously happened. Boundaries move; they do not disappear.

## Two things the model should probably say and currently cannot

**Skill maintenance under sustained delegation.** Every practitioner question in this area eventually arrives here: what happens to the underlying capability when it is not exercised, how fast, and whether it recovers. The model records that people worry about it and has no position. Adding one without evidence would be irresponsible; leaving the gap unmarked would be worse.

**Collective rather than individual position.** The model describes individuals. Teams and professions are visibly moving as units — a whole department reaching `OL` Oversight Load together because a workflow changed, a whole profession negotiating a `SB` Scope Boundary through its standards body. The individual frame captures none of this, and aggregating individual positions is not the same as describing a collective one. This is flagged as a decision rather than resolved, in [10-decisions.md](10-decisions.md).
