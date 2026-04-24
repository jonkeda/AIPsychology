# Method 1: Internal Survey — Detailed Plan

## Objective

Map where people in the organisation currently sit in the AI Psychological Adaptation Cycle and test whether the stages are recognisable from the inside. This is the fastest, cheapest validation method and the first thing to run.

---

## Survey Design

### Section 1: Current Stage Identification

Present the following descriptions **without stage labels or numbers**. Randomise the order for each respondent to prevent sequence bias.

> **Instructions:** Read each statement below. Select the ONE that best describes how you currently feel about AI tools at work. There are no right or wrong answers.

**A.** "I haven't really used AI tools in any meaningful way. It's not something I think about."

**B.** "I don't think AI tools are as useful as people say. They're overhyped and probably won't change much about how I work."

**C.** "I've tried AI tools and I can see they have some uses, but I notice a lot of flaws. I tend to focus on what they get wrong."

**D.** "Honestly, AI tools make me uncomfortable. If they can do what I've spent years learning to do, I'm not sure what that means for me."

**E.** "I use AI tools for some things, but I have clear boundaries. There are tasks I'll always do myself — that's where my real value is."

**F.** "I've been testing AI tools carefully to understand what they're reliable for and what they're not. I want to know exactly where I can trust them."

**G.** "I understand what AI tools can and can't do. They're useful for certain things, and I've figured out where they fit in my work."

**H.** "I use AI tools constantly — for almost everything. I find it hard to imagine working without them now."

**I.** "I've reached a comfortable balance with AI. I know when to use it and when to rely on my own judgement."

**J.** "AI has expanded what I'm capable of. I think of it as part of how I work and create now."

**K.** "I think a lot about what AI means — for my profession, for creativity, for society. It raises important questions."

**L.** "I've stepped back from AI tools. I was using them too much and I needed a break."

**M.** "I actively help others learn to use AI tools. I enjoy showing people what's possible and helping them get comfortable."

**Mapping key (not shown to respondents):**

| Response | Stage |
|----------|-------|
| A | 0 — Pre-Exposure |
| B | 1 — Dismissal |
| C | 2 — Defensive Resistance |
| D | 3 — Ego Shock |
| E | 3B — Bargaining |
| F | 4 — Trust Evaluation |
| G | 5 — Understanding |
| H | 6 — Overcompensation |
| I | 7A — Maturity |
| J | 7B — Identity Expansion |
| K | 7C — Ethical/Philosophical Integration |
| L | 7D — Burnout/Withdrawal |
| M | 7F — Influence/Evangelism |

---

### Section 2: Stage History

> **Instructions:** Looking back over the past 12 months, select ALL of the statements above that you have felt at some point — even if they don't describe how you feel now.

Same options A–M, multi-select.

Follow-up (free text, optional):

> "If your feelings about AI have changed over time, what caused the shift? (e.g., a specific experience, a new tool, a colleague's influence, a news story, a workplace change)"

---

### Section 3: Identity Attachment

> "How strongly is your professional identity tied to skills that AI can now perform?"

Scale: 1 (not at all) — 10 (my identity is deeply tied to these skills)

> "Which of the following best describes your relationship to skills AI can replicate?"

- "AI can't do what I do — my work requires human qualities AI doesn't have."
- "AI can do some of what I do, but the important parts still require me."
- "AI can do a lot of what I do, and that's something I think about."
- "AI can do most of what I do, and I'm not sure how to feel about that."

---

### Section 4: Delegation Depth

> "What do you currently use AI tools for? Select all that apply."

- Finding or summarising information
- Drafting emails, messages, or short communications
- Writing first drafts of documents, reports, or presentations
- Generating or reviewing code
- Creative work (design, writing, brainstorming, strategy)
- Making decisions or forming judgements
- I don't use AI tools

> "For the tasks you selected, how much do you edit or override what AI produces?"

- I use it as-is most of the time
- I edit it moderately — it gets me 70–80% there
- I heavily rework everything — it's a starting point only
- It depends on the task

---

### Section 5: Dropout Analysis

> "Have you stopped using AI tools after trying them?"

- No — I still use them
- Yes — temporarily
- Yes — I don't plan to go back
- I never started

**If yes:**

> "What was the main reason you stopped?"

- "The outputs weren't good enough for my work" *(practical)*
- "It was too time-consuming to get useful results" *(practical)*
- "It didn't fit into my workflow" *(practical)*
- "It made me uncomfortable about my own skills or value" *(emotional)*
- "I felt like I was relying on it too much" *(emotional)*
- "I felt pressure to use it and resented that" *(emotional)*
- "I was exhausted from constantly learning new AI tools" *(emotional/burnout)*
- Other (free text)

---

### Section 6: Social and External Factors

> "Have any of the following influenced how you feel about AI tools?"

Multi-select:

- A colleague or manager enthusiastically using AI
- A colleague or manager dismissing AI
- A new AI model or tool being released
- News coverage about AI
- A workplace policy or mandate about AI
- Seeing AI produce something impressive
- Seeing AI produce something wrong or harmful
- None of the above

> "Do most people around you at work use AI tools regularly?"

- Yes — it's normal here
- Some do, some don't
- No — I'd be unusual if I used them
- I don't know

---

### Section 7: Demographics (optional, for segmentation)

- Role type: Technical / Creative / Operational / Leadership / Other
- Years of professional experience: <5 / 5–10 / 10–20 / 20+
- Team/department (optional)

---

## Distribution Plan

**Platform:** Whatever internal survey tool is already in use (Forms, SurveyMonkey, Qualtrics, etc.)

**Audience:** Cross-section of the organisation. Aim for representation across:
- Role types (technical, creative, operational, leadership)
- Seniority levels
- Departments/teams
- Known AI adopters and non-adopters

**Sample size target:** Minimum 80–100 responses for meaningful segmentation. If the organisation is large, aim for 200+.

**Anonymity:** Fully anonymous. No identifying information collected. Demographics are optional and coarse-grained (role type, experience band — not name, team, or title).

**Timing:** Keep the survey open for 7–10 days. Send one reminder at the midpoint.

**Estimated completion time:** 5–8 minutes per respondent.

---

## Analysis Plan

### Primary analyses

**1. Stage distribution**
Map responses to stages. Produce a histogram showing where the organisation currently sits. Look for clustering — are most people at Dismissal? Bargaining? Understanding?

**2. Identity attachment × stage correlation**
Test whether people with higher identity-attachment scores (Section 3) are more likely to be in emotional stages (2, 3, 3B) vs. rational/stable stages (4, 5, 7A). Use Spearman correlation or chi-square.

**3. Stage history flow**
From Section 2, reconstruct the most common stage sequences. Do people report moving through stages in the predicted order? Where do they skip? Where do they stall?

**4. Dropout type split**
From Section 5, categorise dropout reasons as emotional vs. practical. Test whether these cluster as distinct groups (chi-square or factor analysis on the reasons).

**5. Delegation depth × stage**
Test whether people using AI for higher-delegation tasks (creative work, decision-making) report more intense emotional stages than people using it for information retrieval.

**6. Social/external influence**
From Section 6, test whether external triggers (model releases, peer behaviour, mandates) correlate with stage transitions reported in Section 2.

**7. Segmentation**
Break all analyses by role type and experience band. Test whether technical vs. creative vs. operational roles show different stage distributions.

### What to look for

- **Face validity confirmed** if >60% of respondents can identify with a single stage description
- **Identity–intensity link confirmed** if identity attachment score correlates with emotional stage placement at r > 0.3
- **Bargaining as distinct phase confirmed** if >15% of respondents select option E as current or historical stage
- **Dropout types confirmed** if emotional and practical reasons cluster separately, not mixed randomly

---

## Reporting

Produce a one-page summary for leadership:
- Where the organisation sits (stage distribution chart)
- Whether the model's core claims hold (identity correlation, bargaining prevalence, dropout types)
- What it implies for adoption strategy (where to invest support, what not to rush)

Produce a detailed report for HR/L&D:
- Full analysis results
- Stage distribution by role type and seniority
- Recommended interventions by stage
- Comparison to the model's predictions — where it fits, where it doesn't

---

## Timeline

| Week | Activity |
|------|----------|
| 1 | Finalise survey questions; pilot with 5–8 people for clarity |
| 2 | Deploy survey; send initial communication |
| 2.5 | Send reminder |
| 3 | Close survey; begin analysis |
| 3–4 | Complete analysis; produce reports |

Total: **3–4 weeks** from start to results.

---

## Risks and Mitigations

| Risk | Mitigation |
|------|-----------|
| Low response rate | Keep survey short (<8 min); leadership endorsement in distribution email; emphasise anonymity |
| Social desirability bias (people pick "Understanding" because it sounds mature) | Present descriptions without labels; randomise order; include "there are no right or wrong answers" framing |
| Ego shock under-reporting (people won't admit vulnerability) | Anonymity; normalising language in the description ("many people experience this"); include it in the history section too (easier to admit in past tense) |
| Self-report inaccuracy | This is a known limitation — flag it in the report. Cross-validate with Method 3 (usage data) and Method 4 (manager observation) in Phase 2 |
