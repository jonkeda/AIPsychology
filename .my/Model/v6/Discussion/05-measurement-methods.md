# Discussion 05 — Self-Report, Observation, and Other Measurement Methods

Working notes. The model describes states. This document asks: for each state, how can you actually know someone is in it? Three broad methods exist — direct observation of behaviour, self-report, and telemetry / structural proxies. Each has a different profile of strength and bias. Some states are only accessible by one method; others are accessible by all three but contaminated differently by each.

---

## The measurement problem in brief

The model is a state model. States are internal. Internal states are not directly observable. Everything practitioners do — watching someone use AI, interviewing them, reading usage logs — is a proxy for an internal state. Every proxy carries noise.

Two particular contamination risks run through all methods:

1. **Demand characteristics.** If a person knows the model, they will self-present in the state they think they should be in, or the state they want to be in. Once the vocabulary is shared, interview data is unreliable.
2. **Post-hoc rationalisation.** People explain their own behaviour after the fact in ways that are coherent and flattering. A person in S2D (defensive resistance) will almost never report "I am protecting my professional identity"; they will report "the tool isn't reliable enough." Both can be true, but the self-report does not distinguish them.

The methods below are ordered by their independence from self-report. Higher independence = less contamination risk, lower richness.

---

## Method 1 — Behavioural observation

### What can be directly observed

| State | Observable signals | Reliability |
|---|---|---|
| **S0 Baseline** | No AI usage events; no AI-related conversation | High — absence is observable |
| **S1 Initial Encounter** | First substantive usage event; first expressed reaction | High — the moment is discrete |
| **S6 Overuse (any driver)** | High usage volume across tasks; low selectivity | High for presence; low for driver |
| **S7B Burnout** | Near-zero usage after a high-use period; withdrawal from AI-adjacent workflows | High if usage history available |
| **Dropout** | Cessation of use; tool uninstalled or unused | High if telemetry available |
| **D-level of a specific interaction** | What was handed to AI; what was retained by the person | High for the interaction itself |

### What cannot be directly observed

- **Why** someone is using or not using AI (the driver behind S6, the reason for S2D).
- **Internal framing** (is the person in S3E because they are destabilised, or because they are processing something slowly?).
- **The identity stakes** in a domain — you cannot observe how much someone cares about a skill without asking them.
- **Delegation Ceiling** — the maximum the person can accept is not visible until they refuse something.
- **S7M vs S3B** — both look like "uses AI for some things, not others" in any single observation.
- **S2T vs S2D** — both look like "evaluating AI carefully" in any single observation.

### Observation across time changes the picture

Several states are distinguishable longitudinally that are indistinguishable in a snapshot:

| Pair | Snapshot looks | Longitudinal signal |
|---|---|---|
| S2T vs S2D | Both: careful evaluation | S2T updates on positive evidence; S2D does not |
| S3B vs S7M | Both: selective use | S3B boundary holds on identity grounds; S7M boundary moves on evidence |
| S6D vs S6E | Both: high use | S6D: anxious affect, declining independent judgement over time; S6E: energised affect |
| S5 → S3E regression | Both: competent use at snapshot | S3E: usage drops, affect changes after capability event |

Longitudinal observation is the strongest method but requires weeks to months and is rarely available to practitioners in a single engagement.

---

## Method 2 — Interview and self-report

### What self-report adds that observation cannot

- **Internal framing.** "How do you feel about using AI for this?" is the only practical route to the affective register.
- **Reasoning about limits.** "Why won't you use AI for X?" surfaces whether the limit is identity-based (S3B) or competence-based (S7M).
- **Stakes assessment.** "How central is this skill to your professional identity?" cannot be derived from usage data.
- **Ethical stance.** S2P and S7E are almost entirely self-report-dependent — the values work is internal.
- **History.** "What was your first significant AI experience?" — only the person knows.

### What self-report cannot do reliably

- **Distinguish states that share vocabulary.** A person cannot reliably tell you whether their boundary is identity-drawn or competence-drawn by introspection alone. They will tell you a story that sounds like the one they prefer.
- **Report S6D accurately.** Dependent overuse requires the person to admit their self-trust has transferred to AI. This is ego-threatening. They will report "efficiency" instead.
- **Report S3E accurately during S3E.** Acute disruption is hard to label while in it. People in S3E typically report "confusion" or "frustration," not "identity threat."
- **Give uncontaminated data after model exposure.** Once someone has read this model, their self-report is partly a performance for the framework.

### Self-report by state

| State | Self-report reliability | Primary contamination risk |
|---|---|---|
| **S0 Baseline** | High — "I haven't used AI meaningfully" is easy to verify | Low |
| **S1 Initial Encounter** | High — "My first real experience was..." | Retrospective distortion |
| **S2T Trust Evaluation** | Moderate — person can describe their evaluation process | Demand characteristics; may not notice asymmetric updating |
| **S2D Defensive Resistance** | Low — person attributes resistance to tool quality, not identity threat | Post-hoc rationalisation |
| **S2P Pre-emptive Non-Adoption** | Moderate — values are articulable; but may mix with S2D | Moral self-presentation |
| **S3E Ego Shock** | Low during episode; higher retrospectively | Retroactive framing as "just a phase" |
| **S3B Bargaining** | Moderate — the boundary is often consciously held | Identity-protective framing of the boundary |
| **S4 Understanding** | Moderate — "I know when to use it" is reportable | Overclaiming competence |
| **S5 Overuse** | Moderate for Reward/Efficiency drivers; low for Anxiety driver | Anxiety driver = ego-threatening to report |
| **S6 Integration** | High for Mastery style; moderate for Ethical; lower for Identity-Expanding | Mastery = least threatening to report |
| **S7B Burnout** | High — withdrawal is recognised and articulable | May minimise severity |
| **S7X Structural Displacement** | High — the economic framing is external and conscious | None specific |

### Probe questions by state

The observation guide already documents many probes. The key principle: **probe indirectly**. Asking "are you in S2D?" elicits demand-characteristic response. Asking "tell me about a time AI impressed you in this domain" elicits behaviour that reveals the state.

| State target | Indirect probe |
|---|---|
| S2D vs S2T | "Tell me about a time AI did something that made you reconsider your view." |
| S3B vs S7M | "If a new model came out tomorrow that was noticeably better at [core task], what would you do?" |
| S6 Anxiety driver | "If AI were unavailable for a week, what would you feel — not do, feel?" |
| S6 Social driver | "If you were working entirely alone on this, with no one seeing your process, how would you use AI?" |
| S3E | "What was the moment you found most uncomfortable when you first encountered AI doing this?" |
| S2P | "Would your position change if AI could demonstrably solve [stated concern]?" |
| S7B | "At what point did it stop feeling worth it?" |

---

## Method 3 — Usage telemetry and structural proxies

### What telemetry can measure

| Signal | What it reveals | Limitations |
|---|---|---|
| **Usage volume over time** | S6 presence (high); S7B (collapse after high); S0 (absent) | Volume is state-agnostic for S6 drivers |
| **Tool switching frequency** | S2T evaluation behavior; S3B scope management | Cannot separate genuine testing from anxiety-driven checking |
| **D-level distribution** | What kinds of tasks are being delegated | Requires classifying tasks, which is manual |
| **Domain distribution** | Which domains AI is used in vs not | High-value signal for multi-domain picture |
| **Session patterns** | S6D often shows AI-checks-on-AI-output; S7M shows bounded, purposive sessions | Requires session-level granularity |
| **Revision rate** | How much the person edits AI output | Proxy for S7M (high revision) vs S6E (low revision) |
| **Error correction rate** | Does the person catch AI errors or propagate them? | Strong S7M vs S6E signal |

### What telemetry cannot measure

- Identity stakes — there is no log event for "this domain matters to me."
- Affective register — the log does not record anxiety or conviction.
- Reasoning — why the person chose to delegate or not.
- S3E — the state is internal; the behaviour during S3E varies widely.
- S2D vs S2T — both can produce similar usage patterns.

### Structural proxies (external to the person)

Some state indicators can be inferred from situational facts rather than from the person directly:

| Proxy | What it suggests |
|---|---|
| **Domain tenure** (years in this field) | High tenure = higher identity stakes are likely |
| **Income dependence** on the domain | High income dependence = higher stakes |
| **Public identity** ("known for this skill") | High public identity = higher stakes |
| **Organisational context** (mandatory AI use, leaderboards) | Predicts S6 Efficiency or Social driver |
| **Peer adoption rate** in the person's network | Predicts S6 Social driver or S1 exposure trigger |
| **Recent capability event** (major model release) | Predicts S3E regression risk for high-stakes domains |

Structural proxies are useful for **predicting** which states are likely before observing the person. They are not reliable for classifying the current state.

---

## Method combinations by purpose

Different use cases warrant different method combinations.

### Practitioner trying to understand one person

Priority order:

1. Structural proxies first — identify likely high-stakes domains before the conversation.
2. Behavioural observation during working session if possible — watch actual AI use before interviewing.
3. Indirect interview probes — elicit stories, not self-classifications.
4. Verify with longitudinal follow-up — check whether S3B boundary moves on evidence over the next month.

Avoid: sharing the model vocabulary before assessment is complete.

### Researcher running a study

Priority order:

1. Pre-register domain identification and stakes assessment (structural proxies + brief pre-interview) before any state observation.
2. Collect usage telemetry during the observation period.
3. Post-study interview with indirect probes, using the telemetry as anchors ("I can see you stopped using AI for X in February — what happened?").
4. Blind-rate states from interview transcripts. Have a second rater do the same. Compute agreement.

The measurement note in `01-axes.md` applies: stakes must be assessed before states are observed or the fork prediction is circular.

### Organisation mapping a team

Priority order:

1. Anonymous self-report instrument — broad picture of where people think they are, understanding this is contaminated.
2. Usage telemetry for domains and volume — corrects for self-report demand characteristics.
3. Manager or peer observation notes — catches states people won't self-report (S6D especially).
4. Small-group follow-up conversations for ambiguous cases.

Team-level work should not rely on self-classification into named states — too much demand characteristic. Describe the states in behavioral terms and let the person locate themselves relative to examples.

---

## States ranked by measurement difficulty

| Difficulty | State(s) | Primary method | Why it's hard |
|---|---|---|---|
| **Easy** | S0, S7B, Dropout | Telemetry / observation | Presence/absence is observable |
| **Easy** | S7X Structural Displacement | Self-report | The person knows; the framing is external |
| **Moderate** | S1, S3B boundary, S7M vs S3B | Interview | Indirect probes work; longitudinal confirm |
| **Moderate** | S6 Overuse (Reward, Efficiency, Social drivers) | Interview + telemetry | Driver not in the telemetry; probe works |
| **Hard** | S2T vs S2D | Longitudinal observation | Asymmetric updating only visible over time |
| **Hard** | S3E | Retrospective interview | Hard to label during episode |
| **Hard** | S5 Overuse (Anxiety driver) | Careful indirect interview | Ego-threatening; denial common |
| **Hard** | S6 Integration styles (Identity-Expanding) | Interview | Identity change is internal |
| **Very hard** | S2D vs S2P | Multi-month longitudinal + cross-domain | Neither method alone distinguishes |
| **Very hard** | Delegation Ceiling | Refusal events over time | Not observable until someone refuses |

---

## Open questions

- **Self-report instruments.** No validated questionnaire exists for placing people in states. Designing one is possible but requires careful item construction to avoid demand characteristics (items should not name states, only describe behaviours and feelings).
- **Inter-rater reliability.** The S3X Testable item (Discussion 03, from the 005c plan) proposes a kappa-based reliability test. The same design should be applied to S2D/S3B/S7M triples, which are the hardest to reliably distinguish.
- **Telemetry access.** In most organisational contexts, the practitioner does not have access to usage logs. The methods that depend on telemetry are practitioner-unfriendly in practice.
- **Model contamination.** If this model becomes widely used, self-report data from people who have read it is unreliable for validation. Any validation study should use participants who have not been exposed to V6 vocabulary.
