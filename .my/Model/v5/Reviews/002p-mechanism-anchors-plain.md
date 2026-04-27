This is a simpler rewrite of [002-mechanism-anchors.md](002-mechanism-anchors.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Mechanism Anchors — Plain-Language Version

## What "mechanism anchor" means here

V5 attaches a **mechanism anchor** to each state in the model. That's a fancy term for "the underlying psychological reason this state exists." For example, S3 Ego Shock (the panic state) is anchored to two reasons: (1) the person's belief that they can do their job is collapsing, and (2) they're confronting the idea that they could be replaced.

Anchors are supposed to make the model more credible and more testable. The question this review asks: do the anchors actually do that work, or are they just labels?

## TL;DR

- **S3 Ego Shock's anchor uses two mechanisms at once and won't pick.** V5 says S3 Ego Shock is caused by self-efficacy collapse **plus** confrontation with replaceability, and that "S3 Ego Shock is rarely just one of them." That hedge breaks falsifiability. If you see S3 Ego Shock without the existential dread piece, is it still S3 Ego Shock? The model won't say.
- **S7B Identity Expansion's anchor ("extended-self") is too broad.** Any identity shift after using AI gets retrofitted as "tool incorporation." The model never says what wouldn't count as S7B Identity Expansion.
- **S2T Trust Evaluation's anchor is the same mechanism as S2D Defensive Resistance, just relabeled.** Both states are people updating their beliefs against evidence. The model claims S2T Trust Evaluation is fair updating and S2D Defensive Resistance is defensive, but the anchor (calibration) doesn't predict that split. The split is determined by Identity Stakes, not by a different mechanism.
- **S6A Enthusiastic Overuse and S6B Dependent Overuse have similar problems to S3 Ego Shock.** S6A Enthusiastic Overuse's anchor is fine but says nothing about why S6A Enthusiastic Overuse users are uncritical. S6B Dependent Overuse's anchor cites Bandura's self-efficacy work, but the actual mechanism described is **learned helplessness** (Seligman) — a different and more serious thing.
- **Dropout's emotional-severity anchor is too broad.** "Threat-driven avoidance" could mean S2D Defensive Resistance, S3 Ego Shock, S3B Bargaining, or actual quitting. The model needs to say what kind of threat causes withdrawal versus boundary-setting.
- **Most anchors are decoration, not prediction.** The model picked the behavior first and then attached a mechanism name. A real anchor should predict something new — failure modes, transitions, edge cases. Most don't.
- **S5 Understanding's two-piece stability claim has no anchor at all.** The model says S5 Understanding needs both internal coherence and social acceptance. That's the most testable claim in the whole model. It has no mechanism backing it and is marked as a guess.
- **Bottom line:** V5's anchoring move is half-done. A few anchors earn their place (S3B Bargaining, S7A Maturity). Most don't. The version-bump claim — that anchoring justifies V5 — is overstated. Anchoring buys credibility, not predictive power.

## Findings

### 1. S3 Ego Shock: The "two mechanisms at once" anchor is a hedge

**The claim:** S3 Ego Shock (Ego Shock) is caused by self-efficacy collapse (the feeling of *I can't do my job anymore*) **plus** terror management (confronting *I might be replaceable*). The model says these "compound" and that S3 Ego Shock is "rarely just one of them."

**Why this fails:** If the model won't say which mechanism is primary, you can't disprove S3 Ego Shock.

- Imagine someone in a high-stakes job whose AI-using coworker outperforms them. Clear hit to self-efficacy. No existential dread. Are they in S3 Ego Shock? If yes, the second mechanism is decorative. If no, the model needs a separate state for self-efficacy-only shock.
- Imagine someone who confronts the idea of being replaceable in a low-stakes domain. Existential dread, no hit to professional identity. Are they in S3 Ego Shock? Or S2D Defensive Resistance? The model won't say.

**Why it gets worse:** V5's transition table for S3 Ego Shock (Low Stakes × D1 = mild surprise, all the way up to High Stakes × D4 = existential) looks like one underlying response getting dialed up by stakes and delegation. That's one mechanism scaling, not two mechanisms compounding. The anchor doesn't match the table.

**Falsifiability problem:** Any S3 Ego Shock case can be explained after the fact by mixing the two mechanisms in whatever proportion fits. Anxiety without dread? Mechanism one. Dread without anxiety? Mechanism two. The model never predicts in advance which mix you'll see. That's a story-telling tool, not a scientific anchor.

### 2. S2T Trust Evaluation: The "calibration" anchor misses the actual claim

**The claim:** S2T Trust Evaluation (Trust Evaluation) is anchored to **calibration** — updating your estimates of AI's reliability against the evidence. The model also nods to the Technology Acceptance Model (Davis, 1989 — people adopt tech if they think it's useful and easy).

**Why this fails:** Calibration is a neutral process. It's just updating beliefs against reality. But the model treats S2T Trust Evaluation as specifically *non-defensive* updating. The only thing separating S2T Trust Evaluation from S2D Defensive Resistance in the model is whether the updating is fair or asymmetric.

But calibration theory doesn't predict that split. It predicts people update against evidence. S2D Defensive Resistance users update too — they just update defensively. Both groups are calibrating. The anchor doesn't explain why one is fair and the other isn't.

**The hidden contradiction:** The model says Identity Stakes determine whether you go to S2T Trust Evaluation or S2D Defensive Resistance. But calibration shouldn't care about identity stakes. If the anchor were correct, identity stakes wouldn't predict the fork. The model says they do. So either the anchor is wrong or the fork claim is wrong.

The Technology Acceptance Model nod doesn't help. TAM says people adopt tech if it's useful and easy. It says nothing about whether they're defending an identity while evaluating it.

### 3. S2D Defensive Resistance: The identity-protection anchor is solid, with one caveat

**The claim:** S2D Defensive Resistance (Defensive Resistance) is anchored to **identity-protection cognition** — the tendency to evaluate evidence in ways that defend a valued self-concept. The model cites Dan Kahan's work on political beliefs and Festinger's cognitive dissonance (the discomfort of holding two beliefs that contradict each other).

**This one fits.** Kahan and Festinger are the right references. The behaviors the model describes — nitpicking, downplaying AI's strengths, highlighting weaknesses, weighting bad examples more than good ones — are exactly what identity-protection predicts.

**Caveat:** The model says S2D Defensive Resistance and S2T Trust Evaluation can look identical from outside, and that you only tell them apart by watching whether updating is asymmetric over time. That's true, but it limits how useful the model is for snapshot judgments. You can't sort someone into S2T Trust Evaluation or S2D Defensive Resistance after one conversation. You need longitudinal data. That's not a flaw in the anchor — it's a limitation of the state.

**Testable:** Yes. Measure how the same person evaluates AI in a high-stakes (their own job) versus low-stakes (someone else's job) domain. Identity-protection predicts they'll be tougher on AI in their own domain.

### 4. S3B Bargaining: The scope-limitation anchor is excellent

**The claim:** S3B Bargaining (Bargaining) is anchored to **dissonance reduction by narrowing scope**. The person can't deny AI is good, so instead they shrink the territory they will use it in. "I'll use it for drafting, not for final output."

**This one fits perfectly.** It's Festinger's dissonance theory applied with surgical precision. The model also includes a way to tell S3B Bargaining apart from S7A Maturity (mature bounded use): in S3B Bargaining, the boundary moves quickly when a new model comes out, without testing. In S7A Maturity, the boundary moves only after measured evidence.

That's a real, testable prediction. Track people across model releases. See whether their lines move with or without testing. Good anchoring.

### 5. S5 Understanding: The most testable claim has no anchor

**The claim:** S5 Understanding (Understanding) is anchored to **schema integration** — the cognitive process of fitting AI into your existing mental model of work. But the model also adds: S5 Understanding stability needs two pieces, both required: (1) **internal** — your mental model is coherent, and (2) **social** — your team treats AI use as unremarkable.

**Why this fails:** Schema integration is a *cognitive* mechanism. It only covers piece one. The social piece has no anchor. And the dual-component claim is explicitly marked in the model as a guess.

This is backwards. The two-piece claim is the most testable thing in the model — the most likely candidate for a real study. But it has no mechanism backing it. Meanwhile, less testable claims get anchors.

**A second problem:** Schema integration is supposed to create stable internal coherence. So why does the model treat S6B Dependent Overuse (dependent overuse, where self-efficacy has eroded) and S6D Social Overuse (social overuse, driven by peer pressure) as common downstream paths? If schema integration is doing its job, those should be failure modes or regressions, not separate states. The anchor doesn't explain it.

### 6. S6A Enthusiastic Overuse: Variable-reward anchor is right, but doesn't cover everything

**The claim:** S6A Enthusiastic Overuse (Enthusiastic Overuse) is anchored to **variable-reward reinforcement** — the same dynamic that makes slot machines work. AI sometimes produces something amazing, sometimes mediocre. The unpredictability sustains the behavior.

**This fits.** Variable-reward schedules really do produce sustained, high-rate behavior. The claim that S6A Enthusiastic Overuse users route every workflow through AI even when it's the wrong tool is exactly what the theory predicts.

**Caveat:** The model says S6A Enthusiastic Overuse users are "uncritical." Variable-reward theory doesn't predict uncriticalness. It predicts engagement. A person could be engaged *and critical* — running tests on AI's outputs to learn when it's good. The "uncritical" part might come from a different mechanism (high-dopamine states, maybe), but the model doesn't say.

**Testable:** Yes. The theory predicts that low-variance AI (consistently good) should exit S6A Enthusiastic Overuse faster than high-variance AI. The model could state this prediction explicitly but doesn't.

### 7. S6B Dependent Overuse: The anchor names the wrong mechanism

**The claim:** S6B Dependent Overuse (Dependent Overuse) is anchored to **self-efficacy displacement** (Bandura's term in reverse) — confidence in AI replaces confidence in self.

**Why this fails:** What the model is actually describing is **learned helplessness** (Seligman, Maier), not Bandura's self-efficacy.

- **Learned helplessness:** When a person repeatedly finds their actions don't matter (AI solves it; their input wasn't needed), they stop trying. They learn that effort itself is pointless.
- **Bandura's self-efficacy:** About mastery experiences building belief in your own ability. Reversing it would mean losing confidence in a domain and retreating to other domains where you still feel capable.

These predict different things. Bandura predicts the person backs away from the AI-affected domain but stays competent elsewhere. Learned helplessness predicts a deeper collapse where the person stops believing effort works at all.

**Why it matters:** The model lists a transition from S6B Dependent Overuse to S7A Maturity (maturity) as "rare but possible when the person rebuilds independent judgment." Under learned helplessness, that transition is *very hard*. You usually need outside intervention to break it, not just time. The anchor doesn't predict the difficulty.

### 8. S6C Driven Overuse: Goal-substitution anchor is plausible but vague

**The claim:** S6C Driven Overuse (Driven Overuse) is anchored to **goal-substitution** — efficiency, originally a means to other goals (more output, better balance, career advancement), becomes a goal in itself. The model points at organizational psychology work on subgoals taking over.

**This is plausible.** Subgoal creep is a real phenomenon. People in high-performance cultures do start treating efficiency as terminal. But plausibility isn't the same as fit.

**What's missing:** Goal-substitution theory predicts that when efficiency becomes terminal, people optimize for it even when it damages the bigger goal it was supposed to serve. The model says S6C Driven Overuse exits to S7D Burnout (Burnout) because "there is no natural ceiling on more efficient." That's exactly the failure mode goal-substitution predicts. The model should state that prediction explicitly. It doesn't.

**Testable:** Sort of. You'd need to measure the difference between "I want to be efficient" and "efficiency-as-itself-matters." The only instrument is self-report, which contaminates the test.

### 9. S6D Social Overuse: Social-influence anchor is solid but narrow

**The claim:** S6D Social Overuse (Social Overuse) is anchored to **normative social influence** — behavior driven by wanting to match peers, regardless of personal evaluation. The model cites Asch's classic conformity experiments.

**This fits.** Asch's work and the broader social-influence literature predict exactly this behavior.

**Testable:** Yes, easily. Remove the peer reference — change teams, roles, social context — and S6D Social Overuse users should reduce AI use faster than S6A Enthusiastic Overuse or S6C Driven Overuse users. The model doesn't make that prediction explicit. It should.

### 10. S7A Maturity: Metacognitive calibration anchor is excellent

**The claim:** S7A Maturity (Maturity) is anchored to **metacognitive calibration** — accurate self-assessment of when your own judgment beats the tool's. The mature user has an internal model of where the tool fails (where it hallucinates, where it sucks up to you, where it averages out the interesting answers) and routes work to dodge those failures.

**This is precise.** This is Lichtenstein and Fischhoff's work on confidence-accuracy alignment, applied correctly. The key claim — that S7A Maturity users have a *working model of failure modes*, not just general confidence — is much sharper than S2T Trust Evaluation's vague "calibration."

**Testable:** Yes. Ask S7A Maturity users to explain where AI fails in their domain. Compare their explanations to actual failure patterns. S7A Maturity users should be more accurate than S6 users. Also: the model predicts S7A Maturity regresses to S3 Ego Shock when a capability jump invalidates the calibration. You can test that against model releases.

This is what mechanism anchoring should look like.

### 11. S7B Identity Expansion: "Extended-self" is too broad to be falsifiable

**The claim:** S7B Identity Expansion (Identity Expansion) is anchored to **extended-self / tool incorporation** — humans incorporate tools into their self-concept. Carpenter and hammer. Photographer and camera. The model points at Belk's work on the extended self in consumer behavior.

**Why this fails:** Extended-self is too broad. Every person who uses any tool regularly will incorporate it into their self-concept to some degree. The carpenter doesn't say *I am the person who operates this hammer* — they just become better at carpentry.

**The real distinction the model wants:** The example given is a novelist using AI to polish their voice (S7A Maturity) versus a person who couldn't write fiction before AI and now identifies as a writer-with-AI (S7B Identity Expansion). But that distinction is **identity creation**, not tool incorporation. It's a different mechanism: the tool enabled a capability that became part of who the person is. Extended-self doesn't predict which tools become identity-constitutive and which don't.

There's also a category mismatch. Belk's extended-self is about *possessions* — your car, your clothes, your collection. The model is borrowing a consumer-behavior idea to explain capability-identity fusion. That's not a clean fit.

**Falsifiability:** Very weak. The anchor lets you classify any post-AI identity shift as S7B Identity Expansion. The model never says what wouldn't count.

### 12. S7C Ethical Integration: Meaning-making anchor is too vague

**The claim:** S7C Ethical Integration (Ethical/Philosophical Integration) is anchored to **meaning-making** — integrating a personally significant experience into a coherent worldview. The model cites post-traumatic growth research.

**Why this fails:** Meaning-making is too broad. Any reflection on AI could be called meaning-making. The model describes S7C Ethical Integration as sustained reflection on bias, intellectual property, authenticity, labor, environment, society. But why is that meaning-making rather than just *thinking about ethics*?

In the post-traumatic-growth literature, meaning-making specifically means integrating trauma into a revised sense of life purpose. The model is using the term for a much weaker thing.

**The behavior doesn't match the anchor either:** The model says S7C Ethical Integration people often *use AI minimally* — their reflection leads them away from the technology. But meaning-making predicts integration, not withdrawal. The genuine process being described looks more like ethical deliberation within continued use, not meaning-making in the deep sense.

**Testable:** Weak. To check meaning-making you'd need to ask people about their worldview. That's self-report contamination. The model doesn't specify what observable behaviors would count as evidence — public advocacy, changed boundaries, life changes. Without that, the anchor is just a fancy name for "thinking about ethics."

### 13. S7D Burnout: Resource-depletion anchor is solid

**The claim:** S7D Burnout (Burnout / Withdrawal) is anchored to **resource depletion** — sustained high-effort engagement, whatever its source (S6A Enthusiastic Overuse enthusiasm, S6B Dependent Overuse anxiety, S6C Driven Overuse drive, S6D Social Overuse social pressure), draws on finite regulatory resources. When you're depleted, you withdraw to recover. The model cites cognitive-control fatigue research and Maslach's burnout work, and honestly notes the open debate over whether "depletion" is literal energy or a motivation shift.

**This fits.** Standard burnout theory. The honesty about the depletion-versus-motivation debate is valuable.

**Testable:** Moderately. You could test whether S7D Burnout exits are shorter after vacations (supporting literal depletion) or driven by meaning shifts (supporting motivation). The model could specify what kind of recovery breaks S7D Burnout — rest, meaning change, or both — but doesn't.

### 14. S7F Evangelism: Generativity anchor is right, but the prerequisite claim is unsupported

**The claim:** S7F Evangelism (Influence / Evangelism) is anchored to **generativity** (Erikson's term, broadened — the drive to invest in the next group's success). Senior practitioners turn to mentoring; AI provides a sharp opportunity because the cohort needing guidance is huge and the experience required is just a few years.

**This fits.** Generativity is real, and the AI-specific gloss is reasonable.

**The problem:** The model also claims that stable S7F Evangelism requires having previously gone through S3 Ego Shock (the panic state). It admits this is a guess. But Erikson's generativity doesn't predict that prerequisite. The model is bolting on an extra constraint that the anchor doesn't support.

**Testable:** The model is honest that the S3 Ego Shock-prerequisite is unmeasured. That honesty is good. But it means the anchor isn't carrying the full weight of the state. The real predictor is probably "prior identity threat + current expertise + desire to help" — more complex than just generativity.

### 15. Dropout: The practical side is fine; the emotional side is too broad

**The claim:** Practical dropout is anchored to **expectancy violation** — the tool didn't deliver what its perceived capability promised. Emotional dropout is anchored to **threat-driven avoidance** — continuing predicts further psychological cost, so the person stops.

**Practical side fits.** Expectancy violation is solid.

**Emotional side fails:** "Threat-driven avoidance" is too broad. Threat exists in S2D Defensive Resistance, S3 Ego Shock, and S3B Bargaining as well. What separates emotional dropout from those states?

**The reversibility test the model proposes** — give the dropout a tool that fixes their stated complaint and see if they restart — has confounds:

- If someone dropped out from S3 Ego Shock (identity threat) and you give them a better tool, they still might not restart, because the threat hasn't resolved. The tool isn't the issue.
- If someone dropped out from S6D Social Overuse (social pressure) and the pressure has lifted, they'll restart even if the new tool is mediocre.

**The S3B Bargaining confusion:** S3B Bargaining is the state where someone uses AI for some things but not others *because* identity threat persists. That's not dropout — but it has the same underlying threat as emotional dropout. What's the difference between "S3B Bargaining uses AI for X but avoids Y due to threat" and "emotional dropout avoids AI entirely due to threat"? The model doesn't say. The anchor should connect the two outcomes through one mechanism with different intensity, but it doesn't.

### 16. S1 Initial Encounter: Novelty appraisal is reasonable but does no work

**The claim:** S1 Initial Encounter (Initial Encounter) is anchored to **novelty appraisal** — the brain's first-pass classification of an unfamiliar stimulus as relevant or irrelevant, threatening or benign. The model cites Lazarus and Folkman's stress-appraisal work — the idea that people first decide *what is this and does it matter*, then decide *what can I do about it*.

**This is reasonable.** Lazarus's appraisal theory is the standard model.

**But the anchor does no work:** The model says S1 Initial Encounter's emotional flavor (curiosity, skepticism, threat) "depends on Identity Stakes, not on this state itself." If the axes determine the flavor, the appraisal mechanism isn't doing anything at the state level. You can't test S1 Initial Encounter's appraisal independently of the axes that already decide what the appraisal will conclude.

**Minor conflict:** The model lets S1 Initial Encounter transition directly to S5 Understanding "for low stakes with prior conceptual familiarity." But novelty appraisal should go through S2T Trust Evaluation or S2D Defensive Resistance evaluation first. Appraisal is just initial classification, not full evaluation. The S1 Initial Encounter→S5 Understanding shortcut suggests a different mechanism is operating (probably prior schema compatibility), but the anchor doesn't cover it.

## Recommendations

1. **Fix S3 Ego Shock's compound anchor.** Pick one of three options:
   - **(a)** Make S3 Ego Shock primarily self-efficacy collapse and move existential-threat cases to a separate state or frame.
   - **(b)** Specify which trigger leads to which mechanism: capability replacement → efficacy collapse; replaceability without specific job at stake → terror management; both possible in high-stakes/high-delegation contexts but with different transitions.
   - **(c)** Provide a timeline: efficacy collapse first, existential threat after weeks of continued exposure if nothing resolves.

2. **Reframe the S2T Trust Evaluation/S2D Defensive Resistance anchors.** Either reframe S2T Trust Evaluation as "risk appraisal under evaluative context" or "motivated evaluation of utility and ease-of-use" — acknowledging it's the same calibration mechanism as S2D Defensive Resistance with different stakes. Or drop S2T Trust Evaluation's separate anchor entirely and say: both states are calibration; identity stakes determine fair versus defensive. That's more honest.

3. **Anchor S5 Understanding's two-piece stability or downgrade it.** The dual-component claim (internal coherence + social acceptance) is the most testable thing in the model. Either give it a real anchor — schema integration for the cognitive piece, plus a social-mechanism anchor (for example: internal coherence without social validation drifts to S6D Social Overuse; social validation without internal coherence drifts to S2D Defensive Resistance) — or move it to "Limits of operationalization" and stop treating it as a state property.

4. **Reframe S7B Identity Expansion's anchor.** Replace "extended-self / tool incorporation" with **capability-driven identity expansion** — acquiring a capability through AI that becomes part of who you are because it was previously out of reach. Add a falsifiable line: S7B Identity Expansion users will say *I'm a writer now*; S7A Maturity users will say *I'm a better writer*. The first describes a new identity; the second describes a sharper old one.

5. **Strengthen S7F Evangelism's S3 Ego Shock-prerequisite or drop it.** Either treat the S3 Ego Shock-prerequisite as a heuristic and remove it from the structural claim, or extend the anchor to "generativity post-identity-disruption" — people who passed through S3 Ego Shock can authentically guide others through it because they lived it.

6. **Clarify dropout's emotional-severity mechanism.** Redefine emotional dropout as **withdrawal driven by threat-recovery-blocking conditions** — situations where the person sees no path to resolving the threat (identity won't shift, efficacy can't rebuild, pressure won't relent). For each, specify recovery conditions: identity threat → identity reconstruction or domain shift; efficacy threat → efficacy-building or role change; pressure → context or network shift. Then the reversibility test predicts emotional dropouts won't return until the threat resolves, no matter how good the tool gets.

7. **Rename S6B Dependent Overuse and revise its transitions.** Either retitle it "Learned-helplessness overuse," cite Seligman and Maier instead of Bandura, and revise the transitions to reflect how hard it is to escape. Or keep "efficacy displacement" but specify it's *domain-specific*: confidence in AI replaces confidence in self for *this task*; other domains may be intact. Bandura works once you localize it.

8. **Add falsifiable predictions to anchors that lack them.** S3B Bargaining, S7A Maturity, and S7D Burnout earn their anchors by predicting something. The others should too:
   - **S6A Enthusiastic Overuse:** Low-variance AI (consistently good) causes faster S6A Enthusiastic Overuse exit than high-variance AI.
   - **S6C Driven Overuse:** S6C Driven Overuse users will optimize efficiency past the point where it damages the bigger goals it was supposed to serve.
   - **S2D Defensive Resistance:** Affirming a person's identity in their domain first should make them re-evaluate AI more fairly afterward.
   - **S6D Social Overuse:** S6D Social Overuse collapses faster than S6A Enthusiastic Overuse or S6C Driven Overuse when you change the peer context.

9. **Drop the "anchoring justifies V5" framing.** S1 Initial Encounter and S7C Ethical Integration anchors are decorative — they describe the states correctly but predict nothing new. That's not fatal, but it means the version-bump claim is overstated. Reframe the achievement: V5 adds anchoring to improve credibility and ground future studies. Some anchors (S3B Bargaining, S7A Maturity) make strong falsifiable predictions. Others (S1 Initial Encounter, S7C Ethical Integration) are mainly descriptive. All of them give the next version handholds to test.
