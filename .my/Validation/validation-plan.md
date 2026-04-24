# Validation Plan: The AI Psychological Adaptation Cycle

How to test whether this model reflects reality — not just intuition.

---

## What needs validating

The model makes several testable claims:

1. People move through recognisable psychological stages when adopting AI
2. The stages follow a rough sequence (though not rigidly linear)
3. Emotional intensity scales with identity attachment and delegation depth
4. Bargaining is a distinct, prolonged phase — not just a transition
5. External triggers (model releases, mandates, peers) can regress people to earlier stages
6. Social normalisation is a separate factor from individual understanding
7. There are distinct end states, not a single "adoption" outcome
8. Practical dropout and emotional dropout are different mechanisms

Each of these can be tested independently.

---

## Method 1: Internal Survey (Quick, Low-Cost)

**Purpose:** Map where people in the organisation currently sit in the cycle and test whether the stages are recognisable from the inside.

**Approach:**

- Anonymous survey across a cross-section of roles (technical, creative, operational, leadership)
- Present the stage descriptions *without labels* and ask: "Which of these best describes how you currently feel about AI at work?"
- Follow up with:
  - "Have you previously felt differently? Select any stages you've passed through."
  - "What triggered the shift?"
  - "How strongly is your professional identity tied to skills AI can now perform?" (1–10 scale)
  - "Have you stopped using AI after trying it? If so, why?" (emotional vs. practical options)

**What it validates:**
- Whether the stages are self-recognisable (face validity)
- Whether identity attachment correlates with emotional intensity (Claims 1, 3)
- Whether bargaining is common and prolonged (Claim 4)
- Whether dropout splits into emotional and practical types (Claim 8)

**Limitations:** Self-report bias. People may not accurately identify their own stage, especially ego shock (Stage 3) which involves vulnerability.

**Timeline:** 2–3 weeks to design, deploy, and analyse.

---

## Method 2: Longitudinal Interviews (Medium Effort, High Insight)

**Purpose:** Track individuals through the cycle over time to test sequencing and transitions.

**Approach:**

- Recruit 15–25 participants across roles and identity-attachment levels
- Interview at baseline and then monthly for 6 months
- Semi-structured interviews covering:
  - Current relationship with AI tools
  - Emotional response to recent AI interactions
  - Any boundaries they've set ("I use it for X but not Y")
  - What triggered any shifts in attitude
  - Whether peers, media, or model releases influenced their stance
- Code interviews against the model's stages
- Track movement: do people follow the predicted sequence? Where do they skip, stall, or regress?

**What it validates:**
- Stage sequencing and transitions (Claim 2)
- Bargaining as a distinct, durable phase (Claim 4)
- External triggers causing regression (Claim 5)
- Whether low-identity users genuinely skip emotional stages (Claim 3)

**Limitations:** Small sample. Labour-intensive. Observer effect — being studied may change behaviour.

**Timeline:** 6–9 months for data collection, plus analysis.

---

## Method 3: Usage Data + Sentiment Correlation (Quantitative)

**Purpose:** Test whether behavioural patterns in AI tool usage correspond to predicted emotional stages.

**Approach:**

- Collect anonymised AI tool usage data (frequency, task types, delegation depth, duration of sessions)
- Pair with periodic micro-surveys (2–3 questions, weekly) capturing emotional state and confidence
- Look for predicted patterns:
  - **Dismissal:** Zero or near-zero usage
  - **Defensive Resistance:** Brief sessions, low-delegation tasks, declining frequency after initial spike
  - **Bargaining:** Consistent usage but restricted to specific task types — predictable boundaries
  - **Trust Evaluation:** Systematic, varied task types, comparison behaviour
  - **Overcompensation:** Usage spike, broadening task types, increasing delegation depth
  - **Stabilisation:** Usage plateau at a consistent level and task mix
  - **Regression:** Usage drop or task-type narrowing after an external event (model release, etc.)

**What it validates:**
- Whether usage patterns map to predicted stages (Claims 1, 2)
- Whether delegation depth correlates with emotional intensity (Claim 3)
- Whether external triggers cause measurable regression (Claim 5)
- Whether overcompensation is a real, observable phase (Claim 1)

**Limitations:** Usage data alone doesn't prove emotional states — needs the sentiment pairing. Privacy considerations require careful anonymisation.

**Timeline:** 3–6 months of data collection. Requires tooling access and data governance approval.

---

## Method 4: Manager Observation Framework (Practical, Organisational)

**Purpose:** Test whether managers can reliably identify stages in their reports, and whether stage-aware management changes outcomes.

**Approach:**

- Train a cohort of managers (10–15) on the model
- Ask them to log observed behaviours in their teams over 3 months, coded by stage
- Compare against:
  - Self-reported stages from team members (Method 1)
  - Usage data if available (Method 3)
- Measure inter-rater reliability: do different managers identify the same stage for the same person?
- In a second phase, test whether stage-aware interventions (e.g., support during ego shock vs. pressure during ego shock) change adoption outcomes

**What it validates:**
- Whether stages are observable from the outside (construct validity)
- Whether the model has practical utility for management (applied validity)
- Whether stage-matched interventions outperform generic ones

**Limitations:** Manager bias. Hawthorne effect. Small sample unless scaled.

**Timeline:** 3–4 months for observation phase, 3–4 months for intervention phase.

---

## Method 5: Retrospective Case Studies (Low Cost, Narrative)

**Purpose:** Test the model against known adoption journeys — people who've already gone through the full cycle.

**Approach:**

- Identify 8–12 people in the organisation (or externally) who are now mature AI users (Stage 7)
- Conduct detailed retrospective interviews:
  - "Walk me through your history with AI tools, from first exposure to now."
  - "Were there moments of resistance, doubt, or over-enthusiasm?"
  - "Did anything external — a new model, a colleague, a news story — change how you felt?"
  - "Did you ever set rules for yourself about when to use AI and when not to?"
- Map each narrative to the model's stages
- Check: does the model fit their experience, or do they describe phases the model misses?

**What it validates:**
- Whether the full cycle is recognisable in real histories (narrative validity)
- Whether bargaining (3B) and ego shock (3) actually occur as described
- Whether the model misses any stages that real people report
- Whether end states (7A–7F) are accurately differentiated

**Limitations:** Retrospective bias — people reconstruct memories to fit narratives. Survivorship bias — you're only interviewing people who made it through.

**Timeline:** 4–6 weeks.

---

## Method 6: Cross-Cultural Comparison (Higher Effort, High Value)

**Purpose:** Test whether the model holds across different cultural contexts or whether it's specific to Western knowledge-worker culture.

**Approach:**

- Replicate Method 1 (survey) or Method 2 (interviews) across at least 3 culturally distinct groups:
  - A Western individualist knowledge-work culture
  - A collectivist or hierarchical work culture
  - A techno-optimistic culture (e.g., parts of East Asia, Nordics)
- Compare:
  - Which stages are universally present
  - Which stages are culturally amplified or absent
  - Whether social vs. individual factors dominate differently
  - Whether bargaining looks different in collectivist contexts

**What it validates:**
- Cultural variability claims
- Whether the model is universal or culture-specific
- Which stages are hardwired human responses vs. culturally constructed

**Limitations:** Expensive. Requires cross-cultural research partnerships. Language and framing differences complicate comparison.

**Timeline:** 6–12 months.

---

## Method 7: Controlled Experiment (Highest Rigour)

**Purpose:** Test the causal structure of the model — do identity attachment and delegation depth actually *cause* the predicted emotional responses?

**Approach:**

- Recruit participants with measured identity attachment (pre-screened via validated scales like the Professional Identity Scale)
- Randomly assign to AI tasks at different delegation depths (D1–D4)
- Measure emotional response at each stage using validated instruments:
  - State-Trait Anxiety Inventory (STAI) for anxiety
  - PHQ-9 or similar for depressive response
  - Rosenberg Self-Esteem Scale for identity impact
  - Custom measures for bargaining behaviour and overuse patterns
- Predict: high-identity participants at high delegation depth will show stronger Stage 2–3 responses than low-identity participants at low delegation depth

**What it validates:**
- Causal relationship between identity attachment, delegation depth, and emotional intensity (Claim 3)
- Whether ego shock is a real measurable response, not just a narrative

**Limitations:** Artificial setting. Ethical considerations — deliberately inducing ego shock requires careful oversight and IRB/ethics approval. Short timeframe may not capture full cycle.

**Timeline:** 3–6 months including ethics approval, recruitment, and analysis.

---

## Recommended Sequence

Not all methods need to happen at once. A phased approach:

| Phase | Method | Effort | What you learn |
|-------|--------|--------|---------------|
| **1 (Now)** | Internal Survey (Method 1) | Low | Where the org currently sits; face validity |
| **1 (Now)** | Retrospective Cases (Method 5) | Low | Whether the full cycle matches real histories |
| **2 (Month 2–3)** | Manager Observation (Method 4) | Medium | Whether stages are observable and actionable |
| **2 (Month 2–3)** | Usage Data + Sentiment (Method 3) | Medium | Behavioural evidence for stage patterns |
| **3 (Month 4+)** | Longitudinal Interviews (Method 2) | High | Sequencing, transitions, regression triggers |
| **4 (If publishing)** | Cross-Cultural (Method 6) | High | Universality vs. cultural specificity |
| **4 (If publishing)** | Controlled Experiment (Method 7) | High | Causal evidence for core claims |

Phase 1 alone would give enough signal to know whether the model holds up internally and is worth investing in further.

---

## What would disprove the model?

A model is only useful if it's falsifiable. The model would be weakened or disproven if:

- Most people don't recognise any of the stages in themselves
- Identity attachment doesn't correlate with emotional intensity
- Bargaining doesn't appear as a distinct phase — people go straight from resistance to understanding
- External triggers don't cause measurable regression
- Usage patterns show no correspondence to predicted stages
- The stages appear in a fundamentally different order than predicted
- The model fits Western knowledge workers but no one else

Any of these findings would be valuable — they'd tell us what to revise, not just what to confirm.
