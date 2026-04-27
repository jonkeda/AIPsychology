This is a simpler rewrite of [008-comparative.md](008-comparative.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# 008 — V6 Against Prior Frameworks (Plain Language)

## What this review is about

V6 doesn't exist in a vacuum. There are five earlier frameworks that cover related ground: TAM, Rogers, TTM, the Gartner Hype Cycle, and Kübler-Ross. This review asks: what does V6 actually add? What does it borrow without credit? What should be cut?

**Quick definitions for the five prior frameworks:**
- **TAM** (Technology Acceptance Model, Davis 1989) — predicts whether someone will adopt a new tool based on two factors: does it seem useful, and does it seem easy to use?
- **Rogers** (Diffusion of Innovations) — describes how new ideas spread through a population. Labels people as early adopters, early majority, late majority, and laggards.
- **TTM** (Transtheoretical Model, also called Stages of Change) — psychology model of behavior change. Describes stages from "not thinking about it" through "actively changing" to "maintaining the change." Originally built for things like quitting smoking.
- **Gartner Hype Cycle** — industry analyst's chart of how a technology gets overhyped, crashes into disillusionment, and eventually finds its real level of usefulness. A population-level view of a technology's reputation over time.
- **Kübler-Ross** (Stages of Grief) — denial, anger, bargaining, depression, acceptance. Originally for people dealing with terminal illness. Often borrowed loosely for any major change.

## TL;DR

- **The two-axis intensity system (Identity Stakes × Task Delegation Level) is genuinely new.** No prior framework varies how intense someone's struggle feels depending on how much of their identity is at stake and how much they're handing off to the AI. This is load-bearing and testable.
- **Per-domain state scoping is V6's strongest original claim.** The same person can be in completely different psychological states for different uses of AI at the same time. No prior model allows this.
- **S3X Structural Displacement and PEN Pre-emptive Non-Adoption are real gaps in prior work.** S3X names the situation where a role doesn't just change — it disappears economically, and psychology can't fix that. PEN names the situation where someone refuses AI on values grounds before ever testing it.
- **The S6 and S7 sub-states are useful vocabulary, but they're not new discoveries.** S6E/S6D/S6R/S6S are Rogers' adopter categories with new labels. S7 sub-states are refinements of TTM's maintenance phase. Keep the names; credit the sources.
- **The practical × emotional dropout plane is original and useful, but the severity scale needs calibration.** Right now two people scoring the same dropout case won't agree on the numbers.
- **The limits-of-operationalization file is honest documentation, not a theoretical contribution.** Prior frameworks don't distinguish between tested claims and guesses. V6 does. That's good hygiene, not a new idea.
- **V6 is a real advance over all five prior frameworks on intensity and per-domain scoping.** The new states (S3X, PEN) belong. The documentation improvements prevent misuse. The S6/S7 vocabulary is useful for knowledge-work AI but not structurally new. Before V7, test the two-axis system against the five prior frameworks in a single study. That data will tell you whether V6 is a genuine extension or a repackage.

---

## Findings

### 1. The two-axis intensity system is genuinely new — testable against all five prior frameworks

**What V6 borrows:** The idea that people move through states or stages. TAM uses usefulness + ease-of-use to predict adoption. Rogers uses compatibility with existing practice. TTM uses discrete stages. The Gartner Hype Cycle tracks a technology's maturity arc.

**What V6 adds:** None of those frameworks vary *how intense* someone's experience is within a state. TAM predicts *whether* someone adopts. V6 predicts *how hard they struggle* in S3E Ego Shock or S6E Enthusiastic Overuse depending on (a) how much of their professional identity rides on this domain, and (b) how much cognitive work they're handing to the AI.

This produces two new predictions no prior framework makes:
- The same person in the same state feels it differently when the stakes change. A translator in S2D Defensive Resistance feels it harder than someone using AI to plan travel.
- The same person, same domain, same day experiences different intensity for different interactions. Asking an AI "what does this word mean" produces no emotional reaction. Handing the AI an autonomous task in your core skill triggers the full S3E response if stakes are high.

**The claim is testable.** Compare people using AI for high-identity-stakes work (translation, code review, medical diagnosis) against low-stakes use (summarizing emails, scheduling). Measure emotional affect, hesitation, error-checking behavior. Prediction: high-stakes use correlates with more resistance and stronger reaction in shock states. Low-stakes use skips the resistance states entirely. Things that could confound the test: prior exposure, general anxiety, workplace culture.

**None of the five prior frameworks has this.** TAM's usefulness and ease-of-use are factors in whether you adopt — not modulators of intensity after you've adopted. Rogers has compatibility, but doesn't break it into "how much of my identity rides on this" versus "how much am I delegating." TTM's stages don't get more intense based on stakes. The Gartner Hype Cycle is population-level — it has no concept of individual intensity variation at all.

**Fix:** Keep the two-axis system as V6's primary original claim. Test it before the next major revision. The study design exists: measure affect, hesitation, error-checking, and delegation reluctance with same-person comparisons across high-stakes and low-stakes domains, and across D1 (information query) versus D4 (autonomous partnership) interactions.

---

### 2. The S6 four-way split is a vocabulary-level refinement of Rogers' adopter categories, not a structural discovery

**What V6 borrows:** Rogers describes distinct attitudes toward new technology across a population. Early adopters are curious and willing to accept risk. The early majority are deliberate. The late majority are skeptical. Laggards are tradition-bound and suspicious. V6's S6 sub-states map directly onto this: S6E Enthusiastic (early adopter attitude), S6D Dependent (early majority who adopt but doubt themselves), S6R Driven (late majority conforming to pressure), S6S Social (group-norming behavior).

**What V6 adds:** The labels are clearer for knowledge-work AI specifically. The coexistence rules add some precision — S6E and S6D can't both be true at once; S6R and S6S can coexist in high-pressure workplaces. But this is refining a taxonomy that already existed, not building a new one.

There is one genuine conceptual shift: Rogers describes the *distribution* of attitudes across a population at a point in time. V6 applies those categories to one person's *path over time* — the same person moves from S6E to S6D to S7B. Rogers doesn't forbid this, but he never described it either.

**The practical problem:** S6E and S6D both look like "person uses the tool a lot." Telling them apart requires either following the person over time or asking them directly. A single snapshot can't separate the two. The original review flags this in [limits-of-operationalization.md](limits-of-operationalization.md).

**Fix:** Rename this internally from "original S6 split" to "taxonomy refinement." Credit Rogers explicitly in the S6 state files for the psychological mechanisms (early-adopter enthusiasm, conformity pressure, self-doubt in innovation integration). Keep the four states because they're useful for practitioners. Drop any implication that they're mechanically new.

---

### 3. The practical × emotional dropout plane is original and testable, but only via the reversibility test, and only in clean cases

**What prior frameworks do with dropout:** TAM, Rogers, TTM, and Gartner all treat dropout as a single failure state. They ask whether someone quit. They don't ask what internal process drove the exit.

**What V6 adds:** A two-axis way to distinguish dropout types:
- **High practical / low emotional:** the tool was bad. The user says "the output was wrong" and means it. Fix: better tool, better training, better defaults.
- **High emotional / low practical:** identity threat or exhaustion. The user says "it was too stressful." Fix: psychological support, gradual re-exposure, social reframing.
- **High practical + high emotional:** mixed. The user cites a tool failure but would have tolerated it if the identity threat were lower. Fix the tool first to remove the excuse, then address the emotional layer.
- **Low practical + low emotional:** indifference or opportunity cost. Probably not worth intervening.

This is new in adoption frameworks. Rogers, TAM, and TTM don't separate tool failure from psychological failure.

**How the reversibility test works:** Offer the user a tool that actually solves their stated complaint. If they come back, practical friction was the real driver. If they don't, something deeper was going on. This works well when the cited complaint is specific and tool-fixable.

**Where it breaks:**
- The "tool failure" was actually workflow friction — the person never needed that feature in the first place. Offering a better summarizer doesn't help if they never needed summaries.
- The emotional and practical failures happened in one event. The person's first AI-generated email was both bad *and* made them feel like their voice had been copied. The two can't be separated.
- The emotional cost built up over time. Burnout from months of over-delegating doesn't go away when you swap the tool.

**What's still a guess:** The 0–10 severity axis isn't calibrated. Two people scoring the same dropout case will not reliably agree on the numbers without a shared scoring guide.

**Fix:** Keep the two-axis plane and the reversibility test. Document that the test is most reliable for single-incident dropouts with a specific, fixable tool complaint. For long-term burnout cases or workflow-mismatch cases, mark the test as unreliable. Build a scoring guide before claiming that two raters will agree.

---

### 4. The limits-of-operationalization file is good documentation, not a model contribution

**What prior frameworks do:** TAM, Rogers, TTM, and the Gartner Hype Cycle don't separate their tested claims from their guesses. They present as grounded without specifying what grounds them.

**What V6 adds:** An explicit file that separates what you can see in a snapshot (S0 versus engaged; S6E versus S7B by usage volume) from what requires following someone over time (S2T versus S2D requires seeing how they update when new information arrives) from what's currently just a guess (cultural variability, coexistence patterns, "most people cycle multiple times").

**The honest assessment:** This is transparency, not innovation. V6 makes the same number of unsupported claims as earlier versions. It just now admits which ones lack evidence. That's a good quality gate. It prevents someone from trying to diagnose S7I Identity Expansion from a single conversation. But it doesn't change what the model actually claims.

**Fix:** Keep the file. In the comparative review, credit it for honesty, not for novelty. The fact that prior frameworks don't have this kind of transparency makes them worse — it doesn't make V6 more theoretically powerful.

---

### 5. Per-domain identity-stakes scoping is V6's most defensible original claim

**What prior frameworks do:** All five frameworks treat adoption as something that happens at the person level. A person either adopts or doesn't. Rogers describes population distributions. TTM describes a single person's progression toward a single behavior-change goal. TAM predicts adoption likelihood for a tool. None of them contemplate the same person being in radically different psychological states for different uses of AI at the same time.

**What V6 adds:** Identity Stakes is per-domain, not per-person. The same person can be:
- S3B Bargaining (negotiating scope) for AI use in their core domain (such as software engineering)
- S7M Maturity (calm, integrated use) in a secondary domain (such as writing)
- S5 Understanding (bounded delegation, no anxiety) for scheduling
- S0 Baseline (non-user) for visual design

All on the same day. And within each domain, Task Delegation Level modulates the intensity independently.

**No prior framework has this.** Rogers assumes population heterogeneity (some people are early adopters, others aren't) but not that one person can simultaneously be an "early adopter" in one domain and a "laggard" in another. TTM assumes a single behavior-change trajectory per person. TAM predicts adoption for "the tool," not for domain-specific variants of it. The Gartner Hype Cycle is purely population-level.

**The claim is testable:** Observe whether the same person shows different state-signatures in different domains — high usage and uncritical in one domain, low usage and doubting in another. Predict: the person is in S6E in one domain, S6D in another. Things that could confound the test: genuine skill differences across domains (lower fear in one domain because they're actually better at it), different tools in different domains, one domain being newer so higher resistance is just a recency effect.

**Fix:** Keep per-domain Identity Stakes as V6's signature original contribution. Make it more explicit in the main model documentation. Add a worked example: "Sophia is S7M in email and scheduling (tools that don't threaten her identity), S3B in data analysis (her craft is being replicated but she's negotiating limits), and S2D in creative writing (high identity stakes, still in defensive evaluation)."

---

### 6. S3X Structural Displacement is an original state that fills a gap in all five prior frameworks

**What prior frameworks assume:** TAM, Rogers, TTM, Gartner, and earlier versions of this model all treat the problem as *psychological adaptation to a new tool*. They assume there's a viable path forward if the person can just get past the psychological friction.

**What they miss:** Some AI capabilities create a situation where there is no viable path forward. A translator whose language pair is being handled natively by AI doesn't have a "hybrid AI-collaborative translation practice" to reach, even if their psychology stops resisting. The role simply ceases to exist economically.

**What V6 adds:** S3X as a distinct state that branches off from S3E Ego Shock when the person concludes the role is economically gone. It's not dropout — dropout means someone engaged and then quit. S3X is a branch point where psychological threat and economic reality are the same thing, and psychology alone can't solve it.

V6 doesn't claim to solve S3X. It correctly says "this is now an economic problem, not a psychology problem." But by naming the state and giving it a branch off S3E, V6 acknowledges that TTM's "relapse is normal, keep trying" framing and TAM's "adoption is the goal" framing both fail for workers whose roles are being eliminated.

**The test:** S3X is identifiable by a single question: "Is there any version of your role that still exists in this field that you would want to do?" If the answer is "no, the role is gone," S3X is in play.

**The limitation:** V6 doesn't specify what practitioners do with S3X. The model correctly implies that advocacy and reskilling are outside its scope. That's a limitation, not a weakness — it's not designed to solve structural economic problems.

**Fix:** Keep S3X. Expand the state file to clarify that S3X is not a failure of the adaptation model — it's the point where the adaptation model correctly stops. Link to [populations.md](populations.md) and external reskilling resources. Don't oversell V6's utility here; do credit it for naming the state.

---

### 7. PEN Pre-emptive Non-Adoption is a new concept in adoption frameworks, but it only applies in knowledge-work and creative domains

**What prior frameworks do:** TAM asks "will they adopt?" based on perceived usefulness and ease-of-use. Rogers predicts where someone sits on the adoption curve based on their innovativeness traits. TTM describes relapse risk. Gartner tracks technology maturity. None of them distinguish between "I didn't adopt because I'm not convinced it works" and "I won't adopt because I have an ethical objection before testing."

**What V6 adds:** PEN Pre-emptive Non-Adoption — a state reachable from S1 Initial Encounter, where the person understands the AI's capabilities and chooses not to engage *because of a values commitment*. Not because they doubt usefulness. Not because it's hard to use. Because they have a prior principle: AI is environmentally harmful, AI labor is exploitative, AI-generated content violates creative ethics, using AI in their craft feels like cheating.

This is borrowed from ethics literature (ethical non-consumption, values-driven refusal) but it's new in adoption frameworks.

**How PEN differs from S2D Defensive Resistance:**
- S2D enters after the person understands their skill is being replicated. The resistance is reactive — "this threatens my identity."
- PEN enters *before* the person has tested the tool in their own practice. The refusal is values-grounded — "I don't use AI because of [principle]."

V6 claims these are distinguishable three ways:
1. Cross-domain consistency: a PEN person refuses across all domains. An S2D person uses AI for low-stakes things (email, scheduling) and resists only their core work.
2. Evidence response: an S2D person will reconsider if the tool demonstrably doesn't replicate their skill. A PEN person won't, even if the tool is weak — they don't want to use strong AI either.
3. Emotional register: S2D is anxious. PEN is principled.

**The test:** Ask the person why they don't use AI. If the answer is values-driven and consistent across domains, PEN is in play. If the answer is domain-specific, S2D is in play.

**The limitation:** PEN only applies to people who made a deliberate values-grounded decision at first encounter. Someone who has never encountered AI is not PEN — they're S0 Baseline. Someone who tried AI, engaged with it, and later rejected it is a dropout, not PEN.

**Fix:** Keep PEN. Clarify in the state file that it applies only to people who made an explicit values-grounded decision at first encounter — not people who defaulted to non-use. In [populations.md](populations.md), note that PEN is most relevant for creative and knowledge work, where ethical choice about AI use is a real option. It doesn't apply equally in service or manual work where workers typically don't get to choose.

---

### 8. The S2T → S2D edge is plausible but rare; don't treat it as a standard path

**What the edge claims:** Someone can enter S2T Trust Evaluation (cooperatively testing the tool, low stakes) and later move to S2D Defensive Resistance. This happens when, during testing, the person discovers the AI is also being applied to their core high-stakes work — stakes they didn't realize were in play when they started testing. Their threat perception updates, and so does their state.

**The mechanism is plausible.** The fork between S2T and S2D happens at S1 based on perceived stakes. If stakes are re-evaluated, the fork can re-run. But:

- This edge is marked testable in the model, and no data yet distinguishes "person was always high-stakes and entered S2D directly" from "person entered S2T and re-evaluated to S2D."
- If S2T can become S2D, the fork at S1 isn't a clean binary — it's a trajectory that can reverse. The model doesn't claim S2D can become S2T, so this is a one-way special-case edge, not a symmetric pair. That asymmetry needs to be explicit.
- Most users enter S2T and stay, or enter S2D and stay. This edge covers a small minority.

**The case for keeping it:** Practitioners report that some people's threat perception does shift during testing. Naming the S2T → S2D transition makes that pattern discussable rather than invisible.

**Fix:** Keep the edge. Mark it **[Rare]** and move the operationalization requirement to [limits-of-operationalization.md](limits-of-operationalization.md). Don't treat it as a standard transition. Document: "This edge is observed but the test to confirm it is unclear. If you see it in a user, treat it as a research observation, not a model inference."

---

### 9. The direct S3E → S5 edge should be removed until there's evidence for it

**What the edge claims:** Some people move directly from S3E Ego Shock (confidence shattered, identity threatened after seeing what AI can do) to S5 Understanding (calm, integrated, bounded delegation) without going through S3B Bargaining (negotiating limits and scope).

**The mechanism is implausible.** S3E is defined as the state where the person's sense of competence has collapsed. S5 is defined as the state where the person has rebuilt their sense of competence in a new frame (they have a role *alongside* AI, not *instead of* AI) and accepted bounded delegation. Getting from "I feel like my skills are worthless" to "I've found my place and I'm calm about it" without any negotiation is a category jump, not a small step.

**The model's justification:** V6 marks the edge as testable and distinguishes it from the normal path (S3E → S3B → S5) but acknowledges the two are indistinguishable in short time windows.

**The problem:** If a path is empirically indistinguishable from another path, including it adds complexity without adding explanatory power. A well-built model should cut edges that can't be falsified in practice.

**What practitioners actually observe:** What looks like "direct S3E → S5" is almost always accelerated S3E → S3B → S5, where the person cycled through S3B in hours or days — possibly in a single conversation. The model can't distinguish these because the timescale is too compressed.

**Fix:** Remove the direct S3E → S5 edge from the main graph. Move it to a footnote in [02-state-graph.md](02-state-graph.md): "Theoretically possible; empirically indistinguishable from accelerated S3E → S3B → S5. Include only if longitudinal data demonstrates the direct path exists. Until then, assume S3B is always in play."

---

### 10. V6 is a genuine extension of the prior frameworks, not just a vocabulary rename

**V6 vs TAM:** V6 is not a replacement — it's a downstream extension. TAM predicts adoption likelihood (perceived usefulness + perceived ease-of-use). V6 assumes adoption has already happened and asks: what is the person's psychological state now? How intense is their struggle? How do identity stakes and delegation level shape their experience? The two frameworks are compatible. **Use TAM to predict whether adoption will happen. Use V6 to understand the person's psychology after adoption.**

**V6 vs Rogers:** Rogers is population-level; V6 is individual-level. Rogers describes the distribution of innovativeness traits across a population and predicts the S-curve shape of adoption over time (slow early uptake, rapid middle growth, gradual saturation). V6 describes one person's path through states, across multiple domains, at varying intensities. They describe different things at different levels. **Use Rogers to understand the distribution of adopters in a population. Use V6 to understand one adopter's internal state over time.**

**V6 vs TTM:** TTM describes behavior change toward a goal — the classic stages are pre-contemplation, contemplation, preparation, action, and maintenance, with relapse possible. V6 describes stable states that aren't motivational stages toward a single goal. Someone in S3B Bargaining or S6E Enthusiastic Overuse may never progress further; they may be stable there. TTM assumes progression is the goal. V6 assumes description is the goal. **Use TTM when the goal is behavior change (quitting smoking, starting exercise). Use V6 when the goal is understanding where someone is and why they're there.**

**V6 vs Gartner Hype Cycle:** The Gartner Hype Cycle describes a technology's population-level maturity: peak of inflated expectations, trough of disillusionment, slope of enlightenment, plateau of productivity. V6 describes individual-level psychology. The two can be used together — "The technology is in the Trough of Disillusionment (Gartner); this specific person is in S3E Ego Shock (V6)." **Use Gartner for technology adoption strategy. Use V6 for user support and psychology.**

**V6 vs Kübler-Ross:** Kübler-Ross describes a single psychological process through loss — denial, anger, bargaining, depression, acceptance. V6 borrows the "cycling and bargaining are normal" framing but abandons the linear stage model and the grief-specific language. S3B Bargaining is not grief bargaining (making deals with a higher power). It is identity-protective bargaining — negotiating the scope, boundaries, and conditions of AI use. **Kübler-Ross applies when something is genuinely lost — for example, when someone's role is being eliminated, not transformed. V6 applies when the person's role can be transformed but they're struggling with identity threat during the transformation.**

---

## Recommendations — Priority Order

### Priority 1: Keep the two-axis intensity system (Identity Stakes × Task Delegation Level)

This is genuinely original, testable, and does essential work throughout V6. It appears in no prior framework. Test it against TAM and Rogers by measuring user intensity and affect as a function of these two axes. Study design: 40 users across two AI capability jumps, high-stakes versus low-stakes domains, D1 versus D4 interactions. Cost: $50k. Timeline: 6 months.

### Priority 2: Keep per-domain identity-stakes scoping

This is the second most defensible original claim. Make it more explicit in Model6.md. Add a section called "Multi-domain coexistence" with worked examples. Document clearly that a user's state in one domain tells you nothing about their state in another.

### Priority 3: Keep S3X Structural Displacement

It addresses a real gap in TAM, Rogers, and TTM — none of them have a concept for "the role is economically gone, not just psychologically difficult." Keep it. Don't oversell V6's utility for solving S3X. Link to external reskilling resources.

### Priority 4: Keep PEN Pre-emptive Non-Adoption, but narrow its scope

PEN fills a gap (ethical refusal at first encounter) that no prior model addresses. Clarify in the state file that it applies only to people who made an explicit values-grounded decision at first encounter, and that it's most relevant in knowledge-work and creative domains.

### Priority 5: Keep the practical × emotional dropout plane, but build a scoring guide

The reversibility test is a good starting point. Commit to building a scoring guide so two raters can agree within ±1 on severity. Study design: 50 dropout cases; apply the reversibility test; measure agreement with self-report. Cost: $20k. Timeline: 3 months.

### Priority 6: Remove the direct S3E → S5 edge

It is theoretically possible but empirically indistinguishable from an accelerated S3E → S3B → S5. Remove it from the main graph. Put it in a footnote: "Possible; unverified. Include in V7 only if longitudinal data demonstrates it."

### Priority 7: Demote limits-of-operationalization.md from "model contribution" to "quality gate"

It's good documentation, not a novel theoretical contribution. Keep it. Market it as "transparency about what we don't know," not as an original V6 contribution.

### Priority 8: Mark the S2T → S2D edge [Rare] and operationalization-unclear

It covers a real but infrequent transition. Document it; don't treat it as a standard path.

### Priority 9: Keep the S6/S7 state names; credit Rogers and TTM

S6E/S6D/S6R/S6S are useful vocabulary-level refinements of Rogers' adopter categories. Keep the names; credit Rogers. The S7 sub-states are refinements of TTM's maintenance phase. Keep them; credit TTM.

### Priority 10: Run a benchmark study comparing V6 against all five prior frameworks

Design a mixed-method study following 60 users across AI capability jumps. For each user, code their progression using TAM (adoption likelihood), Rogers (adopter category), TTM (stage of change), and V6 (state + intensity). Measure which framework is most predictive of: sustained use past 6 months; usage intensity (delegation level of interactions); dropout risk; ability to identify a user's state from a single conversation.

Cost: $150k. Timeline: 12 months. This study tells you whether V6 actually adds explanatory power or is just relabeled prior models.

---

## Open Questions — Not Resolved by This Comparative Review

1. **Is per-domain scoping how people actually experience AI, or is it a conceptual convenience?** Do users genuinely partition their identity stakes by domain, or is the model imposing a partition that doesn't match lived experience?
2. **Does V6's descriptive-first stance make it less useful for intervention?** If the model is explicitly non-prescriptive, does that limit its utility for practitioners trying to help people move from S3E to S5?
3. **How does V6 handle domain transfer?** Someone in S7M Maturity in one domain who encounters a new AI capability in a new domain — do they re-enter at S1, or do they carry their integration forward?
4. **Is the Delegation Ceiling a person-level property or a domain-level property?** V6 says per-person with per-domain variation; the model could be clearer.

---

## Summary of Novelty Claims

| V6 Claim | Novel? | Testable? | Recommendation |
| --- | --- | --- | --- |
| Two-axis intensity (Stakes × Delegation) | **YES** | Yes | Keep. Priority 1. Test ASAP. |
| Per-domain identity-stakes scoping | **YES** | Yes | Keep. Priority 2. Expand documentation. |
| S3X Structural Displacement | **YES** (as a graph state) | Yes | Keep. Priority 3. Don't oversell. |
| PEN Pre-emptive Non-Adoption | **YES** (in adoption models) | Yes | Keep. Priority 4. Narrow scope. |
| Practical × emotional dropout plane | Partial (the plane is; the severity scale isn't) | Partially | Keep. Priority 5. Build scoring guide. |
| S6 four-way split | **NO** (vocabulary refinement of Rogers) | Yes | Keep names; credit Rogers. Priority 9. |
| S7 split | **NO** (vocabulary refinement of TTM) | Yes | Keep names; credit TTM. Priority 9. |
| Direct S3E → S5 edge | Theoretical but unverified | No (indistinguishable from accelerated S3B) | Remove. Priority 6. |
| S2T → S2D edge | Plausible but rare | Unclear | Mark [Rare]. Priority 8. |
| Descriptive-first stance | **NO** (framing improvement, not substance) | N/A | Keep as hygiene; don't market it as innovation. Priority 7. |
| Limits-of-operationalization file | **NO** (documentation) | N/A | Market as transparency, not novelty. Priority 7. |
