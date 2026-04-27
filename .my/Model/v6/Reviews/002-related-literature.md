# Related-Literature Audit — V6

## TL;DR

- V6 renames V5's "Mechanism anchors" to "Related literature" and disclaims causal claims. This is honest — V5 did oversell the mechanisms — but it's also a retreat into vocabulary without substituting alternative causal stories.
- Three of the four related-literature constructs (self-efficacy, variable-reward, metacognitive calibration) are accurately paired with their states. "Terror management" for S3E is a loose fit.
- The related-literature lines do real work within state families (S3E vs S3B, S6E vs S6D/R/S, S7M vs S3B) but are less useful for cross-family discrimination.
- S3E's compound anchor (self-efficacy collapse + terror management) is defensible — the two mechanisms do reinforce each other — but "terror management" is imprecise. Better alternatives exist.
- The vocabulary reframing is genuinely useful for the reader who wants to think through what each state *is*, but does not strengthen the model's predictive or diagnostic claims.

---

## 1. The rename is honest but signals a retreat from causal claims

V5 called them "Mechanism anchors" and used strong causal language: "self-efficacy collapse **under domain-specific capability threat**" and "terror management in the loose sense — **confrontation with one's own replaceability triggers** the same kind of existential discomfort that confrontation with mortality does." The syntax commits to causality: the threat *causes* the collapse; the confrontation *triggers* the discomfort.

V6 calls them "Related literature" and explicitly disclaims: "Borrowed conceptually as vocabulary; self-efficacy collapse is offered as a frame for thinking about S3E, not as a tested cause." Model6.md goes further: "Knowing that S3E Ego Shock is conceptually related to self-efficacy collapse tells the reader what kind of phenomenon S3E belongs to. It does not let anyone diagnose S3E in a person, and it does not commit the model to the claim that self-efficacy collapse is the cause of S3E."

This is **honest**. V5 did present these as causal mechanisms without empirical support, and V6 corrects that. But it is also **a retreat**: it's downgrading the model from "these are the mechanisms" to "these are conceptual vocabularies," without replacing them with alternative causal stories or acknowledging what was lost by dropping the mechanism claims. A reader expecting the V5 "why does S3E happen?" gets a V6 "S3E is conceptually like self-efficacy collapse" instead.

**Fix:** Add a one-paragraph rationale in Model6.md after the "Related literature is conceptual, not diagnostic" section explaining what V5 claimed and why V6 dropped it. Name the tradeoff explicitly: "V5 proposed that self-efficacy collapse *caused* S3E. V6 treats self-efficacy collapse as a conceptual frame that helps name the state, without claiming to know the cause. This makes the model more honest but less explanatory." Readers need to know they are not getting mechanisms in V6, not because the model is humble, but because the mechanisms are not tested.

---

## 2. "Terror management" is a loose fit for S3E; three other constructs are well-placed

Here are the accuracy hits on the three test cases:

**Self-efficacy for S3E (Ego Shock — where someone confronts the fact that a skill they built their identity around is now something a tool can do).** Accurate. Bandura's self-efficacy is exactly "a person's belief that they can actually do the thing." When AI demonstrably performs a task the person trained for, that belief is no longer uniquely theirs. This is a precise fit. ✓

**Variable-reward for S6E (Enthusiastic Overuse — where someone routes every workflow through AI even when it is the wrong tool, energized by intermittent hits).** Accurate. This is the core mechanism of slot-machine engagement, social-media checking, and casual-game compulsion. V6's phrasing "intermittent-reward dynamic that underlies compulsive engagement with any tool whose outputs are unpredictably good" is textbook Skinner. ✓

**Metacognitive calibration for S7M (Maturity — where someone knows when to use AI and when not to, with boundaries that move only on measured evidence).** Accurate. Lichtenstein and Fischhoff's calibration research is exactly "accurate self-assessment of when one's own judgment is better than the tool's." This is a precise anchor. ✓

**Terror management for S3E (secondary mechanism).** Loose. Terror management (Greenberg & Solomon) is about mortality salience and existential anxiety in response to confrontation with death. The "existential discomfort" in S3E when someone confronts replaceability is real, but calling it terror management is stretching the construct. Better terms exist: "existential threat salience" or "confrontation with one's replaceability" or "mortality salience by proxy." V6 softens this slightly by saying "in the loose sense," but it should either drop the term or name it more precisely.

**Fix:** Replace "terror management in the loose sense" with "confrontation with replaceability as an existential threat" or "mortality salience by proxy" to avoid misquoting Greenberg & Solomon. If you want to keep a canonical psychological term, consider "existential threat response" or just drop it and say "the existential discomfort that comes from confronting one's replaceability compounds with the efficacy loss." The self-efficacy collapse is doing the real work here anyway.

---

## 3. Load-bearing varies by state; related-literature helps within-family discrimination, not across

The three anchors do different amounts of work:

**S7M's metacognitive calibration is load-bearing.** It carries the weight of distinguishing S7M Maturity from S3B Bargaining. Both states look identical from the outside — "uses AI for some things, not others." V6 says the difference is that S7M boundaries sit on the *competence line* (where is AI reliable?) while S3B boundaries sit on the *identity line* (what feels too important for me to delegate?). Metacognitive calibration explains the competence-line logic and anchors the observational test: "The S7M user can describe specific failure modes of the tools they use. The S3B user cannot." This is genuinely load-bearing vocabulary.

**S6E's variable-reward is moderately load-bearing.** It explains *why* the S6E person stays uncritical (intermittent reward sustains behavior despite failures), which distinguishes S6E from S6D (Dependent Overuse — anxiety-driven), S6R (Driven Overuse — productivity-goal-driven), and S6S (Social Overuse — peer-pressure-driven). But the discriminator here is the emotional register, not the variable-reward construct alone. Variable-reward names the mechanism but doesn't uniquely identify the state — you could have variable-reward in other contexts. It is load-bearing within the S6 family, less useful for saying "this is S6E and not something else."

**S3E's self-efficacy + terror management is contingently load-bearing.** The self-efficacy piece explains why this state is identity-level disruption (efficacy beliefs are central to identity) and distinguishes S3E from S3B (which is about dissonance reduction, not efficacy collapse). But the compound only works if both pieces are true. If only efficacy collapse occurs without existential threat, is it still S3E? If someone confronts replaceability without efficacy-belief loss (because they never had efficacy belief in the skill to begin with), is that S3E? V6 doesn't answer. The compound is load-bearing for S3E vs S3B discrimination, but you are relying on it to do two things at once, and they are not perfectly aligned.

**Fix:** Split the load-bearing claim for S3E. In the state file, separate "This state is characterized by loss of efficacy belief in the core skill" (the weight-bearing part) from "A secondary existential element may compound this" (the contingent part). Make it clear that efficacy collapse is necessary for S3E and the existential register is typical but not required. This prevents the state from being defined as a compound when half the compound is actually the core.

---

## 4. Related-literature vocabulary helps you think about a single state, not discriminate between distant states

A reader who wants to understand "what is S3E?" benefits from knowing "it's conceptually related to self-efficacy collapse." A reader who wants to know "is this person in S3E or S5?" gets less help. The related-literature anchors do not cleanly separate across state families.

Here's why: each related-literature construct describes an internal psychological process (efficacy belief, reward-driven behavior, calibration), and each state involves that process *combined with* a particular identity-stakes context and delegation level. A person could have variable-reward-driven behavior in S5 (understanding) or in S6E (enthusiastic overuse) depending on other factors. Metacognitive calibration exists in S5 (understanding) and S7M (maturity) and S7A (maturity in V5) and even S3B (bargaining) — most S3B users do calibrate their scope, just on identity grounds rather than competence grounds.

The related-literature vocabulary is most useful for anchoring individual states in existing thinking. It is less useful for diagnosing "which state are they in?" because the same underlying mechanism can show up in multiple states.

**Fix:** In the observation-guide, make explicit that the related-literature anchors are **not** diagnostic instruments. Say: "These constructs explain what each state involves cognitively, not how to identify which state a person is in. Identification uses behavioral markers and the graph logic, not the related-literature names."

---

## 5. For S3E specifically, the compound anchor is defensible but imprecise

The question: is the compound anchor (self-efficacy collapse + terror management) a defensible compound or two hedges stapled together?

It is **defensible** because the two mechanisms reinforce each other in the context of identity threat:

1. Efficacy collapse says: "I can no longer claim exclusive expertise in this skill."
2. Existential threat says: "My skill defined my role in the world. If I cannot claim it, what is my role?"

These are not independent; the second amplifies the first when identity is at stake. A person who loses efficacy belief in a low-stakes skill (e.g., using a calculator when they could do arithmetic by hand) does not experience existential threat. A person who loses efficacy belief in a high-stakes skill (e.g., writing if they are a novelist) experiences both. The compound is real.

But it is **imprecise** because:

1. "Terror management" is not the right term for the existential component. It implies death anxiety, not identity threat or replaceability anxiety. You are borrowing a term that carries baggage from thanatology into a different domain. V6's "in the loose sense" does not fix this.
2. The compound assumes both pieces activate together. If someone experiences efficacy collapse without existential threat (because the skill was never identity-central), are they in S3E? The model doesn't say. If someone experiences existential threat without efficacy collapse (a growing concern about AI impact on the field generally), is that S3E? It doesn't sound like it, but the model leaves room for it.

**Fix:** Rename the existential component to "confrontation with one's replaceability" or "existential threat through skill displacement" and drop the terror-management reference. Then add a note in the S3E file: "The compound is load-bearing when identity stakes are high. At low identity stakes, efficacy collapse may occur without the existential element. S3E is primarily defined by efficacy collapse; the existential register is typical at high stakes but not required for diagnosis."

---

## Recommendations

1. **Replace "terror management" with a more precise label.** Use "confrontation with replaceability as an existential threat" or drop the concept and just say "existential discomfort from replaceability." Terror management specifically refers to mortality-salience responses and should not be used for identity-threat responses. This is a correctness fix, not optional. (Priority: high)

2. **Clarify in Model6.md what was lost when moving from mechanisms to vocabulary.** Add one paragraph explaining that V5 claimed specific causal mechanisms without empirical support, V6 dropped those claims to be more honest, and this makes the model more epistemically careful but less explanatory. Readers need to know they are not getting "why S3E happens" — they are getting "what S3E is conceptually like." (Priority: high)

3. **In S3E, separate the load-bearing component (efficacy collapse) from the typical-but-not-required component (existential register).** Make it clear that efficacy collapse is necessary for the state, the existential element is typical in high-stakes contexts, and the two reinforce each other but the first is the actual anchor. (Priority: medium)

4. **In the observation-guide, add a note that related-literature constructs are not diagnostic instruments.** Say explicitly: "These anchors explain what is happening cognitively in each state, not how to identify which state a person is in. Use behavioral markers and the state-graph logic to identify states. Use the related-literature names to understand what you are looking at once you have identified it." (Priority: medium)

5. **Audit the other states for similar "loose fit" anchors.** Check S6R (Driven Overuse, anchored to "goal-substitution"), S6D (Dependent Overuse, anchored to "self-efficacy displacement"), and S7F (Evangelism, anchored to "generativity") for precision the same way you audited S3E. If "generativity" is just Erikson name-dropped without precision, rename it. (Priority: low — these were not in the test set, but the same audit logic applies)