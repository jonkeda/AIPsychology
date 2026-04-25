# Mechanism Anchor Audit — Model V5

## TL;DR

- **S3's compound anchor (self-efficacy + terror management) is a hedge, not a defensible union.** V5 avoids saying which mechanism is primary, which creates falsifiability ambiguity: if S3 manifests without existential dread, is it S3 or something else?
- **S7B's "extended-self" anchor is too broad to be falsifiable.** Every identity-shift after AI exposure can be retrofitted as "tool incorporation"; the model doesn't say what wouldn't count as S7B.
- **S2T's "calibration" anchor obscures a key claim.** The model treats S2T as non-defensive evaluation, but calibration theory predicts defensive updating too. The anchor doesn't carve out why S2T avoids the asymmetry that defines S2D.
- **S6A and S6B share the mechanism problem as S3.** S6A is "variable-reward" and S6B is "self-efficacy displacement"—but displaced *toward AI*, which isn't what self-efficacy psychology predicts. This might be correct, but the anchor papers over the difference instead of defending it.
- **Dropout's two-axis mechanisms (expectancy violation + threat-driven avoidance) are vague.** "Threat-driven" is too broad; it could apply to S2D, S3, or S3B. The model needs to specify what kind of threat triggers emotional dropout vs. what keeps a person in S3B bargaining.
- **Falsifiability gain across the board is minimal.** Most anchors are **post-hoc fit**—the model behavior is specified first, then a mechanism name is attached. Anchors would buy value if they predicted novel transitions or failure modes; instead they describe the states the model already claimed.
- **S5's dual-component stability (internal reframing + social normalization) is a conjecture without anchoring.** This is the most falsifiable claim in the model, but it has no mechanism anchor. The asymmetry is suspicious.

## Verdict

V5's mechanism anchoring move is partial. Some anchors earn their place by predicting failure modes (S3B's scope limitation, S7A's metacognitive boundaries). Most are decorative — they restate the model's claims in mechanistic language without improving predictiveness or testability. The compound anchor on S3 is particularly problematic because it defers the hard question: if identity threat and self-efficacy threat come apart, which one determines S3 transitions? Until the model answers that, S3 is unfalsifiable. This doesn't sink V5 — it's still a valuable descriptive framework — but it means the version-bump claim ("mechanism anchoring justifies V5") is overstated. The anchoring buys *credibility*, not *predictive power*.

---

## Findings

### 1. S3: Compound anchor is a hedge masquerading as precision

**The claim:** S3 (Ego Shock) is anchored to "self-efficacy collapse under domain-specific capability threat (Bandura's term — a person's belief that they can actually do the thing). When AI demonstrably performs a task the person built their self-concept around, the belief that 'I can do this' no longer carries unique weight. A secondary mechanism is terror management in the loose sense — confrontation with one's own replaceability triggers the same kind of existential discomfort that confrontation with mortality does. The two mechanisms compound; S3 is rarely 'just' one of them."

**Fit problem:** The phrase "compound; S3 is rarely 'just' one of them" is doing work that violates the model's own falsifiability claims. If S3 is defined as "self-efficacy collapse *plus* existential threat," then:

- A person in high-stakes domain whose AI-capable colleague outperforms them (clear self-efficacy hit, no existential framing) enters what state? If it's still S3, the "plus" is decorative. If it's not S3, the model should have a separate state for self-efficacy-only shock.
- A person confronted with their own replaceability in a low-stakes domain (existential threat, no professional identity at stake) enters what state? Terror management theory predicts defensive reactions. Is that S3 or S2D or something else?

**Conflict:** V4 called S3 "the emotional core of the model." V5 inherits that claim but adds two mechanisms without specifying which one(s) are sufficient. The model's transition table for S3 (Low × D1 = mild surprise, Low × D4 = curiosity, High × D2 = discomfort, High × D3 = identity crisis, High × D4 = existential) looks like it's modulating a *single underlying response* by stakes and delegation level, not *combining two independent mechanisms*. If the response scales smoothly across the axes, why would two distinct mechanisms compound rather than one dominating?

**Falsifiability problem:** Because the anchor is compound and underspecified, any S3 observation can be explained by allocating it differently between self-efficacy and terror management after the fact. If a subject shows anxiety without existential dread, you invoke the first mechanism. If a subject shows existential dread without job-loss anxiety, you invoke the second. The anchor doesn't predict which subjects will manifest which mixture. It's a post-hoc explanation machine, not a predictive tool.

**Recommendation:** Either (a) make S3 a single mechanism — "self-efficacy collapse in a valued domain" (simpler and more testable) — and move existential-threat cases to a separate consideration or state. Or (b) specify a decision rule: "If a person exhibits existential confrontation without domain-specific capability threat, the primary mechanism is X, not terror management." Right now it's neither.

---

### 2. S2T: Calibration anchor misses the central claim

**The claim:** S2T (Trust Evaluation) is anchored to "calibration under uncertainty — the cognitive process of updating subjective probability estimates against observed evidence. Closely tied to the Technology Acceptance Model (Davis, 1989 — the idea that adoption is driven by perceived usefulness and perceived ease of use)."

**Fit problem:** Calibration is a *neutral process* — updating estimates toward reality regardless of direction. But the model treats S2T as specifically *non-defensive*. The claim is "systematic testing on known problems, comparing AI output to personal output, evaluating reliability, calibrating expectations" with "asymmetric updating" as the only marker that separates S2T from S2D.

But calibration theory (Lichtenstein, Fischhoff) doesn't predict non-defensiveness. It predicts that people update in response to evidence. S2D updates defensively; S2T updates fairly. Both are updating. Both are calibrating. The anchor doesn't explain why S2T avoids the asymmetric updating that defines S2D.

**Conflict:** The model claims S2T is reached from S1 when "Identity Stakes are low" and S2D is reached when "Identity Stakes are high." But if both states are calibration processes, stakes shouldn't determine the mechanism — it should determine the direction of bias. Low-stakes users should still be capable of defensive updating; high-stakes users should be capable of fair evaluation. The anchor suggests S2T is a *different mechanism* when it's really the *same mechanism with different initial conditions*.

The Technology Acceptance Model gloss doesn't help — TAM is silent on the S2T/S2D distinction. TAM just says people adopt based on usefulness and ease; it says nothing about whether they're defending an identity while they evaluate usefulness.

**Falsifiability problem:** If calibration is the anchor, the model should predict that identity-threat context (which shouldn't matter to a pure calibration process) doesn't predict S2T vs. S2D. But the model explicitly claims Identity Stakes *do* predict the fork. That's a contradiction the anchor glosses over.

**Recommendation:** Reframe the anchor as "risk appraisal under selective attention" or "motivated evaluation" — a process where the same updating machinery is pointed toward different evidence depending on stakes. Or drop the pretense of a mechanism anchor and just say S2T and S2D are a fork driven by Identity Stakes, with different evaluative strategies as the behavioral consequence. A mechanism that doesn't distinguish between the two states isn't earning its place.

---

### 3. S2D: Identity-protection anchor is solid, but leaves a gap

**The claim:** S2D (Defensive Resistance) is anchored to "identity-protection cognition — the tendency to evaluate evidence in ways that defend a valued self-concept. Dan Kahan's term in the political-belief literature; the same mechanism applies to professional identity under capability threat. Festinger's cognitive dissonance (the discomfort of holding two beliefs that contradict each other) is the older and broader framing of the same dynamic."

**Fit:** Good. This is the right mechanism. Kahan's work on "cultural cognition" and Festinger's dissonance are both solid fits for the described behavior (nitpicking, downplaying strengths, highlighting weaknesses, asymmetric evidence updating). The model's claim that S2D "discounts positive evidence and amplifies negative evidence" is exactly what identity-protection cognition predicts.

**Conflict:** Minor. The model describes S2D as "the behavior can look identical to S2T from outside; the difference is asymmetric updating." This is true *as a mechanism*, but the claim is weaker than it seems. If an outside observer sees someone systematically finding flaws in AI, they can't tell whether the person is (a) doing fair evaluation and finding real problems, or (b) defending an identity. The asymmetric-updating heuristic distinguishes the two only in longitudinal data, which limits the model's snapshot-level utility. This isn't a flaw in the anchor — it's a limitation of the state itself.

**Falsifiability:** Good. Identity-protection cognition predicts specific updating biases and their dependence on domain relevance. The model could test this: measure how the same person's evaluation of AI shifts when the AI threatens different domains (high-stakes vs. low-stakes). The mechanism is falsifiable.

No recommendation on this one. The anchor is doing real work here.

---

### 4. S3B: Scope-limitation anchor is specific and good

**The claim:** S3B (Bargaining) is anchored to "cognitive dissonance reduction via scope limitation. When the dissonance between 'I am skilled at X' and 'AI is also skilled at X' cannot be resolved by demoting AI, the person resolves it by demoting the scope of 'X' — narrowing what they will use AI for so the remaining domain still belongs to them."

**Fit:** Excellent. This is Festinger's dissonance mechanism applied with surgical precision. The predicted behavior matches exactly: the person creates a boundary ("I'll use it for drafting, not for final output") that preserves identity while reducing contradiction. This is more specific and testable than generic "dissonance reduction."

**Conflict:** None. The transitions and triggers described for S3B all align with what dissonance-reduction theory predicts.

**Falsifiability:** Good. The model includes a heuristic to distinguish S3B from S7A (mature bounded adoption): "In S3B, boundaries are renegotiated under capability pressure. When a new model release crosses one of the self-imposed lines, the line moves quickly without documented testing. In S7A, boundaries move only after measured evidence." This is testable across model releases, though it requires longitudinal observation.

No recommendation. This is a good example of what mechanism anchoring should look like.

---

### 5. S5: Dual-component stability claim has no mechanism anchor at all

**The claim:** S5 (Understanding) is anchored to "schema integration — the cognitive process by which a new tool is incorporated into existing mental models of work, rather than competing with them." But the model then immediately adds: "Stability has two components, both required: (1) Internal reframing — personal mental model is coherent. (2) Social normalization — surrounding environment treats AI use as unremarkable."

**Fit problem:** Schema integration is a *cognitive* mechanism (how the individual's mind reorganizes). But the model claims S5 stability requires *both* internal reframing *and* social normalization — which is a cognitive + social claim. The anchor only explains one half.

More problematically, the model then says: "*Note: the dual-component requirement is currently conjecture. No instrument is specified for either component, and any observed discomfort can be attributed to mismatch.*"

This is suspicious. The most falsifiable claim in the model — S5 requires social normalization, not just individual cognition — has no mechanism anchor and is explicitly marked as conjecture. Meanwhile, less falsifiable claims get mechanism anchors. Either the dual-component stability is important enough to anchor and defend, or it's conjecture that belongs in the "Limits of operationalization" section and not in the state description itself.

**Conflict:** The model gives schema integration a leading role in S5 stability, but every mechanism anchor after S5 (S6A–D, S7A–F) describes how the person's internal model and external pressures can diverge. If schema integration is supposed to create stable internal coherence, why are S6B (dependent overuse from eroded self-efficacy) and S6D (social overuse from peer pressure) so common downstream of S5? The model should predict these are failures or regressions from S5. Instead, it treats them as distinct outcomes. The anchor doesn't explain that.

**Falsifiability:** Minimal. Schema integration is too broad. Any sustained AI use could be retrofitted as "tool incorporation into existing mental models." The model doesn't say what would count as schema integration *failing*, or what role social normalization plays relative to internal reframing. The conjecture note correctly flags that this is unmeasurable as written.

**Recommendation:** Either (a) reframe S5's anchor to explicitly include social-context mechanisms (Rogers' diffusion of innovations talks about this — peer-adoption context shapes perceived compatibility). Or (b) split S5 into two claims: "schema integration" for the individual cognitive side, and "social normalization" for the external side, each with its own anchor and falsifiability threshold. Right now S5 is smuggling a two-mechanism anchor under a one-mechanism name, the opposite of the S3 problem.

---

### 6. S6A: Variable-reward anchor is correct but incomplete

**The claim:** S6A (Enthusiastic Overuse) is anchored to "variable-reward reinforcement — the intermittent-reward dynamic that underlies compulsive engagement with any tool whose outputs are unpredictably good. Sometimes the AI produces something exceptional, sometimes mediocre; the unpredictability is what sustains the behavior."

**Fit:** Good. This is solid behavioral-psychology grounding. Variable-ratio reward schedules do produce sustained, high-rate behavior — it's why slot machines work and why people check social media compulsively. The claim that "every workflow gets routed through AI even when it is the wrong tool for the task" is exactly what variable-reward schedules predict.

**Conflict:** Minor. The model claims S6A is "energy, productive, and uncritical" but variable-reward theory doesn't predict uncriticalness — it just predicts sustained engagement. A person could be engaged *and critical*, running hypothesis tests on the AI's outputs to refine their own sense of when it's good. The "uncritical" part might be caused by high dopamine states, but that's a separate mechanism (reward-based motivation) not encoded in the anchor.

**Falsifiability:** Good. The model predicts that variability of output quality sustains S6A engagement. You could test this: low-variance AI (consistently good) should exit S6A faster than high-variance AI (good sometimes, mediocre sometimes), all else equal. But the model doesn't make that explicit.

No change needed, but the recommendation is: if you want to deepen the anchor, add a prediction about what breaks S6A engagement — is it predictability (outputs become consistently mediocre), or is it something else?

---

### 7. S6B: Self-efficacy-displacement anchor misnames the mechanism

**The claim:** S6B (Dependent Overuse) is anchored to "self-efficacy displacement — confidence in the AI replaces, rather than supplements, confidence in self. Bandura's construct in reverse: instead of mastery experiences building self-efficacy, repeated outsourcing erodes it. Each successful AI completion is silent evidence that the person's contribution wasn't necessary."

**Fit problem:** This is not Bandura's self-efficacy mechanism; it's a **learned-helplessness** mechanism (Seligman, Maier). Learned helplessness happens when a person repeatedly finds their own actions are ineffective (the AI solves the problem; their input wasn't needed), and they stop trying. Bandura's self-efficacy is about mastery experiences building confidence in one's own ability to handle challenges.

The model is describing learned helplessness — repeated outsourcing breaks the person's sense that their actions matter. That's correct psychology. But Bandura didn't predict this outcome. Bandura would predict that if AI eliminates the person's mastery experiences, they lose confidence in that domain and retreat to domains where they still have mastery experiences. They might become dependent on AI in one domain while maintaining efficacy in others. Learned helplessness predicts they lose the belief that effort itself matters — a deeper breakdown.

**Conflict:** Significant. If S6B is learned helplessness, it should have different transitions than the model predicts. Learned helplessness predicts passivity and giving up (consistent with the transitions to S3 Ego Shock and S7D Burnout). But it *also* predicts that people in learned helplessness don't re-engage easily, because they've learned that engagement doesn't work. The model lists a transition to "S7A Maturity — rare but possible when the person rebuilds independent judgment alongside AI use." That transition is actually *very hard* under learned-helplessness conditions — you need external intervention to break the helplessness, not just time. The anchor doesn't predict the difficulty.

**Falsifiability:** Weak. The anchor could be tested (does repeated outsourcing erode agency beliefs?), but the model doesn't specify how to measure "confidence in self" or how to distinguish it from identity threat in S3. Without operational definitions, it's vague.

**Recommendation:** Either (a) retitle S6B as "Learned-helplessness overuse" and cite Seligman/Maier instead of Bandura, and revise the transitions to reflect the actual difficulty of escape. Or (b) reframe the anchor as "efficacy displacement" but specify: "confidence in the AI replaces confidence in self specifically for *this task*; confidence in other domains may remain intact." Bandura's concept is actually useful once you localize it to domain-specific efficacy rather than global confidence erosion.

---

### 8. S6C: Goal-substitution anchor is plausible but under-specified

**The claim:** S6C (Driven Overuse) is anchored to "goal-substitution — efficiency, originally a means to other goals (more output, better life balance, career advancement), becomes a terminal goal in itself. Adjacent literature: the cognitive-psychology work on goal hierarchies and the documented tendency of subgoals to displace the superordinate goals they were meant to serve."

**Fit:** Plausible. Goal hierarchies do show subgoal creep in organizational psychology and decision science. The claim that efficiency becomes terminal is a reasonable prediction in high-performance cultures. But plausibility isn't fit — fit is whether this is the *best* explanation for S6C, or whether you reached for a familiar mechanism after seeing the behavior.

**Conflict:** Real. Goal-substitution theory predicts that when the subgoal (efficiency) becomes terminal, people optimize for the subgoal even when it damages the superordinate goal. The model predicts S6C transitions to S7D Burnout because "there is no natural ceiling on 'more efficient,' so the person runs until depleted." This is correct — the person keeps optimizing efficiency even past the point where it damages their health or output quality. But the anchor should predict this outcome explicitly. Instead it just describes the mechanism without drawing the failure mode.

**Falsifiability:** Moderate. Goal-substitution is testable (people in S6C should report that efficiency is now a goal in itself, not a means to other goals), but the model doesn't specify how to measure the difference between "I want to be efficient" and "efficiency-as-itself-matters." Self-report is the only instrument available, which contaminates the test.

**Recommendation:** Add a testable prediction: "S6C users will continue using AI to optimize efficiency even when the superordinate goal (career advancement, life balance) would be better served by stopping." This is already implied, but making it explicit gives the anchor actual falsifiability. Also, specify how you'd measure "goal substitution" — perhaps by asking people to rank their reasons for AI use at different timepoints, watching efficiency rise relative to other goals.

---

### 9. S6D: Normative social influence anchor is standard but narrow

**The claim:** S6D (Social Overuse) is anchored to "normative social influence — behavior change driven by the desire to match peer behavior, independent of personal evaluation of the behavior's merit. Asch's classic conformity work is the canonical reference; the modern variant is the documented tendency of professionals to adopt tools their peers visibly use even when their own work doesn't require them."

**Fit:** Good. Asch's conformity paradigm and the broader social influence literature clearly predict this behavior. The claim is well-grounded.

**Conflict:** None. The transitions align with what conformity theory predicts: S6D exits into S5 Understanding (when peer pressure fades) or S7D Burnout (when pressure persists past capacity) or drifts to S6A (when external pressure converts to internal enthusiasm). All reasonable.

**Falsifiability:** Moderate. Normative social influence is testable — remove the peer reference (change teams, roles, social context) and S6D users should reduce AI usage faster than S6A or S6C users. But the model doesn't explicitly predict this. It should.

No major recommendation, but: add a prediction that S6D is more *context-dependent* than S6A or S6C. Change the peer context, and S6D collapses. Change the AI tool's capability, and S6A and S6C may persist. This would be a falsifiable distinction between S6 states.

---

### 10. S7A: Metacognitive calibration anchor is excellent

**The claim:** S7A (Maturity) is anchored to "metacognitive calibration — accurate self-assessment of when one's own judgment is better than the tool's. The mature user has an internal model of the tool's failure modes (where it hallucinates, where it sycophants, where it confidently averages out the interesting answer) and routes work to avoid those modes."

**Fit:** Excellent. This is precise. Metacognitive calibration is Lichtenstein and Fischhoff's work on confidence-accuracy alignment. The model correctly predicts that S7A users have a *working model of the tool's failure modes*, not just general confidence. This is much more specific than "calibration under uncertainty" for S2T.

**Conflict:** None. The transitions and behavioral claims align with metacognitive calibration predictions.

**Falsifiability:** Good. You could test this by asking S7A users to explain where the AI fails in their domain, comparing their explanations to actual failure patterns. S7A users should have more accurate models of failure modes than S6 users. The model predicts regression when "a capability jump invalidates the calibration" — testable by observing whether S7A users regress to S3 after model releases more frequently than the baseline.

No recommendation. This is a good example of mechanism anchoring done right.

---

### 11. S7B: Extended-self anchor is too broad to be falsifiable

**The claim:** S7B (Identity Expansion) is anchored to "extended-self / tool incorporation — the documented tendency of humans to incorporate tools into their self-concept. The carpenter and the hammer; the writer and the typewriter; the photographer and the camera. With AI the integration is deeper because the tool participates in cognition rather than just executing it, which is why the identity claim feels different from 'I'm good with Photoshop.' Adjacent literature: Belk's work on the extended self in consumer behavior; the broader phenomenology-of-technology literature on tool-self continuity."

**Fit problem:** Extended-self is *too broad*. Every person who uses a tool regularly will incorporate it into their self-concept to some degree. The carpenter doesn't think "I am the person who operates this hammer"; they just become better at carpentry. The model claims S7B is "partly defin[es] themselves through this expansion" — but extended-self theory doesn't predict *identity centrality*, it predicts that tools become familiar and reliable and feel like an extension of the body/mind.

The distinction the model tries to make is: "A novelist who uses AI carefully to polish their voice is in S7A; a person who couldn't write fiction before AI and now identifies as a writer-with-AI is in S7B." But that distinction is *identity-creation*, not *tool incorporation*. It's a different mechanism — the tool enabled a capability that became identity-constitutive. Extended-self doesn't predict that some tools become identity-constitutive and others don't.

**Conflict:** Real. The model treats S7B as a distinct end state from S7A (maturity), but if both are tool-incorporating, the difference must be something other than incorporation. The model says the difference is *identity expansion* — doing something you couldn't before and making it part of who you are. But "extended-self" doesn't predict that. Belk's extended-self is about *possessions* (I identify with my car, my clothes, my collection), not about *capabilities*. The model is using a consumer-behavior mechanism to explain cognitive capability-identity fusion. That's a mismatch.

**Falsifiability:** Very weak. The anchor allows any identity-shift post-AI to be classified as S7B. There's no prediction of what wouldn't count as S7B. If a person uses AI to improve a skill they already had (which the model says is S7A), could that still be identity-strengthening (which sounds like S7B)? The model doesn't say. The anchor is post-hoc — you see someone calling themselves "a writer-with-AI" and assign them to S7B, but the anchor doesn't predict when this identity claim will arise.

**Recommendation:** Either (a) drop the extended-self anchor and reframe S7B as "*capability-driven identity expansion* — the process by which newly enabled capabilities become identity-constitutive, particularly when the person couldn't perform at that level before the tool." This is more specific. Or (b) keep extended-self but add a falsifiable criterion: "S7B users will report that the AI is so fundamental to their capability that losing it would require rebuilding their sense of what they can do. S7A users will report that losing the AI would require changing their workflow, but not their sense of self." This distinguishes incorporation (which is about being skilled) from identity-fusion (which is about being).

---

### 12. S7C: Meaning-making anchor is vague

**The claim:** S7C (Ethical/Philosophical Integration) is anchored to "meaning-making — the broader cognitive process of integrating a personally significant experience into a coherent worldview. Adjacent literature: post-traumatic growth research, which documents that confrontation with destabilizing experience can yield a more articulated worldview rather than a return to the prior state."

**Fit problem:** Meaning-making is *way too broad*. Any reflection on AI could be meaning-making. The model says S7C is "sustained reflection on bias, intellectual property, authenticity, labor displacement, environmental cost, societal effects." But why is that meaning-making rather than just *thinking about ethics*? Meaning-making in the post-traumatic-growth literature means integrating trauma into a revised sense of life purpose and worldview. The model treats S7C as sustained ethical thinking, which might or might not involve meaning-making in that deep sense.

**Conflict:** Real. The model says "When it appears alone, the person typically uses AI minimally and treats engagement with the technology as primarily a thinking subject." This suggests S7C is characterized by *minimal use* despite ethical reflection — i.e., the person's thinking leads them *away from* AI use. But meaning-making doesn't predict withdrawal; it predicts integration. The model's description of S7C as "rarely a sole end state" and usually co-occurring with S7A or S7B suggests the genuine psychological process is *ethical deliberation within continued use*, not meaning-making in the integrative sense. The anchor doesn't fit the behavior.

**Falsifiability:** Weak. You can't test "meaning-making" without asking the person what their worldview now includes about AI. But that's self-report contamination. The model would need to specify what observable behavior changes would count as evidence of meaning-making — perhaps public advocacy, changed ethical boundaries, specific life changes in response to AI ethical concerns. Without that, it's just a name for "thinking about ethics."

**Recommendation:** Reframe as "*ethical deliberation and stance-taking* — the process by which people develop and articulate their own ethical positions on AI use, often making those positions visible to others." This is more grounded in behavior. Or, if meaning-making is the right concept, add a prediction: "S7C users will report that their understanding of themselves and society has shifted as a result of engaging with AI ethics questions." Test that with longitudinal interviews.

---

### 13. S7D: Resource-depletion anchor is solid

**The claim:** S7D (Burnout / Withdrawal) is anchored to "resource depletion in the cognitive-control sense — sustained high-effort engagement (whether enthusiastic in S6A, anxious in S6B, driven in S6C, or socially compelled in S6D) draws on finite regulatory resources. When depletion crosses a threshold, withdrawal restores the resource. Adjacent literature: the cognitive-control fatigue research and the broader burnout literature in occupational psychology (Maslach), allowing for the unresolved debate about whether 'depletion' is a literal energy mechanism or a motivation shift."

**Fit:** Good. This is standard burnout theory. Ego depletion (Baumeister) or resource depletion (Maslach) are well-established mechanisms for withdrawal after sustained high-effort engagement. The model correctly notes the debate about whether this is a literal energy mechanism or a motivation shift — that intellectual honesty is valuable.

**Conflict:** Minimal. The model claims S7D is "reachable from any S6 state and from sustained S7B or S7F intensity." This aligns with depletion theory — high-effort states (whether driven by reward, anxiety, goals, or social pressure) deplete resources. That's correct.

**Falsifiability:** Moderate. You could test whether S7D exits are shorter after vacations or other recovery periods (supporting literal depletion) or whether they're driven by *meaning* shifts (supporting motivation-shift view). The model could make this testable by specifying what kind of recovery breaks the depletion — rest, meaning change, or both?

No major recommendation, but: the phrase "allowing for the unresolved debate" is appropriate intellectual honesty. Strengthen it by saying what difference it would make: "If depletion is literal, S7D users will recover with rest. If depletion is motivation-driven, they'll recover only if the meaning of AI in their work changes."

---

### 14. S7F: Generativity anchor is correct but under-defended

**The claim:** S7F (Influence / Evangelism) is anchored to "generativity (Erikson's term, broadened from its original developmental-stage context — the drive to invest in the next cohort's success). The same mechanism that explains why senior practitioners across many domains turn to mentoring and teaching once their own competence is settled. AI provides an unusually sharp opportunity for this because the cohort needing guidance is large and the experience required to guide them is a few years rather than a few decades."

**Fit:** Good. Erikson's generativity is a real thing. The model's claim that it's particularly pronounced in AI adoption (because there's a large cohort learning rapidly) is reasonable.

**Conflict:** Real. The model includes a note: "*Note: the 'S3 prerequisite for stable S7F' claim is currently conjecture. A future longitudinal study could refute it by documenting stable S7F users who never passed through identity-disruptive AI experiences.*" This note admits the anchor doesn't predict one of the model's own claims. If generativity is the mechanism, why would prior identity disruption be necessary? Erikson's theory doesn't predict that. The model is adding a *constraint* that the anchor doesn't support.

**Falsifiability:** Weak. The model correctly identifies this as conjecture — the claim that S3 is a prerequisite for stable S7F is unmeasured. This is intellectual honesty, but it means the anchor isn't carrying the weight of the state description. The anchor is generativity; the actual predictor might be "prior identity threat + current expertise + desire to help," which is more complex.

**Recommendation:** Either (a) keep the conjecture note and accept that S7F's transitions are partially unanchored — which is fine, but weakens the version-bump claim. Or (b) extend the anchor to include "integration of prior identity disruption into a coherent new identity," which would ground the S3-prerequisite claim. Right now the anchor under-specifies the mechanism.

---

### 15. Dropout: Practical severity (expectancy violation) is straightforward; emotional severity (threat-driven avoidance) is too broad

**The claim:** Practical dropout is "expectancy violation in the usability sense. The tool failed to do what its perceived capability promised. Emotional severity → threat-driven avoidance. Continuing use predicts further psychological cost, so the person stops."

**Fit problem:** Expectancy violation for practical dropout is solid — the tool didn't work as expected. But "threat-driven avoidance" for emotional dropout is underspecified. The model identifies threat as the cause, but threat exists in S2D, S3, and S3B as well. What distinguishes emotional dropout from those states?

The model's "operational test (the reversibility check)" is supposed to disambiguate: "Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit." But this test has confounds:

- If someone drops out due to identity threat (S3) and you give them a better tool, they might still not restart because the threat remains. The tool quality doesn't matter if the person's sense of self is still disrupted.
- If someone drops out due to social pressure (S6D) and that pressure is removed, they'll restart even if the tool is mediocre. The tool quality isn't the determining factor.

**Conflict:** Real. The emotional-severity anchor treats dropout as avoidance of continued psychological cost. But S3B is *not dropout* — it's bounded adoption where the person uses the tool within narrow limits *because* identity threat persists. So what's the difference between "S3B uses the tool for X but avoids Y due to threat" and "emotional dropout avoids the tool entirely due to threat"? The model doesn't say. The anchor should predict that boundary-setting (S3B) is driven by the same mechanism as withdrawal (emotional dropout), just with different outcomes.

**Falsifiability:** Moderate. The reversibility test is executable, but it's contaminated by multiple causes. You'd need to control for whether the threat itself is resolved (new role, time, external validation). Without that control, "they still won't use it even with a better tool" could mean emotional threat, or social pressure, or learned helplessness, or identity shift. The mechanism anchor doesn't disambiguate.

**Recommendation:** Redefine emotional dropout as "withdrawal driven by identity threat, efficacy threat, or sustained regulatory depletion — conditions where the threat itself must be resolved or the person won't re-engage." This is more specific than "threat-driven avoidance." Then specify what conditions would resolve each type of threat: identity threat requires either identity reconstruction or domain-irrelevance; efficacy threat requires efficacy-building or domain shift; depletion requires rest or meaning change. Without specifying recovery conditions, the anchor is just a label.

---

### 16. S1: Novelty appraisal anchor is reasonable but not falsifiable for this state

**The claim:** S1 (Initial Encounter) is anchored to "novelty appraisal — the brain's first-pass classification of an unfamiliar stimulus as relevant or irrelevant, threatening or benign. Standard cognitive-appraisal terrain (Lazarus and Folkman's work on stress appraisal is the closest classical reference: people first decide *what is this and does it matter to me*, then decide *what can I do about it*)."

**Fit:** Reasonable. Lazarus's appraisal theory is the standard model for how people respond to new stimuli. First, appraisal; then, coping response.

**Falsifiability:** Very weak. The model claims S1 is "stance is unformed" and "emotional flavor (curiosity, skepticism, threat) depends on Identity Stakes, not on this state itself." But if emotional flavor depends on Identity Stakes, then appraisal isn't a state-level mechanism — it's determined by the axes. The anchor is doing no work for the state itself. You can't test S1's appraisal mechanism independently of the axes that determine what the appraisal concludes.

**Conflict:** Minor. The model says S1 can transition directly to S5 Understanding "for low stakes with prior conceptual familiarity." But novelty appraisal should proceed through S2T or S2D evaluation before reaching Understanding — appraisal is just the initial classification, not the full evaluation. The direct S1→S5 path suggests something other than appraisal is operating (maybe prior schema compatibility?). The anchor doesn't explain it.

**Recommendation:** Either accept that S1 is a placeholder state whose transitions are fully determined by the axes, with no novel mechanism of its own. Or add a specificity: "Novelty appraisal for S1 predicts that the speed of exit to S2T/S2D/S5 depends on prior familiarity with the class of tool (if you know what an AI assistant is, appraisal is quicker)." This would give the anchor actual predictive power.

---

## Recommendations

### Priority 1: Fix S3's compound anchor

S3 is the emotional core of the model. V5 anchors it to "self-efficacy collapse *plus* terror management," but doesn't specify which is primary or what happens when they come apart. The compound anchor defers the hard question and makes S3 unfalsifiable.

**Action:** Specify a decision rule. Either:
- (a) Make S3 primarily self-efficacy collapse in a valued domain; move existential-threat cases to a separate frame or state.
- (b) Specify what initiates terror management vs. efficacy collapse: "If a person faces capability replacement (AI does my job), the primary mechanism is efficacy collapse. If a person confronts replaceability (I have no unique role), the primary mechanism is terror management. Both occur in high-stakes/high-delegation contexts, but the transition behavior differs [specify how]."
- (c) Provide a timeline: "Initially (Day 1), appraisal triggers efficacy collapse. If the person can't downgrade AI's capability or narrow their identity, existential threat emerges after 2–4 weeks of continued exposure."

Pick one and defend it.

### Priority 2: S2T/S2D fork is under-anchored

S2T is anchored to "calibration under uncertainty," but calibration theory doesn't predict non-defensiveness. S2D is anchored to "identity-protection cognition," which is good. But the fork is triggered by Identity Stakes, which means the *same cognitive process* (calibration) is pointed toward different evidence depending on stakes. The anchors should reflect that.

**Action:** Reframe S2T's anchor as "risk appraisal under evaluative context" or "motivated evaluation of utility and ease-of-use." This acknowledges that both S2T and S2D are calibration processes, but contextually different in stakes. Or drop the separate anchor for S2T and just say: "The S2T/S2D fork is determined by Identity Stakes; both states involve testing the tool, but identity threat determines whether the testing is fair or defensive." This is more honest about what the model is actually claiming.

### Priority 3: S5's dual-component stability needs anchoring or downgrading

S5's "internal reframing + social normalization" is the most falsifiable claim in the model but has no mechanism anchor and is marked as conjecture. This is backwards. Either anchor it (with a mechanism explaining why both components are necessary) or move it entirely to the "Limits of operationalization" section and drop it from the state description.

**Action:** If you keep the dual-component claim, add a social-mechanism anchor: "Schema integration (cognitive) + social normalization (external). Schema integration is how the individual mental model accommodates the tool. Social normalization is how the surrounding environment treats tool use as unremarkable, reducing the person's sense of standing out or being deviant. Both are necessary because internal coherence without social validation leads to S6D (social pressure-driven overuse), and social validation without internal reframing leads to S2D (defensive adoption)."

Or drop the dual-component claim from S5 itself and say: "S5 is schema integration; social normalization is a contextual factor that accelerates exit from S5 but is not constitutive of the state."

### Priority 4: Reframe S7B's anchor or tighten the definition

"Extended-self" is too broad to distinguish S7B (identity expansion) from S7A (mature bounded adoption of an existing identity). Both incorporate the tool; the difference is whether the tool enables a *new identity* or serves an *existing identity*.

**Action:** Reframe as "capability-driven identity expansion — acquiring a capability via AI that becomes identity-constitutive because it was previously out of reach." Then add a falsifiable boundary: "S7B users will report that the capability is now part of how they see themselves (e.g., 'I'm a writer now'). S7A users will report that the capability is how they practice their existing role better (e.g., 'I'm a better writer')." Test by asking people to describe what changes about their sense of self vs. their sense of their skills.

### Priority 5: Strengthen S7F's S3-prerequisite claim or drop it

The model claims S3 (identity disruption) is a prerequisite for stable S7F (evangelism), but the generativity anchor doesn't predict this. This is marked as conjecture — which is honest — but it creates a gap where the anchor doesn't carry the state description.

**Action:** Either (a) accept that S7F's transitions are partially unanchored and remove the S3-prerequisite from the state description, treating it as a heuristic rather than a structural claim. Or (b) extend the anchor to "generativity post-identity-disruption," and specify what role prior S3 experience plays: "People who've passed through S3 can authentically guide others through it because they've lived it. Their evangelism is grounded in lived experience rather than naïveté." Then test whether S7F speakers without S3 history are perceived as less credible or effective.

### Priority 6: Clarify dropout's emotional-severity mechanism

Emotional dropout is anchored to "threat-driven avoidance," but threat exists in S2D, S3, and S3B as well. The anchor needs to specify what kind of threat triggers withdrawal rather than boundary-setting.

**Action:** Redefine emotional dropout as "withdrawal driven by threat-recovery-blocking conditions — situations where the person perceives no path to resolving the threat (identity won't shift, efficacy can't rebuild, pressure won't relent)." Then add recovery conditions for each: identity threat→identity reconstruction or domain shift; efficacy threat→efficacy-building or role change; pressure→context change or network shift. The "reversibility test" should then predict that emotional dropouts won't return until recovery conditions are met, even with a better tool.

### Priority 7: Add falsifiable predictions to anchors that currently lack them

Most anchors are post-hoc descriptions. S3B (scope limitation), S7A (metacognitive calibration), and S7D (resource depletion) earn their anchors by predicting something. The others should too:

- **S6A (variable-reward):** Predict that low-variance AI (consistently good output) causes faster exit than high-variance AI.
- **S6C (goal-substitution):** Predict that S6C users will optimize efficiency past the point where it damages their superordinate goals.
- **S2D (identity-protection):** Predict that S2D users will re-evaluate the tool more fairly if you first affirm their identity in the domain.

### Priority 8: Acceptance — some anchors are decorative and that's OK

S1's novelty appraisal and S7C's meaning-making are post-hoc. They describe the states correctly but don't predict anything the model doesn't already claim. This doesn't make V5 wrong — descriptive models are valuable. But it does mean the version-bump claim ("mechanism anchoring justifies V5") is overstated. V5 is an improved descriptive model with *some* mechanistic grounding, not a mechanistic model that happens to describe behavior well.

**Action:** In a V5 discussion or follow-up, reframe the achievement: "V5 adds mechanism anchoring to improve credibility and to ground future empirical work. Some anchors (S3B, S7A) make strong falsifiable predictions. Others (S1, S7C) are primarily descriptive. All of them provide handholds for the next version to test." This is honest and sets better expectations for V6.
