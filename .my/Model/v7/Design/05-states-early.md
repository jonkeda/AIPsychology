# Positions — Pre-engagement, Stance, and Disruption

Seven positions across three families. The Working and Exit families are in [06-states-working.md](06-states-working.md).

Each position is described in a fixed order: the voice of the person, what the position is in plain language, entry conditions, attributes, exits, what an observer can actually see, and a falsifiable claim.

---

# Pre-engagement family

## NE — No Engagement

> *"I haven't really used it."*

The person has not had a substantive encounter with AI in this domain. Not a stance, not a refusal, not an opinion held under pressure — an absence. They may have opinions absorbed from the surrounding culture, but those opinions have not been tested against use and are not being defended.

`NE` No Engagement covers two situations that look identical and behave differently, distinguished by an attribute rather than by separate positions.

**Entry:** the starting position. Not reachable from anywhere else. A person who has engaged and stopped is in `DX` Disengagement, not `NE` No Engagement, however long ago the engagement was.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `horizon` | `open` \| `closed` | `open` — an encounter is expected. `closed` — the person does not expect one and is not seeking one. A `closed` `NE` No Engagement has no forward edge. |
| `exposure` | `none` \| `ambient` | `ambient` — the person has absorbed a cultural position without use. Predicts a sharper `FC` First Contact reaction in either direction. |

**Exits:** `FC` First Contact on first substantive use. That is the only forward edge.

**What an observer can see:** absence of usage. This is one of the few positions that is directly and reliably observable, provided the observation window is long enough and covers the domain in question.

**The distinction that matters:** `NE` No Engagement: closed is not `VR` Values Refusal and not `GE` Guarded Evaluation. Those positions require an actively held and defended stance. `NE` No Engagement: closed requires nothing — the person has simply not taken the question up. Treating a non-user as a resister is a common and costly misreading, because it introduces a confrontation where there was no position to confront.

**Testable —** People classified `NE` No Engagement: closed should still be `NE` No Engagement at 24-month follow-up in a substantial majority. If more than roughly a third have entered `FC` First Contact, the `closed` criteria are too loose and are picking up people who were merely slow.

---

## FC — First Contact

> *"Huh. Okay. That's… actually not bad."*

The first substantive encounter with AI performing work in the person's domain, and the reaction to it. `FC` First Contact is brief — a session, sometimes an afternoon. Its importance is out of proportion to its duration, because the stance formed here shapes the next several months.

"Substantive" is doing real work in that definition. Watching a demonstration is not `FC` First Contact. Reading about capability is not `FC` First Contact. `FC` First Contact requires the person to see the tool do something in *their* domain, at a quality they have to assess.

**Entry:** from `NE` No Engagement. Sole entry point.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `trigger` | `voluntary` \| `mandated` \| `peer` \| `demonstration` \| `incidental` | `mandated` compresses deliberation and raises the probability of `GE` Guarded Evaluation |
| `prior-knowledge` | `none` \| `conceptual` \| `hands-on` | `hands-on` makes direct `CU` Calibrated Use entry more likely |
| `outcome-quality` | `poor` \| `mixed` \| `strong` | What the tool actually produced. Strongly shapes the fork, and is frequently forgotten when the episode is recalled later |

**Exits:** `OE` Open Evaluation at low or moderate stakes, `GE` Guarded Evaluation at high stakes, `VR` Values Refusal where a values commitment predates the encounter. Direct `CU` Calibrated Use occurs where stakes are low and prior knowledge is hands-on.

**What an observer can see:** the event itself, if the observation is live. `FC` First Contact is one of the few discrete, dateable moments in the model. Retrospective accounts of it are heavily reconstructed — people narrate their first encounter to fit the stance they subsequently adopted.

**Testable —** The fork is claimed to establish itself within the first substantive session rather than over weeks. Observe first sessions and code stance at 30 minutes and at 30 days. If a large proportion show no stable stance tendency at 30 minutes, the fork is not an `FC` First Contact event and the graph needs restructuring.

---

# Stance family

The three Stance positions are the fork after `FC` First Contact. All three are postures rather than actions: the person is deciding what AI is going to be to them. They are distinguished by what the person does with evidence.

## OE — Open Evaluation

> *"Let me see what it can actually do."*

The person is testing the tool without a stake in the answer. They want to know whether it works. Positive and negative results both update their view, and the view moves.

The defining property is **symmetric updating**. A good output raises the estimate; a bad output lowers it. This sounds trivial and is the single hardest thing to observe, because it is invisible in any one interaction.

**Entry:** from `FC` First Contact at low or moderate stakes. From `VR` Values Refusal when the values concern is resolved or bounded.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `stakes` | `low` \| `moderate` | High stakes with genuine openness is possible but rare, and tends to be unstable |
| `test-scope` | `narrow` \| `broad` | Whether the person is testing one workflow or probing generally |

**Exits:** `CU` Calibrated Use when judgement settles. `GE` Guarded Evaluation when testing surfaces a threat the person did not expect — this is the asymmetric edge described in [04-state-graph.md](04-state-graph.md).

**What an observer can see:** in a single conversation, very little. `OE` Open Evaluation and `GE` Guarded Evaluation present identically in a snapshot: both look like careful, sceptical testing. The discriminating signal is only visible across time.

**The probe that works:** *"Tell me about a time AI impressed you and made you reconsider something."* A person in `OE` Open Evaluation has an answer, and it is specific. A person in `GE` Guarded Evaluation either has no answer or supplies one and immediately discounts it.

**Testable —** `OE` Open Evaluation should update in both directions on mixed evidence. Record stated views before and after five interactions with deliberately mixed outcomes. If bidirectional updating is not the clear majority, the criterion does not separate `OE` Open Evaluation from `GE` Guarded Evaluation and the two positions should collapse into one with a stance attribute.

---

## GE — Guarded Evaluation

> *"It's impressive until you look closely. It doesn't understand anything."*

The person is testing the tool while defending a position. The testing is often rigorous — more rigorous than `OE` Open Evaluation, because a defended position needs better evidence. What distinguishes it is what happens to the results.

The defining property is **asymmetric updating**. Failures are incorporated into the assessment and remembered. Successes are attributed elsewhere: to prompting skill, to a low-stakes example, to luck, to the task having been easy. The view does not move, and the person is not aware that it has not moved.

The V6 name for this was Defensive Resistance. It was renamed because "resistance" is what a change programme calls a person who disagrees with it. What is actually happening is that a person with a genuine investment is evaluating a genuine threat, and their evaluation is skewed by the investment. That is not obstruction; it is ordinary human cognition under threat.

**Entry:** from `FC` First Contact at high stakes. From `OE` Open Evaluation when stakes surface during testing. From `VR` Values Refusal when a competence threat emerges behind the values position. As a regression from any Working position under an access, cost, or trust shock.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `depth` | `surface` \| `entrenched` | `surface` — the position can be engaged directly. `entrenched` — no argument moves it; movement requires an event |
| `ethical-overlay` | `absent` \| `present` | Marks mixed `GE` Guarded Evaluation/`VR` Values Refusal cases. Changes the approach entirely |
| `object` | `capability` \| `access` \| `trust` | What is being defended against. Regression arrivals typically carry `access` or `trust` rather than `capability` |

**Exits:** `IS` Identity Shock when the defence fails against evidence that cannot be discounted. `SB` Scope Boundary when a partial defence holds and a workable line is negotiated. `DX` Disengagement.

**What an observer can see:** the attribution pattern, across at least three or four separate discussions. Within a single conversation, a person in `GE` Guarded Evaluation is indistinguishable from a well-calibrated sceptic who happens to be right.

**Mechanism anchor:** conceptually adjacent to motivated reasoning and to identity-protective cognition — the tendency to process evidence in ways that protect a valued self-concept. Vocabulary, not mechanism.

**Testable —** `GE` Guarded Evaluation should show asymmetric attribution across five or more interactions with mixed outcomes: failures attributed to the tool, successes attributed to circumstances. If a substantial minority update symmetrically, `GE` Guarded Evaluation is not distinct from `OE` Open Evaluation on this criterion.

---

## VR — Values Refusal

> *"I know what it can do. That isn't the issue."*

The person declines to use AI in this domain on grounds that do not depend on how well it performs. Training data provenance, labour displacement, environmental cost, attribution and consent, or a professional-ethical commitment.

The position is defined by **independence from performance**. Improving the tool does not address the objection, because the objection was never about the tool's quality.

**Entry:** from `FC` First Contact only. `VR` Values Refusal is a stance formed at first encounter. Non-use adopted after engagement is `DX` Disengagement or the market-driven pattern described in [06-states-working.md](06-states-working.md), not `VR` Values Refusal.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `source` | `individual-secular` \| `professional-code` \| `community` \| `religious` \| `economic` | Only `individual-secular` and `professional-code` are described well by the current diagnostic frame |
| `consistency` | `cross-domain` \| `domain-specific` | `cross-domain` supports `VR` Values Refusal. `domain-specific` suggests `GE` Guarded Evaluation with ethical language |
| `conditionality` | `conditional` \| `unconditional` | Whether the person can state what would change their position |

**Exits:** `CU` Calibrated Use if the concern is resolved or the person finds a bounded way to act within it. `GE` Guarded Evaluation if a competence threat surfaces behind the values framing. `DX` Disengagement.

**What an observer can see:** the language, which is unreliable, and the consistency, which is better. The strongest available signal is the **domain transfer test**: does the objection hold in a low-stakes domain where the person has no competence to defend? A `VR` Values Refusal position holds. A `GE` Guarded Evaluation position with ethical vocabulary usually does not — the person turns out to use AI freely for things they do not care about.

The **concern-addressed test** is a second signal: if the stated concern were removed — provenance resolved, a licensed model available, disclosure norms established — does the position persist? If it dissolves, it was `VR` Values Refusal. If it produces a new objection, it was probably `GE` Guarded Evaluation.

**Scope limit:** these signals are drawn from Western secular ethics traditions — privacy advocacy, labour rights, open-source ethics. They are not validated for refusal grounded in religious doctrine or in community-held positions inherited from collective experience of earlier technological disruption. In those cases the diagnostic frame does not apply and should not be forced.

**Testable —** Place a sample classified `VR` Values Refusal in roles where AI does not compete with their core skill. If a large proportion resolve within six months, the position is better described as `GE` Guarded Evaluation with ethical language, and `VR` Values Refusal should be demoted to an attribute of `GE` Guarded Evaluation.

---

# Disruption family

Two positions. `IS` Identity Shock is acute and `SB` Scope Boundary is its chronic, stabilised form. Both require the skill to be genuinely at stake; neither appears at low Identity Stakes.

## IS — Identity Shock

> *"I spent fifteen years learning to do that."*

Acute destabilisation when AI convincingly performs the thing the person's professional identity was built around. Not disappointment, not annoyance at a tool — a specific and disorienting reduction in the felt value of accumulated skill.

The characteristic experience is not that the machine is better. It is usually not better. It is that the gap has become small enough that the fifteen years no longer feel like they mean what they meant.

**Duration:** hours to weeks in most accounts. Beyond several months unresolved, the presentation has typically moved into clinical territory — sustained low mood, loss of professional motivation, withdrawal — and belongs with a trained clinician rather than with this model.

**Entry:** from `GE` Guarded Evaluation when the defence fails. As a regression from any Working position under a capability shock, at high stakes.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `trigger` | `capability-demonstration` \| `workflow-disruption` \| `peer-comparison` \| `public-event` | |
| `severity` | `mild` \| `moderate` \| `severe` | `severe` indicates clinical distress; refer out |
| `recurrence` | `first` \| `repeat` | Repeat episodes are typically shorter and are experienced differently — the person recognises what is happening |

**Exits:** `SB` Scope Boundary — by a wide margin the most common, and the healthiest-looking in practice. `CU` Calibrated Use directly, rare and usually misidentified. `SD` Structural Displacement when economic non-viability is confirmed. `DX` Disengagement.

**Intensity by delegation level**, at high stakes — the qualitative anchor that replaced V4's formula:

| Delegation | Experience |
| --- | --- |
| D1 | Barely registers |
| D2 | Mild discomfort |
| D3 | The characteristic `IS` Identity Shock experience |
| D4 | Sharpened by shared authorship |
| D5 | **New in V7 —** distinct: the person cannot locate their contribution at all. **Conjecture —** this is a different experience rather than a more intense one, and the model does not yet describe it well |

**What an observer can see:** very little reliably. Behaviour during `IS` Identity Shock varies from complete withdrawal to compulsive testing to unchanged output with altered affect. Self-report during the episode is poor — people report confusion, irritation, or tiredness rather than identity disruption, because the accurate label is not available to them at the time. Retrospective report months later is considerably better and correspondingly reconstructed.

**Mechanism anchor:** conceptually adjacent to self-efficacy collapse — a sharp downward revision of belief in one's own capability in a specific domain. Vocabulary, not mechanism.

**Testable —** Practitioners at high Identity Stakes should show measurable decline on a domain-specific self-efficacy instrument within four weeks of a major capability release in their domain, relative to a matched low-stakes group. No reliable decline would mean the self-efficacy anchor overstates what is happening.

---

## SB — Scope Boundary

> *"Fine for the first draft. Not for the parts that matter."*

A stable, negotiated line. AI is admitted for some of the work and refused for the rest, and the person can usually say where the line is. `SB` Scope Boundary is the chronic, functional form of the tension that `IS` Identity Shock presents acutely.

`SB` Scope Boundary is frequently stable for years and frequently works. The model makes no claim that it is a stopping point on the way to somewhere better. Many people build good careers here.

**Entry:** from `IS` Identity Shock as the most common resolution. From `GE` Guarded Evaluation where a partial defence holds without an acute episode.

**Attributes:**

| Attribute | Values | Notes |
| --- | --- | --- |
| `boundary` | free text | The actual line, in the person's own words — "structure yes, voice no" |
| `stability` | `stable` \| `eroding` \| `expanding` | `eroding` means the protected domain is shrinking; if it reaches zero, `SD` Structural Displacement |
| `articulation` | `explicit` \| `implicit` | Whether the person can state the line or only enact it |
| `basis` | `identity` \| `competence` \| `mixed` | The discriminator against `IP` Integrated Practice: mastery |

**Exits:** `CU` Calibrated Use when the line is recognised as movable and moves on evidence. `SD` Structural Displacement if the boundary erodes to nothing. `DX` Disengagement.

**What an observer can see:** the boundary itself, easily. What is hard is why it is where it is.

**The distinction from `IP` Integrated Practice: mastery** is the most consequential judgement call in the model, because the behaviour is nearly identical — both look like a person using AI selectively and confidently.

| | `SB` Scope Boundary | `IP` Integrated Practice: mastery |
| --- | --- | --- |
| Where the line sits | Around what the person is known for | Around what the tool is actually unreliable at |
| Under a hypothetical better model | Moves immediately, or refuses to engage | "I would have to test that" |
| After a capability release | Line holds, reasons are restated | Line moves, after deliberate testing |
| Basis when probed | Identity investment | Observed failure rate |

The probe: *"If a model came out next month that was noticeably better at the part you keep for yourself, what would you do?"* An `SB` Scope Boundary answer is immediate in either direction. An `IP` Integrated Practice: mastery answer involves a test.

This heuristic is not a measured instrument. Both positions can produce either answer on a bad day.

**Testable —** `SB` Scope Boundary boundaries should correlate more strongly with domain identity centrality than with the tool's measured failure rate in that domain. Elicit boundaries, then independently measure both correlates. A reversed correlation refutes the claim directly.
