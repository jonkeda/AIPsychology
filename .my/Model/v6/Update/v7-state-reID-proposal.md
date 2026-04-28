# V7 State Re-ID Proposal

Derived from Discussion 01–03. No backward compatibility constraint. Treats the S6/S7 collapse and the S8 terminal family as accepted, then proposes a clean numbering scheme and per-state properties.

---

## Design decisions

1. **Close the S4 gap.** Renumber S5 Understanding → S4 Understanding. The gap was an artifact; there is no reason to preserve it.
2. **Collapse S6 as S5.** The four S6 overuse states become one state (S5 Overuse) with a `driver` attribute.
3. **Collapse S7M/S7I/S7E as S6.** The three integration styles become one state (S6 Integration) with a `style` attribute.
4. **Make Evangelism an overlay.** S7V is not a state someone transitions *to* — it is a behavior that overlays S6 Integration. Rename S6V, mark as overlay.
5. **Create S7 as the terminal family.** S7B Burnout and S3X Structural Displacement share the same structural character (post-engagement, resolved through external means, long residence). Move both under S7.
6. **Dropout is not a numbered state.** It is reachable from every state. Preserved as a cross-cutting concept with severity properties.

---

## New state map

| New ID | Name | Type | Replaces |
|---|---|---|---|
| **S0** | Baseline | State | S0 Baseline |
| **S1** | Initial Encounter | State | S1 Initial Encounter |
| **S2T** | Trust Evaluation | State | S2T Trust Evaluation |
| **S2D** | Defensive Resistance | State | S2D Defensive Resistance |
| **S2P** | Pre-emptive Non-Adoption | State | S2P Pre-emptive Non-Adoption |
| **S3E** | Ego Shock | State | S3E Ego Shock |
| **S3B** | Bargaining | State | S3B Bargaining |
| **S4** | Understanding | State | S5 Understanding |
| **S5** | Overuse | State + drivers | S6E, S6D, S6R, S6S |
| **S6** | Integration | State + styles | S7M, S7I, S7E |
| **S6V** | Evangelism | Overlay on S6 | S7V Evangelism |
| **S7B** | Burnout | Terminal state | S7B Burnout |
| **S7X** | Structural Displacement | Terminal state | S3X Structural Displacement |

State count: **11 states** (down from 18), plus 1 overlay, plus Dropout.

---

## Simplified state graph

```
S0 Baseline
  └─→ S1 Initial Encounter
        ├─→ S2T Trust Evaluation
        │     ├─→ S4 Understanding
        │     └─→ S2D (stakes surface during testing)
        ├─→ S2D Defensive Resistance
        │     ├─→ S3E Ego Shock (defences collapse)
        │     └─→ S3B Bargaining (partial defences)
        └─→ S2P Pre-emptive Non-Adoption
              ├─→ S4 (concern resolved)
              └─→ S2D (competence threat surfaces)

S3E Ego Shock
  ├─→ S3B Bargaining
  ├─→ S4 Understanding (rare, direct)
  └─→ S7X Structural Displacement (economic non-viability confirmed)

S3B Bargaining
  └─→ S4 Understanding

S4 Understanding
  ├─→ S5 Overuse
  └─→ S3E (regression on capability shock)

S5 Overuse
  ├─→ S6 Integration (driver runs dry / fails)
  ├─→ S7B Burnout (cost > value)
  └─→ Dropout

S6 Integration   [+ S6V Evangelism overlay]
  ├─→ S3E (regression on capability shock)
  ├─→ S7B Burnout
  └─→ Dropout

S7B Burnout
  ├─→ S6 Integration (recovery)
  └─→ Dropout (permanent)

S7X Structural Displacement
  ├─→ S4 Understanding in new domain (occupational transition)
  ├─→ Permanent Dropout (principled exit)
  └─→ Advocacy (outside model)

Dropout: reachable from every state.
```

---

## Properties and attributes per state

### S0 — Baseline

| Property | Values | Notes |
|---|---|---|
| `engagement-status` | `transient` \| `permanent` | transient = S1 is pending; permanent = no encounter expected |

The permanence property replaces the current "Two readings" prose note. A permanent-S0 person has no exit edge.

---

### S1 — Initial Encounter

| Property | Values | Notes |
|---|---|---|
| `trigger` | `voluntary` \| `mandated` \| `peer-exposure` \| `demo` | Mandated triggers tend to compress deliberation and increase S2D probability |
| `prior-knowledge` | `none` \| `conceptual` \| `hands-on` | Hands-on prior knowledge makes S4 direct entry more likely |

---

### S2T — Trust Evaluation

| Property | Values | Notes |
|---|---|---|
| `domain-stakes` | `low` \| `moderate` \| `high` | Low stakes is the typical S2T entry condition; high stakes during testing triggers S2T → S2D |
| `updating-symmetry` | `symmetric` \| `asymmetric` | Asymmetric positive-evidence discounting is the S2D diagnostic signal |

Note: `updating-symmetry` is the key property distinguishing S2T from S2D. Both states are preserved because their trajectories diverge, not because their moment-to-moment behavior differs.

---

### S2D — Defensive Resistance

| Property | Values | Notes |
|---|---|---|
| `domain-stakes` | `high` | Defining entry condition |
| `defensive-depth` | `surface` \| `entrenched` | Surface = challenge accessible; entrenched = requires regression event before movement |
| `ethical-overlay` | `none` \| `present` | Marks mixed S2D/S2P cases; affects intervention approach |

---

### S2P — Pre-emptive Non-Adoption

| Property | Values | Notes |
|---|---|---|
| `ethics-source` | `secular-individual` \| `community` \| `religious` \| `economic` | Secular-individual is the well-described case; others are outside the current diagnostic frame |
| `cross-domain-consistency` | `consistent` \| `domain-specific` | Consistent = S2P likely; domain-specific = S2D with ethical language likely |

---

### S3E — Ego Shock

| Property | Values | Notes |
|---|---|---|
| `trigger` | `capability-demo` \| `workflow-disruption` \| `peer-comparison` \| `public-event` | |
| `severity` | `mild` \| `moderate` \| `severe` | Severe = clinical distress range; six-plus months unresolved |
| `domain-stakes` | `high` | S3E does not appear at genuinely low identity stakes |

---

### S3B — Bargaining

| Property | Values | Notes |
|---|---|---|
| `domain-boundary` | free text / domain name | The bounded scope the person has retreated to ("core craft only", "strategy only") |
| `boundary-stability` | `stable` \| `eroding` | Eroding = the domain is shrinking; may transition to S7X if nothing remains |
| `identity-line` | `explicit` \| `implicit` | Whether the person can articulate where their boundary is |

---

### S4 — Understanding

*(Was S5 Understanding. Renamed to close the numbering gap.)*

No state-level attributes beyond the axis properties. The state itself is the stable calibrated position. The axes do the modulation work.

Axis properties (inherited from the axis definitions, recorded here for completeness):

| Property | Values | Notes |
|---|---|---|
| `identity-stakes` | `low` \| `moderate` \| `high` | Per-domain |
| `delegation-ceiling` | `D1` \| `D2` \| `D3` \| `D4` | Per-domain ceiling; can differ from current task delegation |

---

### S5 — Overuse

*(Collapsed from S6E, S6D, S6R, S6S.)*

| Property | Values | Notes |
|---|---|---|
| `driver` | `reward` \| `anxiety` \| `efficiency` \| `social` | Multi-select, ordered by dominance. Multiple drivers are common. |
| `duration` | `acute` \| `sustained` \| `chronic` | Acute = weeks; sustained = months; chronic = years |
| `self-awareness` | `unaware` \| `partial` \| `aware-and-choosing` | Affects intervention approach; aware-and-choosing is not necessarily problematic |

Driver definitions:

| Driver | What it means | Former state |
|---|---|---|
| **Reward** | Intermittent good outputs sustain use regardless of failure rate | S6E Enthusiastic |
| **Anxiety** | Self-trust has transferred to the AI; person doubts their own judgement without it | S6D Dependent |
| **Efficiency** | Productivity metrics or external pressure override quality judgement | S6R Driven |
| **Social** | Peer adoption, team norms, or visibility pressure drive use | S6S Social |

---

### S6 — Integration

*(Collapsed from S7M, S7I, S7E.)*

| Property | Values | Notes |
|---|---|---|
| `style` | `mastery` \| `identity-expanding` \| `ethical` | Multi-select; any combination; all three simultaneously is common |
| `stability` | `stable` \| `under-stress` | Under-stress = approaching S7B or regression threshold |

Style definitions:

| Style | What it means | Former state |
|---|---|---|
| **Mastery** | Knows when to use AI and when not to; draws the line on competence grounds, not identity grounds | S7M Maturity |
| **Identity-Expanding** | AI is constitutive of what the person can now do; the self-concept expanded to include the capability | S7I Identity Expansion |
| **Ethical** | Values, attribution, and consent are integrated into how the person works, not afterthoughts | S7E Ethical Integration |

---

### S6V — Evangelism (overlay)

Not a state. A behavior that overlays S6 Integration. A person in S6 with S6V active is publicly advocating for AI adoption in their domain or field.

| Property | Values | Notes |
|---|---|---|
| `scope` | `peer` \| `organizational` \| `public` | |
| `grounding` | `experience-based` \| `enthusiasm-based` | Enthusiasm-based without depth risks relapse to S5 Overuse |

S6V can co-occur with any S6 style. It is most stable when the Mastery style is also active.

---

### S7B — Burnout

*(Was S7B Burnout. Promoted to S7 terminal family.)*

| Property | Values | Notes |
|---|---|---|
| `severity` | `mild` \| `moderate` \| `severe` | Mild = temporary withdrawal; severe = extended withdrawal with functional impairment |
| `trigger` | `cost-exceeded-value` \| `coerced-adoption` \| `capability-shock` \| `compounded-stress` | |
| `recovery-trajectory` | `active` \| `passive` \| `absent` | Absent = transition to permanent dropout likely |

---

### S7X — Structural Displacement

*(Was S3X Structural Displacement. Promoted to S7 terminal family.)*

| Property | Values | Notes |
|---|---|---|
| `domain-type` | `knowledge-work` \| `service-care-manual` | Knowledge-work = narrowing path to S7X; service/care/manual = elimination path (not fully described) |
| `resolution-trajectory` | `occupational-transition` \| `principled-exit` \| `adversarial-advocacy` | |
| `economic-confirmation` | `partial` \| `confirmed` | Confirmed = person has external evidence of non-viability, not just fear |

---

### Dropout (cross-cutting)

Not a numbered state. Reachable from every state.

| Property | Values | Notes |
|---|---|---|
| `severity-practical` | 0–10 | Existing anchor scale |
| `severity-emotional` | 0–10 | Existing anchor scale |
| `permanence` | `temporary` \| `permanent` | Temporary dropout can resolve; permanent is terminal |

---

## What is removed entirely

| Removed | Replaced by |
|---|---|
| S5 Understanding | S4 Understanding (same content, new ID) |
| S6E Enthusiastic Overuse | S5 Overuse, driver = Reward |
| S6D Dependent Overuse | S5 Overuse, driver = Anxiety |
| S6R Driven Overuse | S5 Overuse, driver = Efficiency |
| S6S Social Overuse | S5 Overuse, driver = Social |
| S7M Maturity | S6 Integration, style = Mastery |
| S7I Identity Expansion | S6 Integration, style = Identity-Expanding |
| S7E Ethical Integration | S6 Integration, style = Ethical |
| S7V Evangelism (state) | S6V Evangelism (overlay) |
| S3X Structural Displacement (under S3) | S7X Structural Displacement (under S7) |

---

## Open questions not resolved here

1. **S2T vs S2D as one state.** The proposal keeps them separate because their trajectories diverge. This remains debatable. A future version could collapse them into S2 Evaluation with a `stance` property (`open` / `defensive`). The asymmetric-updating signal is the real discriminator — it is an observable property, not a state identity.

2. **S2P retention.** The 012p review recommends removing S2P and making it a note inside S2D. The current proposal keeps S2P. Revisit in V8.

3. **The S6V overlay vs. a proper state.** Evangelism has its own observable markers and entry conditions. If S6V turns out to need its own file with transition rules, it may warrant promotion to a state. Mark as provisional.

4. **Descriptive vs. prescriptive.** None of the above resolves the fundamental question in Discussion 03. The properties and attributes are descriptive; they do not imply a recommended trajectory. That decision has to be made at the model level, not the state level.
