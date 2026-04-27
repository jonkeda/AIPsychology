# Dropout — Two Severity Axes

V4 split dropout into emotional and practical, with a warning that confusing them leads to wrong interventions. V5 kept the distinction but replaced the binary with **two independent severity axes**, because most real dropouts are mixed (a tool failure that lands in an identity-vulnerable spot). V6 keeps the V5 frame.

A dropout is characterised by two scores:

- **Practical severity (0–10)** — the degree to which tool failures, workflow friction, bad outputs, prompt fatigue, or cost drove the exit.
- **Emotional severity (0–10)** — the degree to which identity threat, ego shock, fear, or exhaustion drove the exit.

A dropout is not a single point on one axis but a position on the plane.

### Practical severity anchors

| Range | Description | Example |
| --- | --- | --- |
| **0–3** | Tool meets most needs; friction is minor | Occasional slow responses; one tool doesn't support a niche format |
| **4–6** | Significant gaps; core tasks still work | Reliable hallucination in the domain; cost is high but manageable; prompt fatigue on complex tasks |
| **7–10** | Tool fails critical tasks or is effectively unusable | The tool cannot perform the domain's primary task type; cost makes regular use impractical; outputs require more correction than starting from scratch |

### Emotional severity anchors

| Range | Description | Example |
| --- | --- | --- |
| **0–3** | Mild discomfort; self-concept intact | Vague unease about AI in the profession; no change in day-to-day confidence |
| **4–6** | Meaningful identity pressure; reduced confidence | Recurring doubt about the value of one's expertise; avoidance of AI in specific identity-relevant tasks |
| **7–10** | Severe identity disruption or exhaustion | Cannot engage with AI without significant distress; self-confidence in core competence has materially declined; or complete emotional exhaustion from sustained S6D or S6R |

| Region | Description | Intervention |
| --- | --- | --- |
| High practical / low emotional | Tool genuinely doesn't work for them | Better tools, training, defaults |
| Low practical / high emotional | Identity threat or exhaustion | Psychological support, gradual re-exposure, social context shift |
| High practical / high emotional | Mixed — tool failed in an identity-vulnerable spot | Both interventions; address tool first to clear the rationalisation |
| Low / low | Boredom, indifference, opportunity cost | Often not worth intervening |

## Operational test — the reversibility check

Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit even if the cited reason was practical. This is the closest thing the model has to a clean operationalisation of the dropout space.

**Testable —** the reversibility check is a study-able protocol. **Conjecture —** inter-rater reliability of the 0–10 axes has not been established.

## Mechanism anchors

- Practical severity → conceptually related to **expectancy violation** in the usability sense — the tool failed to do what its perceived capability promised.
- Emotional severity → conceptually related to **threat-driven avoidance** — continuing use predicts further psychological cost, so the person stops.

Borrowed as vocabulary, not as tested causal mechanisms.

## Reach

Dropout is reachable from **every state**, including [S7M Maturity](states/S7M-maturity.md). Severity scores are independent of which state the person dropped from.

## What dropout is not

- **Not [S3X Structural Displacement](states/S3X-structural-displacement.md).** S3X is structural non-viability, not insufficient willingness to continue.
- **Not [S2P Pre-emptive Non-Adoption](states/S2P-pre-emptive-non-adoption.md).** S2P is a values-grounded stance reached at first encounter, not after engagement.
- **Not permanent S0.** Permanent non-users in [S0 Baseline](states/S0-baseline.md) have not engaged at all; dropout requires prior engagement.
