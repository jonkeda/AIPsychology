This is a simpler rewrite of [004-adversarial.md](004-adversarial.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# V6 Adversarial Critique — Plain Language

## TL;DR

- V6's rename from "mechanism anchors" to "related literature" lowers the bar rather than raises it. Vocabulary connections prove nothing; mechanism claims at least have shape you can test.
- The "descriptive-first" framing sounds humble. It is actually a shield. The model describes typical transitions between states but won't commit to predicting them, so you can never prove it wrong.
- S3X Structural Displacement is a dropout path with an economic cause, not a new state. PEN Pre-emptive Non-Adoption is S2D Defensive Resistance with some genuine values mixed in, and the model admits you usually can't tell them apart.
- Per-domain identity-stakes scoping sounds like a refinement. It is actually a get-out-of-jail card: when the model is wrong, you redeclare what the stakes were in that domain after the fact.
- These three features stack. Redefine concepts as vocabulary, declare the model descriptive-not-predictive, and redeclare domain stakes — and no observation can ever prove the model wrong.

---

## Findings

### 1. The rename to "related literature" trades testable claims for circular ones — this is retreat, not honesty

V5 tied each state to a **mechanism** (the specific psychological reason for ending up there). S3E Ego Shock — the identity-panic state — was anchored to self-efficacy collapse (the feeling of "I'm no longer competent at my job") and to something called terror management (roughly, how people push back when their sense of identity feels threatened). Those are testable claims. Measure whether people in S3E actually show self-efficacy collapse. If they don't, the anchor was wrong.

V6 renames these anchors "related literature" and adds a disclaimer: knowing that S3E relates to self-efficacy collapse tells you what kind of thing S3E is, but it does not commit the model to saying self-efficacy collapse causes S3E.

What happened here: the model stopped making falsifiable claims (claims you can prove wrong with evidence) and started making definitional ones. S3E is identity disruption. Self-efficacy collapse is also identity disruption under a different name. Saying they're "related" is circular — it restates the same thing twice. You could say S3E is related to dissonance, or existential threat, or any other concept that sounds like identity disruption. It would be equally true and equally useless.

The claim that this is more honest than V5 is wrong. V5 said: here is the mechanism; test it. V6 says: here is a vocabulary tag; it commits to nothing. That is not transparency. It is obfuscation dressed up as transparency.

**Fix:** Pick a lane:
- **(a) Make the literature anchors testable:** for example, "S3E shows the pattern of identity-protective thinking (where people reject evidence that threatens their self-image). Test: measure whether people in S3E update their beliefs asymmetrically across multiple AI releases. If they update symmetrically, the anchor is wrong."
- **(b) Drop the literature anchors entirely:** name states plainly and describe them in behavioral terms. The link to self-efficacy is interesting but not required.

Don't do what V6 does: claim conceptual grounding while refusing to commit to what that grounding means.

---

### 2. The "descriptive-first" label gives the model immunity it hasn't earned

V6 opens by saying it is descriptive: it names recognizable patterns; it does not make causal claims, predictions, or diagnostic tools.

Then it immediately describes transitions as if they are observed patterns. S2D Defensive Resistance typically leads to S3E Ego Shock. S3E typically leads to S3B Bargaining or S5 Understanding. The initial encounter forks to either S2T Trust Evaluation (where a person evaluates AI fairly) or S2D, depending on how much the person's identity is tied to the threatened skill.

Those are claims about how people move through states. They read exactly like predictions to anyone using the model. But when the prediction fails — say, someone in S2D skips S3E and goes straight to S5 — the model says: I never made a prediction; I'm descriptive, not predictive. This is cover without substance.

The word **"typically"** is doing all the work. Either it means something (more than half the time? more than 70%?) or it means nothing. V6 will not say which.

**Fix:** One of two choices:
- **(a) Commit to the transitions as testable claims:** specify a study that could prove them wrong. For example: "A long-running study tracking 100+ people across three model releases, measuring which state they're in at each point. We predict that more than 60% of S2D people enter S3E within 12 months. If fewer do, the 'typically leads to' claim needs revision."
- **(b) Be genuinely descriptive:** stop claiming which states lead to which. Instead say: "In the trajectories we've observed, we've seen people go from S2D to S3E, from S2D to S3B, and from S2D directly to S5. Here are three example profiles." No implied frequency. No "typically."

Flagging things as Conjecture or Testable does not fix this. The claims still aren't falsifiable; the flags just say you already know that.

---

### 3. S3X Structural Displacement is a labeled dropout scenario, not a new state

V6 introduces S3X (Structural Displacement) as a state reached when a person concludes "my job isn't being disrupted — my job is being replaced." It distinguishes S3X from S3E Ego Shock (which is about identity) and from dropout (described as a willing exit).

But read the logic. S3X occurs when "viable AI-collaborative work no longer exists in the person's domain" — when there is genuinely no role left to adapt into. The identity question is still unresolved, but now there is also an economic fact: the job market has already made the decision.

This is not a new state. The existing model already has a dropout zone described on two axes: how severe the practical problems are (tool failures, workflow friction) and how severe the emotional problems are (identity threat, exhaustion). S3X is the case where **practical severity is extreme** because the labor market has objectively removed the role. It is not "unwilling to continue" — that would be emotional dropout. It is "there is no position left to continue into" — extreme practical dropout with a structural cause rather than a tool-failure cause.

The S3X file says this isn't emotional dropout because emotional dropout happens when the psychological cost gets too high, while S3X happens when the domain is gone. But that distinguishes the reason for the exit, not the psychological state the person is in. Both are exits. The psychological work in both cases is similar: accept the exit and figure out what comes next.

The model has labeled a dropout scenario as a state to look more comprehensive. It isn't.

**Fix:** Demote S3X from state to documented path. Move it into the dropout file as: "Some people drop out because the labor market made the choice for them — the role is economically non-viable and there is nowhere to adapt to. This is a high-practical-severity dropout with a structural cause rather than a tool-failure cause. The psychological work is the same as other dropouts, but the external cause and timeline differ."

Alternatively: provide an operational test — a way to tell S3X apart from practical-high dropout that doesn't use the circular definition "S3X is when the role is gone." V6 doesn't have one.

---

### 4. PEN Pre-emptive Non-Adoption is S2D Defensive Resistance with genuine values in the mix — the model admits it can't reliably tell them apart

V6 introduces PEN as a new state: values-based refusal to adopt AI at first encounter, distinct from S2D (identity-protective thinking — the tendency to reject evidence that threatens how you see yourself).

The diagnostic file lists three signals:
- Cross-domain consistency: does the ethical objection apply consistently across areas, not just where the person feels most threatened?
- Evidence response: does the position hold even if the stated concern is addressed?
- Emotional register: does the person sound like someone making a moral argument, or someone who is anxious?

Then the file says: "Most real cases are mixed. A person can simultaneously be in S2D and making genuine ethical arguments that are also true and genuinely held... Labeling a mixed case as 'pure PEN' would be wrong; so would 'pure S2D.' Use the frame to understand the mixture, not to classify it."

So the model introduces a state and immediately admits you usually can't tell whether someone is in that state or in S2D. The signals require months of observation across multiple areas of the person's life. The file then says: don't classify people as pure PEN anyway.

This is not a state. It is a footnote in the S2D file. A state is something you can identify. PEN, as described, is only distinguishable from S2D after months of observation — the exact thing the model said it wouldn't require.

What V6 actually did: it added a label for "S2D plus genuine moral reasoning." That is not a new state; it is a recognition that people in S2D sometimes also hold real ethical objections. That is always true. You don't need a new state for it; you need a note about variation within S2D.

**Fix:** Demote PEN to an annotation inside the S2D file. Write: "Some people in S2D also have genuine, values-grounded ethical objections alongside their identity-protective thinking. These cases are hard to separate from 'pure ethical non-adoption' without months of observation. The three signals (cross-domain consistency, evidence response, emotional register) help practitioners understand the mix. If the evidence-response pattern suggests the values are doing the real work, prioritize the ethical conversation over the identity-protection work." No state number. Not in the graph.

---

### 5. Per-domain identity-stakes scoping looks like a refinement but works as a get-out-of-jail card

V6 makes explicit that **identity stakes** (how much a person's professional self-image depends on the skill being threatened) are per-domain, not per-person. The same person can be in S2D in their main area of expertise and in S5 Understanding — the stable, integrated state — in a skill they picked up two years ago.

As a description of how people actually work, this is accurate. People are not psychologically uniform across domains.

But it creates a logical problem: identity stakes are now unmeasurable before the fact.

The model's core claim is: high-stakes people tend to fork to S2D; low-stakes people tend to fork to S2T Trust Evaluation (the state where someone evaluates AI fairly). But identity stakes are defined after the fact by watching which fork the person takes. High stakes = person went to S2D. Low stakes = person went to S2T. The parameter is defined by the outcome it is supposed to explain. That is circular.

For example: you predict someone will go to S2T because you judged their identity stakes low. They go to S2D instead. Rather than the model being wrong, you declare: "the identity stakes in this domain were higher than I thought." The model can't be proved wrong. Every surprise can be reframed as new information about domain parameters you hadn't measured yet.

V5 had the same per-domain structure but kept it quiet, which was more honest. V6 elevated it to a design principle, making it look like a feature when it is an escape hatch.

**Fix:** Define identity stakes independently of behavior — using a measure that works before you know which fork someone takes. Examples that would work:
- Years invested in training or certification in this domain
- Percentage of income from this domain
- A short interview asking how central this skill is to the person's professional identity

Then run a prospective study — one where you measure first and observe outcomes second. If low-stakes people still go to S2D at rates above 40%, the fork prediction needs revision.

If you can't define stakes in advance, the per-domain framing is not a model feature. It is an admission that the S2T-vs-S2D fork may not be real.

---

### 6. Three escape hatches stacked together make the model impossible to disprove

Put the pieces together. The model:
1. Uses vocabulary anchors that commit to nothing ("related literature" can mean any nearby concept).
2. Declares itself descriptive-not-predictive while describing transitions as typical patterns.
3. Allows per-domain identity stakes to be redeclared after the fact.

The result: no observation can disprove the model.

- A transition doesn't happen? The transition was never a prediction; the model is descriptive.
- A state definition doesn't hold? Reframe the state as "related to" a different vocabulary concept.
- The fork prediction is wrong? Redeclare the identity stakes for that domain.

This is a vocabulary set with three layers of insulation against criticism. The five stages of grief model faced the exact same problem — people do not actually move through five ordered stages — and the honest response was to either make the model more specific and testable, or admit it is a loose guide. V6 chose a third path: add escape hatches so the model is never obviously wrong.

**Fix:** Commit to falsifiability or admit the model is speculative. Pick one:
- **(a) Make it falsifiable:** lock down the identity-stakes measurement in advance; commit to specific transition probabilities or ranges; run long-running studies with hypotheses locked in before data collection starts; accept the model could be wrong.
- **(b) Admit it is speculative:** reframe the model as "a vocabulary and an orientation — useful for thinking about adaptation patterns, but not yet grounded in evidence. This is a first draft of how to think about this space, not a tested description of it." That would be more honest than the current position.

The current position — "this is descriptive so it is safe from criticism, but here are all the typical patterns anyway" — is not defensible.

---

## Minimum Changes to Make This Critique Not Apply

1. **Operationalize identity stakes** — provide a measurement that doesn't depend on observing which fork someone takes (a survey item, income data, a short interview, time-in-domain). Then run a prospective study. If low-stakes people still show S2D rates above 40%, revise the fork prediction.

2. **Choose between mechanism and vocabulary** — either restore falsifiable mechanism claims and commit to testing them, or drop the literature anchors and describe states in purely behavioral terms. Don't claim vocabulary anchors while running from empirical commitment.

3. **Make transition claims testable or drop them** — either specify a study that would falsify "S2D typically leads to S3E," or stop claiming that S2D typically leads anywhere. "In observed trajectories we have seen X, Y, Z" is defensible. "Typically leads to" is a prediction that needs a test.

4. **Demote S3X and PEN from states** — reframe them as documented paths (S3X as a structured-practical-severity dropout variant, PEN as variation within S2D), or give them pre-observation diagnostics that don't require months of long-running observation.

5. **Add falsifiability test cases to the limits-of-operationalization section** — for each of the three escape hatches (vocabulary redefinition, descriptive-not-predictive shield, per-domain parameter redeclare), specify what observation would show the escape hatch is being misused. You can't prevent rescue clauses; you can make their overuse visible.
