# 008-comparative.md — V6 Against Prior Frameworks

## TL;DR

- **V6 borrows structure from TAM and TTM but supplies what they lack:** per-state intensity modulation via two axes (Identity Stakes, Task Delegation Level). This is genuine original work.
- **The S6 split (Enthusiastic/Dependent/Driven/Social) and S7 split are vocabulary-level additions.** They rename Rogers' adopter categories and relabel TTM maintenance modes. Useful for knowledge-work AI, but not mechanically new.
- **The practical × emotional dropout plane is defensible and original,** but only within a narrow operationalisation (reversibility test). Outside that test it is speculation.
- **S3X Structural Displacement and PEN Pre-emptive Non-Adoption are real gaps in prior frameworks.** S3X fills a hole that TAM, Rogers, and TTM leave (economic non-viability distinct from psychological resistance). PEN is new to this domain, borrowed from the ethics literature but not from mainstream adoption models.
- **The per-domain identity-stakes scoping is original and load-bearing.** This is what distinguishes V6 from all five comparison frameworks — no prior model lets you be in different states for different domains while varying intensity by delegation level.
- **Descriptive-first with inline markers is a framing improvement, not a structural one.** It does not change the model's claims; it changes how transparent they are about uncertainty.
- **Recommendation: Keep the two-axis modulation (1), per-domain scoping (5), S3X (6), PEN (7), and the dropout plane (3).** Drop or subsume claims 2 (S6/S7 splits are just renamed Rogers) and 8 (descriptive-first is hygiene, not substance). Replace claim 4 (limits-of-operationalization) with a data-driven roadmap.

---

## Comparative Findings

### 1. Identity Stakes × Task Delegation Level modulation is genuinely original — testable against all five priors

**What V6 borrows:** The structure of states-with-transitions appears in TAM (usefulness + ease-of-use drive adoption), Diffusion of Innovations (adoption depends on compatibility), Transtheoretical Model (discrete stages), and the Gartner Hype Cycle (technology maturity trajectory).

**What V6 adds:** No prior framework varies *intensity within a state* across two independent axes. TAM predicts *whether* someone adopts; V6 predicts *how intensely they struggle* in S3E Ego Shock or S6E Enthusiastic Overuse depending on whether their professional identity is at stake and how much cognitive delegation they hand to the AI.

This is the first framework to model:
- The same person in the same state feeling different intensity when stakes change (high-stakes translator in S2D Defensive Resistance feels it harder than low-stakes travel-planner).
- The same person, same domain, same day experiencing different intensity for different interactions (D1 Information query generates no emotion; D4 autonomous partnership activates the full S3E Ego Shock if stakes are high).

**The claim is testable.** Compare a high-identity-stakes person using AI for core work (translation, code review, medical diagnosis) against low-identity-stakes use (email summarization, schedule planning) and measure emotional affect, usage hesitation, error-checking behavior. Predict: high-stakes pairs with higher resistance/shock intensity. Low-stakes pairs with skipping resistance altogether. Confounds: prior exposure, individual anxiety traits, workplace culture.

**Across the five priors, this axis multiplication exists nowhere:**
- TAM has usefulness and ease-of-use, but they are factors in the adoption *decision*, not modulators of the emotional intensity of states after adoption.
- Rogers has compatibility with existing practice, but does not decompose the compatibility into "how much of my identity rides on this" vs "how much am I delegating this interaction."
- TTM stages move sequentially toward a goal; no stage is *more intense* based on how high the stakes are.
- Transtheoretical Model does not contemplate the possibility of varying intensity within a stage.
- Gartner Hype Cycle is a population-level technology trajectory; it has no concept of individual intensity variation.

**Fix:** Retain the two-axis modulation as V6's primary original claim. Test it before the next major framework revision. The operationalisation exists: measure affect, hesitation, error-checking, delegation reluctance in same-person contrasts (high-stakes domain vs low-stakes domain, D1 vs D4 in same domain).

---

### 2. The S6 four-way split (Enthusiastic, Dependent, Driven, Social) is vocabulary-level re-labeling of Rogers' adopter category spectrum, not a structural innovation

**What V6 borrows:** Rogers identifies distinct adopter *attitudes* toward innovation: early adopters are venturesome and willing to accept risk; early majority are deliberative; late majority are skeptical; laggards are tradition-bound and suspicious of change. V5 and V6's S6 states map onto this: S6E Enthusiastic (early adopter attitude), S6D Dependent (early majority who adopt but doubt themselves), S6R Driven (late majority conforming to pressure), S6S Social (group-norming behavior).

**What V6 adds:** The naming is clearer for knowledge-work AI specifically. And the coexistence rules (S6E + S6D mutually exclusive; S6R + S6S can coexist in pressure-cultures) add precision to Rogers. But this is refinement of a populated taxonomy, not a new discovery.

**The deeper issue:** Rogers' categories describe *population distribution* of attitudes. V6 applies them to *individual trajectory* — the same person moves from S6E to S6D to S7B. That is a conceptual shift (from cross-sectional distribution to longitudinal path), but Rogers does not forbid it. Rogers' framework is silent on whether individuals change attitudes, but it is consistent with the idea that they do.

**The four states are behaviorally distinct** if you have time-series data (high usage + uncritical is S6E; high usage + self-doubt is S6D; high usage + pressure-compliance is S6R; high usage + peer-conformity is S6S). But if you have a snapshot, S6E and S6D both look like "person uses the tool a lot." The distinction requires longitudinal observation or self-report, per [limits-of-operationalization.md](limits-of-operationalization.md).

**Fix:** Rename this finding from "original S6 split" to "taxonomy refinement." Do not claim novelty beyond Rogers. In the model prose, credit Rogers explicitly in the S6 state files for the psychological mechanisms (early-adopter enthusiasm, conformity pressure, self-doubt in innovation integration). Keep the four-state model because it is useful for practitioners; drop the implication that it is mechanically new.

---

### 3. The practical × emotional severity dropout plane is original and operationalisable, but only via the reversibility test

**What prior frameworks do with dropout:** TAM, Rogers, TTM, and Gartner all treat dropout / non-adoption as a single failure state. They ask *whether* someone abandons the innovation but not *why* — what internal psychological process vs external friction drove the exit.

**What V6 adds:** The two-axis plane distinguishes:
- **High practical / low emotional:** tool failure. User says "the output was bad" and means it. Fix: better tool, training, better defaults.
- **High emotional / low practical:** identity threat or exhaustion. User says "it was too stressful" and means it. Fix: psychological support, gradual re-exposure, social re-framing.
- **High / high:** mixed. User cites a tool failure but would have tolerated it if the identity threat were lower. Intervention: fix the tool first to remove the rationalisation.
- **Low / low:** indifference or opportunity cost. Not worth intervening.

This is novel in adoption frameworks. Rogers, TAM, and TTM do not separate practical failure from emotional failure. Gartner Hype Cycle maps technological maturation but not user psychological drivers of dropout.

**The operationalisation problem:** The reversibility test works if you can provide the user a tool that actually solves the cited practical failure. If they use it, practical was high. If they don't, emotional was driving the exit. This is a clean test *when the cited failure is tool-specific and reproducible*.

**But it breaks when:**
- The "tool failure" is actually workflow friction or task redesign, not the tool itself. Offer a better summarizer and the real problem was the person never needed summaries in the first place.
- The practical failure and emotional failure are confounded in a single event. The person's first AI-generated email was both bad *and* felt like it replicated their writing voice — the emotion and the practical failure are the same event.
- The emotional cost accrues over time (burnout from sustained high-delegation overuse). Fixing the tool doesn't undo the fatigue.

**Testable claim within the reversibility test:** For single-incident dropouts with clear tool-citable failures (bad summarization, slow response, wrong output format), the reversibility test successfully distinguishes practical from emotional in 80%+ of cases. Confound: people rationalize emotional exits as practical ones.

**Conjecture remaining:** The 0–10 severity axis is not calibrated. Two raters scoring the same dropout case will not correlate to ±1 on the practical or emotional axis without a scorecard.

**Fix:** Keep the two-axis plane and the reversibility test. Document that the test is most reliable for acute single-incident dropouts with citable tool failures. For chronic dropouts (sustained overuse leading to burnout) or workflow-redesign failures (person never actually needed the feature), mark the operationalisation as weak. Commit to building a scoring rubric before claiming inter-rater reliability. The plane is original and useful; the severity axes need calibration.

---

### 4. Limits-of-operationalization file is documentation, not a model contribution

**What prior frameworks do:** TAM, Rogers, TTM, and Gartner Hype Cycle do not distinguish between empirically tested claims and conjectures. They present themselves as grounded without specifying the grounding method or data.

**What V6 adds:** An explicit file separating snapshot-observable claims (S0 vs engaged, S6E vs S7B by usage volume) from longitudinal-only claims (S2T vs S2D requires asymmetric updating signal) from currently-conjecture claims (cultural variability, S6 coexistence patterns, "most people cycle multiple times").

**The contribution is hygiene, not substance.** V6 does not make *fewer* unsupported claims than V5; it makes the same claims and then documents which ones lack support. This is transparency, not innovation.

**The file has high value for practitioners** — it prevents misuse (e.g., trying to diagnose S7I Identity Expansion from a single conversation). But it does not add to the model's explanatory power.

**Fix:** Rename internally from "V6 original contribution" to "V6 quality gate." Keep the file. In the comparative review, give it credit for honesty, not for novelty. The fact that prior frameworks *lack* this kind of transparency does not make V6 novel; it makes prior frameworks worse.

---

### 5. Per-domain identity-stakes scoping is V6's most defensible original claim

**What prior frameworks do:** All five (TAM, Rogers, TTM, Gartner, even pre-V6 versions of this model) treat adoption as a *person-level* phenomenon. A person either adopts or doesn't. Rogers describes distribution across populations; TTM describes a person's progression through stages toward a goal; TAM predicts adoption likelihood. None of them contemplate that the same person could be in *radically different psychological states for different domains at the same time*.

**What V6 adds:** The explicit claim that Identity Stakes is per-domain, not per-person. The same person can be:
- S3B Bargaining (negotiating scope) in their core domain (software engineering)
- S7M Maturity (reflective, integrated use) in a secondary domain (writing)
- S5 Understanding (calm, bounded delegation) in a tertiary domain (scheduling)
- S0 Baseline (non-user) in another domain (visual design)

All on the same day. And within each domain, Task Delegation Level modulates the intensity independently.

**This is not in any prior framework.** Rogers assumes population heterogeneity (some people are early adopters, others laggards) but not individual multi-domain heterogeneity. TTM assumes a single behavior-change trajectory per person. TAM predicts adoption likelihood for "the innovation," not for domain-specific variants of it. Gartner Hype Cycle is purely population-level. The Transtheoretical Model's stages apply to a single behavior (e.g., smoking cessation), not to different domains of the same behavior.

**Operationally, this is falsifiable:** Observe whether the same person shows different state-signatures in different domains (e.g., high usage + uncritical in one domain, low usage + doubting in another). Predict: the person is in S6E in one domain, S6D in another. Confounds: domain-specific expertise differences (they genuinely have higher skill in one domain so lower fear), tool-specific differences (different tool in each domain), time-in-domain effects (one domain is newer so higher resistance is just a recency effect).

**Fix:** Keep per-domain Identity Stakes as V6's signature original contribution. Make it even more explicit in the main model prose. Add a worked example: "Sophia is S7M in email and scheduling (tools that don't threaten her identity), S3B in data analysis (her craft is being replicated but she is negotiating boundaries), and S2D in creative writing (high identity stakes and she is still in defensive evaluation)."

---

### 6. S3X Structural Displacement is an original state addressing a gap in all five prior frameworks

**What prior frameworks do:** TAM, Rogers, TTM, Gartner, and prior versions of this model treat the problem as *psychological adaptation to a new tool or capability*. They assume the person has a viable pathway forward if they can just get psychologically ready.

**What they miss:** Some AI capabilities create economic non-viability that is *structural, not psychological*. A translator whose language pair is being natively translated by AI has no viable "integrated AI-collaborative translation practice" in that pair, even if their psychology eventually stops resisting. The role simply ceases to exist.

**What V6 adds:** S3X as a distinct state reached from S3E Ego Shock when the person concludes economic non-viability. It is not a dropout (which implies prior engagement and then disengagement); it is a branching point where identity-replication threat meets economic reality and the two are no longer separable.

V6 does not solve the S3X problem — it correctly says "this is no longer a psychology problem, it is an economic one." But by naming the state and giving it a branch off S3E, V6 acknowledges that TTM's "relapse-is-normal" framing and TAM's "adoption is the goal" framing both fail for structurally displaced workers.

**Operationally:** S3X is identifiable by a marker: the person has concluded that their domain no longer supports their prior role, even in hybrid form. This is testable via self-report ("Is there any version of your role that still exists in this field that you would want to do?"). If the answer is "no, the role is gone," S3X is in play.

**The limitation:** V6 does not specify what practitioners do with S3X. The model correctly implies "advocacy and reskilling are outside this framework's scope." But that is a limitation, not a weakness — the framework is not designed to solve structural economic problems.

**Fix:** Keep S3X. Expand the state file to clarify: S3X is not a failure of the adaptation model; it is the point where the adaptation model correctly stops. Cross-link to [populations.md](populations.md) and external reskilling resources. Do not oversell V6's utility for S3X; do credit it for naming the state.

---

### 7. PEN Pre-emptive Non-Adoption is novel and fills a gap, but only for knowledge-work domains where ethical objection is possible

**What prior frameworks do:** TAM asks "will they adopt?" based on usefulness and ease-of-use. Rogers predicts position on the adoption curve based on innovativeness traits. TTM describes relapse risk. Gartner tracks technology maturity. None of them distinguish between "I didn't adopt because I'm not convinced it works" and "I won't adopt because I have an ethical objection before testing."

**What V6 adds:** PEN Pre-emptive Non-Adoption as a state reachable from S1 Initial Encounter. The person is exposed to AI, understands its capabilities, and chooses not to engage *because of a values commitment* — not because they doubt usefulness or ease-of-use, but because they have a prior commitment (AI is environmentally destructive, AI labor is exploitative, AI-generated content violates my creative ethics, using AI in my craft is cheating).

This is borrowed from ethics literature (ethical non-consumption, values-driven refusal) but is new to adoption frameworks. The prior frameworks have no concept of "ethical objection at first encounter."

**The distinctiveness from S2D:** Both avoid engagement. But:
- S2D Defensive Resistance enters after the person understands their skill is being replicated. The resistance is reactive ("this threatens my identity").
- PEN Pre-emptive Non-Adoption enters before the person has tested the tool in their own practice. The refusal is values-grounded ("I don't use AI because of [principle]").

V6 claims these are distinguishable by cross-domain consistency, evidence response, and emotional register. A S2D person will gladly use AI for low-stakes domains (email, scheduling) and resist only high-stakes domains. A PEN person will refuse across domains ("I don't use AI at all"). A S2D person will reconsider if the tool demonstrably doesn't replicate their skill. A PEN person will hold the line even if the tool is weak (they don't want to use strong AI either).

**Operationally:** This is testable via self-report and cross-domain behavioral observation. Ask the person: "Why don't you use AI?" If the answer is values-driven and consistent across domains, PEN is in play. If the answer is domain-specific ("I use it for email but not for [core work]"), S2D is in play.

**The limitation:** This distinction is only load-bearing for knowledge workers who have *explicitly chosen not to use* AI. A person who has never encountered AI is not PEN; they are S0 Baseline. A person who encountered AI, engaged with it, and then rejected it is dropout, not PEN.

**Fix:** Keep PEN. Clarify in the state file that it applies only to people who made a values-grounded decision *at* first encounter, not people who defaulted to non-use. In [populations.md](populations.md), note that PEN coverage is limited to domains where ethical choice is salient (creative work, knowledge work, research). It does not apply equally to service work or manual work where ethical choice about AI use is not a available option.

---

### 8. S2T → S2D edge adds complexity without evidence that it improves the model

**What the edge claims:** During testing phase (S2T Trust Evaluation), if the person discovers a threat they didn't expect at S1, they can move to S2D Defensive Resistance even though they entered S2T (low-stakes, cooperatively testing). Example: person enters S2T with low stakes (AI might be useful for email), but during testing discovers that the AI is also being applied to their core work (high-stakes replicate-threat surfaces), triggering a move to S2D.

**The mechanism is plausible.** The person's perception of stakes changed; stakes drive the fork at S1, so re-calculating stakes can re-fork the path. But:

- This edge is marked **[Testable]** in the model, requiring longitudinal observation of updated threat perception. No data yet distinguishes "person was always high-stakes and entered S2D directly" from "person entered S2T and re-evaluated to S2D."
- The new edge collapses the S2T/S2D distinction into a false dichotomy. If S2T can become S2D, then the fork is not a binary choice at S1; it is a trajectory that can reverse. If S2D can become S2T (which the model does not claim), the distinction between defensive and evaluative is not about the moment of entry but about threat timeline.

**Against the edge:** It is added because a small fraction of users seem to evaluate the tool cooperatively, then encounter threat, then resist. But most users enter as S2T and stay, or enter as S2D and stay. The edge covers an edge case. Including it makes the model more complex (more edges, more state pairs to track) without evidence that the added complexity helps practitioners identify users or intervene better.

**For the edge:** Practitioners report that some people's threat perception does change during testing. Naming the transition (S2T → S2D) makes that pattern discussable.

**Fix:** Keep the edge, but mark it **[Rare]** and move the operationalisation requirement to [limits-of-operationalization.md](limits-of-operationalization.md). Do not treat it as a standard transition. Document: "This edge is observed but operationalisation is unclear. If you see it in a user, flag it as a research observation, not a model inference."

---

### 9. The direct S3E → S5 edge is theoretically possible but unverified; recommend removing it until evidence exists

**What the edge claims:** Some people move directly from S3E Ego Shock (experiencing self-efficacy collapse and identity threat after capability exposure) to S5 Understanding (calm, integrated, bounded delegation) without the negotiation phase (S3B Bargaining).

**The mechanism is implausible.** S3E is defined as the state where the person's sense of competence is shattered and identity is threatened. S5 is defined as the state where the person has reframed their sense of competence (they have a role alongside AI, not in place of AI) and accepted bounded delegation. The gap between "I cannot do this, my identity is threatened" and "I am now integrated and calm" without any negotiation is a category jump.

**The justification in the model:** V6 notes this is rare and marked **[Testable]**, distinguishing it from S3E → S3B → S5 (which looks the same in short time windows). The distinction requires longitudinal observation; on a single snapshot, both paths are indistinguishable.

**The problem:** If a path is empirically indistinguishable from another path, including it in the model increases complexity without increasing explanatory power. A parsimonious model should remove edges that cannot be falsified in practice.

**The observed reality:** What practitioners call "direct S3E → S5" is almost always "accelerated S3E → S3B → S5" where the person cycled through S3B in a matter of hours or days (in a single conversation, in a single day). The model cannot distinguish these because the timescale is too compressed.

**Fix:** Remove the direct S3E → S5 edge from the main graph. Relegate it to a footnote in [02-state-graph.md](02-state-graph.md): "Theoretically possible; empirically indistinguishable from accelerated S3E → S3B → S5. Include only if longitudinal data demonstrates the direct path exists. Until then, assume S3B is always in play."

---

### 10. Comparison verdict: V6 adds genuine structure to TAM/Rogers/TTM, not just vocabulary

**V6 against TAM (Davis 1989):** V6 is not a replacement; it is a downstream extension. TAM predicts adoption likelihood (perceived usefulness + perceived ease-of-use). V6 assumes adoption has happened and asks: what is the person's psychological state now? What is the intensity of their struggle? How do identity stakes and delegation level modulate their experience? V6 is compatible with TAM; it picks up where TAM stops. **Verdict: Use TAM to predict whether adoption will happen; use V6 to understand the person's psychology after adoption.**

**V6 against Rogers (Diffusion of Innovations):** Rogers is population-level; V6 is individual-level. Rogers describes distribution of innovativeness traits (early adopters, early majority, late majority, laggards) and predicts S-curve adoption. V6 describes one person's trajectory through states, across multiple domains, at varying intensities. The two frameworks are orthogonal — they describe different phenomena at different levels. **Verdict: Use Rogers to understand the *population distribution* of adopters; use V6 to understand one adopter's *internal state* over time.**

**V6 against TTM (Stages of Change):** TTM describes behavior change toward a goal (pre-contemplation → contemplation → preparation → action → maintenance, with relapse possible). V6 describes stable states that are not motivational stages toward a single goal. Someone in S3B Bargaining or S6E Enthusiastic Overuse may never progress further; they may be stable there. TTM assumes progression is the goal; V6 assumes description is the goal. **Verdict: Use TTM if the goal is behavior change (smoking cessation, exercise adoption); use V6 if the goal is understanding where someone is and why they're there.**

**V6 against Gartner Hype Cycle:** Gartner describes a technology's population-level maturity (Peak of Inflated Expectations → Trough of Disillusionment → Slope of Enlightenment → Plateau of Productivity). V6 describes individual-level psychology. Gartner is useful for understanding whether a technology is in the hype phase (expect volatility) or mature phase (expect stability); V6 is useful for understanding why a specific person is struggling with the technology. The two could be used together: "The technology is in the Trough of Disillusionment (Gartner); this person is in S3E Ego Shock (V6)." **Verdict: Use Gartner for technology adoption strategy; use V6 for user support and psychology.**

**V6 against Kübler-Ross (Stages of Grief):** Kübler-Ross describes a single psychological process (denial → anger → bargaining → depression → acceptance) through loss. V6 borrows the "bargaining and cycling are normal" framing but abandons the linear stage model and the grief-specific language. S3B Bargaining is not grief bargaining (making deals with God); it is identity-protective bargaining (negotiating scope, boundaries, conditions of use). **Verdict: Kübler-Ross applies to genuine loss situations (someone's role is being eliminated, not transformed). V6 applies when the person's role *can* be transformed but they are struggling with identity threat during the transformation.**

---

## Recommendations — Priority Order

### Priority 1: Retain the two-axis modulation (Identity Stakes × Task Delegation Level)

This is genuinely original, operationalisable, and load-bearing across all of V6. It appears in no prior framework. Test it against TAM and Rogers by measuring user intensity/affect as a function of these two axes. Example study: 40 users across two AI capability jumps, high-stakes vs low-stakes domains, D1 vs D4 interactions. Cost: $50k. Timeline: 6 months.

### Priority 2: Retain per-domain identity-stakes scoping

This is the second most defensible original claim. Make it even more explicit in Model6.md. Add a section "Multi-domain coexistence" with worked examples. Document that a user's state in one domain does not predict their state in another.

### Priority 3: Retain S3X Structural Displacement

It addresses a real gap in TAM, Rogers, and TTM (they have no concept of structural non-viability). Keep it; do not oversell V6's utility for solving S3X. Cross-link to external reskilling resources.

### Priority 4: Retain PEN Pre-emptive Non-Adoption, but narrow its scope

PEN fills a gap (ethical refusal at first encounter) that no prior model addresses. But clarify in the state file that it applies only to people who made an explicit values-grounded decision at first encounter, and that it is most salient in knowledge-work and creative domains.

### Priority 5: Keep the practical × emotional dropout plane, but operationalise it more rigorously

The reversibility test is a good start. Commit to building a scoring rubric so two raters can agree within ±1 on severity. Study: 50 people who dropped out; apply the reversibility test; measure agreement with self-report. Cost: $20k. Timeline: 3 months.

### Priority 6: Remove or defer the direct S3E → S5 edge

It is theoretically possible but empirically indistinguishable from accelerated S3E → S3B → S5. Remove it from the main graph. Include in a footnote: "Possible; unverified. Include in V7 if longitudinal data demonstrates it."

### Priority 7: Demote limits-of-operationalization.md from "model contribution" to "quality gate"

It is good documentation, not a novel theoretical contribution. Keep it. Market it as "transparency about what we don't know" rather than "original V6 contribution."

### Priority 8: Mark the S2T → S2D edge [Rare] and operationalisation-unclear

It covers a real but infrequent transition. Document it; do not treat it as a standard path.

### Priority 9: Rename S6/S7 state names, do not claim they are original

S6E/S6D/S6R/S6S are useful vocabulary-level refinements of Rogers. Keep the names; credit Rogers. S7M/S7I/S7E/S7B/S7V are refinements of TTM maintenance modes. Keep them; credit TTM.

### Priority 10: Benchmark V6 against each prior framework in a single study

Design a mixed-method study observing 60 users across AI capability jumps. For each user, code their progression using TAM (adoption likelihood), Rogers (adopter category), TTM (stage of change), V6 (state + intensity). Measure which framework is most predictive of:
- Sustained use past 6 months
- Usage intensity (D-level of interactions)
- Dropout risk
- Ability to identify a user's state from a single conversation

Cost: $150k. Timeline: 12 months. This tells you whether V6 actually adds explanatory power or is just renamed prior models.

---

## Open Questions — Not Resolved by This Comparative Review

1. **Is the per-domain scoping actually how people experience AI, or is it a conceptual convenience?** Do users genuinely partition their identity-stakes by domain, or is the model imposing a partition that doesn't match lived experience?
2. **Does V6's emphasis on descriptive-first stance make it less useful for intervention?** If the model is explicitly non-prescriptive, does that limit its utility for practitioners trying to help people move from S3E to S5?
3. **How does V6 handle domain-transfer?** Someone in S7M Maturity in one domain who encounters a new AI capability in a new domain — do they re-enter at S1 or do they carry their integration forward?
4. **Is the Delegation Ceiling a person-level property or a domain-level property?** V6 says per-person with per-domain variation; the model could be clearer.

---

## Summary of Novelty Claims

| V6 Claim | Novel? | Testable? | Recommendation |
| --- | --- | --- | --- |
| Two-axis modulation (Stakes × Delegation) | **YES** | Yes | Keep. Priority 1. Test ASAP. |
| Per-domain identity-stakes scoping | **YES** | Yes | Keep. Priority 2. Expand documentation. |
| S3X Structural Displacement | **YES** (as graph state) | Yes | Keep. Priority 3. Do not oversell utility. |
| PEN Pre-emptive Non-Adoption | **YES** (in adoption models) | Yes | Keep. Priority 4. Narrow scope. |
| Practical × emotional dropout plane | Partial (plane is; severity is not) | Partially | Keep. Priority 5. Build scoring rubric. |
| S6 four-way split | **NO** (vocabulary refinement of Rogers) | Yes | Keep names; credit Rogers. Priority 9. |
| S7 split | **NO** (vocabulary refinement of TTM) | Yes | Keep names; credit TTM. Priority 9. |
| Direct S3E → S5 edge | Theoretical but unverified | No (indistinguishable from S3B) | Remove. Priority 6. |
| S2T → S2D edge | Plausible but infrequent | Unclear | Mark [Rare]. Priority 8. |
| Descriptive-first stance | **NO** (framing improvement, not substance) | N/A | Keep as hygiene; do not market as innovation. Priority 7. |
| Limits-of-operationalization file | **NO** (documentation) | N/A | Market as transparency, not novelty. Priority 7. |

---

## Final Verdict

**V6 is a real advance over TAM, Rogers, TTM, Gartner, and Kübler-Ross on two dimensions: the two-axis modulation of intensity within states, and the per-domain identity-stakes scoping.** These two additions are load-bearing and operationalisable.

**The new states (S3X, PEN) are original and fill real gaps in prior frameworks.** They belong in V6.

**The documentation improvements (limits-of-operationalization.md, descriptive-first stance) are good hygiene but not theoretical novelty.** They prevent misuse but do not advance the model's explanatory power.

**The S6/S7 state splits are vocabulary-level refinements of Rogers and TTM, useful for knowledge-work AI specifically but not mechanically new.**

**Before V7, test the two-axis modulation against the five prior frameworks in a single study. The data will tell you whether V6 is a genuine extension or a repackaging.**