# Mechanism Anchor Audit — Model V5

## TL;DR

- **S3 Ego Shock's compound anchor (self-efficacy + terror management) is a hedge, not defensible.** V5 avoids saying which mechanism is primary, creating falsifiability ambiguity: if S3 Ego Shock appears without existential dread, is it S3 Ego Shock or something else?
- **S7B Identity Expansion's "extended-self" anchor is too broad.** Every identity-shift after AI exposure gets retrofitted as "tool incorporation"; the model doesn't say what wouldn't count as S7B Identity Expansion.
- **S2T Trust Evaluation's "calibration" anchor obscures the key claim.** Calibration is neutral updating; S2T Trust Evaluation should be non-defensive updating. But calibration theory doesn't predict that distinction, so the anchor doesn't explain why S2T Trust Evaluation avoids the asymmetry defining S2D Defensive Resistance.
- **S6A Enthusiastic Overuse and S6B Dependent Overuse have the same mechanism problem as S3 Ego Shock.** S6A Enthusiastic Overuse is "variable-reward" and S6B Dependent Overuse is "self-efficacy displacement" — but displaced toward AI, which isn't what self-efficacy psychology predicts. The anchor papers over the difference instead of defending it.
- **Dropout's mechanisms are vague.** "Threat-driven avoidance" is too broad; it could apply to S2D Defensive Resistance, S3 Ego Shock, or S3B Bargaining. The model needs to specify what kind of threat triggers withdrawal versus boundary-setting in S3B Bargaining.
- **Falsifiability gain is minimal across the board.** Most anchors are post-hoc fit — the model specifies behavior first, then attaches a mechanism name. Anchors would help if they predicted novel transitions or failure modes; instead they describe states the model already claimed.
- **S5 Understanding's dual-component stability (internal reframing + social normalization) is conjecture without a mechanism anchor.** This is the model's most falsifiable claim, yet it has no anchor. The asymmetry is suspicious.
- V5's mechanism-anchoring move is partial. Some anchors earn their place by predicting failure modes (S3B Bargaining's scope limitation, S7A Maturity's metacognitive boundaries). Most are decorative — they restate the model's claims in mechanistic language without improving predictiveness or testability. The compound anchor on S3 Ego Shock is particularly problematic: if identity threat and self-efficacy threat come apart, which one determines S3 Ego Shock transitions? Until the model answers that, S3 Ego Shock is unfalsifiable. This doesn't sink V5 — it's still a valuable descriptive framework — but it means the version-bump claim ("mechanism anchoring justifies V5") is overstated. The anchoring buys credibility, not predictive power.

## Findings

### 1. S3 Ego Shock: Compound anchor is a hedge masquerading as precision

**The claim:** S3 Ego Shock (Ego Shock) is anchored to "self-efficacy (a person's belief that they can actually do the thing) collapse under domain-specific capability threat. When AI demonstrably performs a task the person built their self-concept around, the belief that 'I can do this' no longer carries unique weight. A secondary mechanism is terror management (confrontation with one's own replaceability triggers the same kind of existential discomfort that confrontation with mortality does). The two mechanisms compound; S3 Ego Shock is rarely 'just' one of them."

**Fit problem:** The phrase "compound; S3 Ego Shock is rarely 'just' one of them" violates the model's own falsifiability standard. If S3 Ego Shock is defined as "self-efficacy collapse *plus* existential threat," then:

- A person in a high-stakes domain whose AI-capable colleague outperforms them (clear self-efficacy hit, no existential framing) enters what state? If it's still S3 Ego Shock, the "plus" is decorative. If it's not S3 Ego Shock, the model should have a separate state for self-efficacy-only shock.
- A person confronted with replaceability in a low-stakes domain (existential threat, no professional identity at stake) enters what state? Terror management theory predicts defensive reactions. Is that S3 Ego Shock or S2D Defensive Resistance or something else?

**Conflict:** V4 called S3 Ego Shock "the emotional core of the model." V5 inherits that claim but adds two mechanisms without specifying which one(s) are sufficient. The model's transition table for S3 Ego Shock (Low Stakes × D1 = mild surprise, through High Stakes × D4 = existential) looks like it's modulating a *single underlying response* by stakes and delegation level, not *combining two independent mechanisms*. If the response scales smoothly across the axes, why would two distinct mechanisms compound rather than one dominating?

**Falsifiability problem:** Because the anchor is compound and underspecified, any S3 Ego Shock observation can be explained by allocating it differently between self-efficacy and terror management after the fact. If a subject shows anxiety without existential dread, invoke the first mechanism. If a subject shows existential dread without job-loss anxiety, invoke the second. The anchor doesn't predict which subjects manifest which mixture. It's a post-hoc explanation machine.

### 2. S2T Trust Evaluation: Calibration anchor misses the central claim

**The claim:** S2T Trust Evaluation (Trust Evaluation) is anchored to "calibration under uncertainty — the cognitive process of updating subjective probability estimates against observed evidence. Closely tied to the Technology Acceptance Model (Davis, 1989 — the idea that adoption is driven by perceived usefulness and perceived ease of use)."

**Fit problem:** Calibration is a *neutral process* — updating estimates toward reality regardless of direction. But the model treats S2T Trust Evaluation as specifically *non-defensive*. The claim is "systematic testing on known problems, comparing AI output to personal output, evaluating reliability" with "asymmetric updating" as the only marker separating S2T Trust Evaluation from S2D Defensive Resistance.

But calibration theory doesn't predict non-defensiveness. It predicts that people update in response to evidence. S2D Defensive Resistance updates defensively; S2T Trust Evaluation updates fairly. Both are updating. Both are calibrating. The anchor doesn't explain why S2T Trust Evaluation avoids the asymmetric updating that defines S2D Defensive Resistance.

**Conflict:** The model claims S2T Trust Evaluation is reached from S1 Initial Encounter when "Identity Stakes are low" and S2D Defensive Resistance is reached when "Identity Stakes are high." But if both states are calibration processes, stakes shouldn't determine the mechanism — stakes should determine the direction of bias. Low-stakes users should still be capable of defensive updating; high-stakes users should be capable of fair evaluation. The anchor suggests S2T Trust Evaluation is a *different mechanism* when it's really the *same mechanism with different initial conditions*.

The Technology Acceptance Model gloss doesn't help — TAM is silent on the S2T Trust Evaluation/S2D Defensive Resistance distinction. TAM just says people adopt based on usefulness and ease; it says nothing about whether they're defending an identity while evaluating usefulness.

**Falsifiability problem:** If calibration is the anchor, the model should predict that identity-threat context (which shouldn't matter to a pure calibration process) doesn't predict S2T Trust Evaluation versus S2D Defensive Resistance. But the model explicitly claims Identity Stakes *do* predict the fork. That's a contradiction the anchor glosses over.

### 3. S2D Defensive Resistance: Identity-protection anchor is solid, but leaves a gap

**The claim:** S2D Defensive Resistance (Defensive Resistance) is anchored to "identity-protection cognition — the tendency to evaluate evidence in ways that defend a valued self-concept. Dan Kahan's work in the political-belief literature; the same mechanism applies to professional identity under capability threat. Festinger's cognitive dissonance (the discomfort of holding two beliefs that contradict each other) is the older and broader framing of the same dynamic."

**Fit:** Good. This is the right mechanism. Kahan's work on "cultural cognition" and Festinger's dissonance are both solid fits for the described behavior (nitpicking, downplaying strengths, highlighting weaknesses, asymmetric evidence updating). The model's claim that S2D Defensive Resistance "discounts positive evidence and amplifies negative evidence" is exactly what identity-protection cognition predicts.

**Conflict:** Minor. The model describes S2D Defensive Resistance as "the behavior can look identical to S2T Trust Evaluation from outside; the difference is asymmetric updating." This is true *as a mechanism*, but the claim is weaker than it seems. If an outside observer sees someone systematically finding flaws in AI, they can't tell whether the person is (a) doing fair evaluation and finding real problems, or (b) defending an identity. The asymmetric-updating heuristic distinguishes the two only in longitudinal data, which limits the model's snapshot-level utility. This isn't a flaw in the anchor — it's a limitation of the state itself.

**Falsifiability:** Good. Identity-protection cognition predicts specific updating biases and their dependence on domain relevance. The model could test this: measure how the same person's evaluation of AI shifts when the AI threatens different domains (high-stakes versus low-stakes). The mechanism is falsifiable.

### 4. S3B Bargaining: Scope-limitation anchor is specific and good

**The claim:** S3B Bargaining (Bargaining) is anchored to "cognitive dissonance reduction via scope limitation. When the dissonance between 'I am skilled at X' and 'AI is also skilled at X' cannot be resolved by demoting AI, the person resolves it by demoting the scope of 'X' — narrowing what they will use AI for so the remaining domain still belongs to them."

**Fit:** Excellent. This is Festinger's dissonance mechanism applied with surgical precision. The predicted behavior matches exactly: the person creates a boundary ("I'll use it for drafting, not for final output") that preserves identity while reducing contradiction. This is more specific and testable than generic "dissonance reduction."

**Conflict:** None. The transitions and triggers described for S3B Bargaining all align with what dissonance-reduction theory predicts.

**Falsifiability:** Good. The model includes a heuristic to distinguish S3B Bargaining from S7A Maturity (mature bounded adoption): "In S3B Bargaining, boundaries are renegotiated under capability pressure. When a new model release crosses one of the self-imposed lines, the line moves quickly without documented testing. In S7A Maturity, boundaries move only after measured evidence." This is testable across model releases, though it requires longitudinal observation.

This is a good example of what mechanism anchoring should look like.

### 5. S5 Understanding: Dual-component stability claim has no mechanism anchor at all

**The claim:** S5 Understanding (Understanding) is anchored to "schema integration — the cognitive process by which a new tool is incorporated into existing mental models of work, rather than competing with them." But the model then immediately adds: "Stability has two components, both required: (1) Internal reframing — personal mental model is coherent. (2) Social normalization — surrounding environment treats AI use as unremarkable."

**Fit problem:** Schema integration is a *cognitive* mechanism (how the individual's mind reorganizes). But the model claims S5 Understanding stability requires *both* internal reframing *and* social normalization — a cognitive plus social claim. The anchor only explains one half.

More problematically, the model then says: "*Note: the dual-component requirement is currently conjecture. No instrument is specified for either component, and any observed discomfort can be attributed to mismatch.*"

This is backwards. The most falsifiable claim in the model — S5 Understanding requires social normalization, not just individual cognition — has no mechanism anchor and is explicitly marked as conjecture. Meanwhile, less falsifiable claims get mechanism anchors. Either the dual-component stability is important enough to anchor and defend, or it's conjecture that belongs in the "Limits of operationalization" section.

**Conflict:** The model gives schema integration a leading role in S5 Understanding stability, but every mechanism anchor after S5 Understanding (S6A Enthusiastic Overuse–D, S7A Maturity–F) describes how the person's internal model and external pressures can diverge. If schema integration is supposed to create stable internal coherence, why are S6B Dependent Overuse (dependent overuse from eroded self-efficacy) and S6D Social Overuse (social overuse from peer pressure) so common downstream of S5 Understanding? The model should predict these are failures or regressions from S5 Understanding. Instead it treats them as distinct outcomes. The anchor doesn't explain that.

**Falsifiability:** Minimal. Schema integration is too broad. Any sustained AI use could be retrofitted as "tool incorporation into existing mental models." The model doesn't say what would count as schema integration *failing*, or what role social normalization plays relative to internal reframing.

### 6. S6A Enthusiastic Overuse: Variable-reward anchor is correct but incomplete

**The claim:** S6A Enthusiastic Overuse (Enthusiastic Overuse) is anchored to "variable-reward reinforcement — the intermittent-reward dynamic that underlies compulsive engagement with any tool whose outputs are unpredictably good. Sometimes the AI produces something exceptional, sometimes mediocre; the unpredictability is what sustains the behavior."

**Fit:** Good. This is solid behavioral-psychology grounding. Variable-ratio reward schedules do produce sustained, high-rate behavior — it's why slot machines work and why people check social media compulsively. The claim that "every workflow gets routed through AI even when it is the wrong tool for the task" is exactly what variable-reward schedules predict.

**Conflict:** Minor. The model claims S6A Enthusiastic Overuse is "energy, productive, and uncritical" but variable-reward theory doesn't predict uncriticalness — it just predicts sustained engagement. A person could be engaged *and critical*, running hypothesis tests on the AI's outputs to refine their own sense of when it's good. The "uncritical" part might be caused by high dopamine states, but that's a separate mechanism not encoded in the anchor.

**Falsifiability:** Good. The model predicts that variability of output quality sustains S6A Enthusiastic Overuse engagement. You could test this: low-variance AI (consistently good) should exit S6A Enthusiastic Overuse faster than high-variance AI (good sometimes, mediocre sometimes), all else equal. But the model doesn't make that explicit.

### 7. S6B Dependent Overuse: Self-efficacy-displacement anchor misnames the mechanism

**The claim:** S6B Dependent Overuse (Dependent Overuse) is anchored to "self-efficacy displacement — confidence in the AI replaces, rather than supplements, confidence in self. Bandura's construct in reverse: instead of mastery experiences building self-efficacy, repeated outsourcing erodes it. Each successful AI completion is silent evidence that the person's contribution wasn't necessary."

**Fit problem:** This is not Bandura's self-efficacy mechanism; it's a **learned-helplessness** mechanism (Seligman, Maier). Learned helplessness happens when a person repeatedly finds their own actions are ineffective (the AI solves the problem; their input wasn't needed), and they stop trying. Bandura's self-efficacy is about mastery experiences building confidence in one's own ability to handle challenges.

The model is describing learned helplessness — repeated outsourcing breaks the person's sense that their actions matter. That's correct psychology. But Bandura didn't predict this outcome. Bandura would predict that if AI eliminates the person's mastery experiences, they lose confidence in that domain and retreat to domains where they still have mastery experiences. They might become dependent on AI in one domain while maintaining efficacy in others. Learned helplessness predicts they lose the belief that effort itself matters — a deeper breakdown.

**Conflict:** Significant. If S6B Dependent Overuse is learned helplessness, it should have different transitions than the model predicts. Learned helplessness predicts passivity and giving up (consistent with transitions to S3 Ego Shock and S7D Burnout). But it *also* predicts that people in learned helplessness don't re-engage easily, because they've learned that engagement doesn't work. The model lists a transition to "S7A Maturity — rare but possible when the person rebuilds independent judgment alongside AI use." That transition is actually *very hard* under learned-helplessness conditions — you need external intervention to break the helplessness, not just time. The anchor doesn't predict the difficulty.

**Falsifiability:** Weak. The anchor could be tested (does repeated outsourcing erode agency beliefs?), but the model doesn't specify how to measure "confidence in self" or how to distinguish it from identity threat in S3 Ego Shock. Without operational definitions, it's vague.

### 8. S6C Driven Overuse: Goal-substitution anchor is plausible but under-specified

**The claim:** S6C Driven Overuse (Driven Overuse) is anchored to "goal-substitution — efficiency, originally a means to other goals (more output, better life balance, career advancement), becomes a terminal goal in itself. Adjacent literature: cognitive-psychology work on goal hierarchies and the documented tendency of subgoals to displace the superordinate goals they were meant to serve."

**Fit:** Plausible. Goal hierarchies do show subgoal creep in organizational psychology and decision science. The claim that efficiency becomes terminal is a reasonable prediction in high-performance cultures. But plausibility isn't fit — fit is whether this is the *best* explanation for S6C Driven Overuse.

**Conflict:** Real. Goal-substitution theory predicts that when the subgoal (efficiency) becomes terminal, people optimize for the subgoal even when it damages the superordinate goal. The model predicts S6C Driven Overuse transitions to S7D Burnout because "there is no natural ceiling on 'more efficient,' so the person runs until depleted." This is correct — the person keeps optimizing efficiency even past the point where it damages their health or output quality. But the anchor should predict this outcome explicitly. Instead it just describes the mechanism without drawing the failure mode.

**Falsifiability:** Moderate. Goal-substitution is testable (people in S6C Driven Overuse should report that efficiency is now a goal in itself, not a means to other goals), but the model doesn't specify how to measure the difference between "I want to be efficient" and "efficiency-as-itself-matters." Self-report is the only instrument available, which contaminates the test.

### 9. S6D Social Overuse: Normative social influence anchor is standard but narrow

**The claim:** S6D Social Overuse (Social Overuse) is anchored to "normative social influence — behavior change driven by the desire to match peer behavior, independent of personal evaluation of the behavior's merit. Asch's classic conformity work is the canonical reference; the modern variant is the documented tendency of professionals to adopt tools their peers visibly use even when their own work doesn't require them."

**Fit:** Good. Asch's conformity paradigm and the broader social influence literature clearly predict this behavior. The claim is well-grounded.

**Conflict:** None. The transitions align with what conformity theory predicts: S6D Social Overuse exits into S5 Understanding (when peer pressure fades) or S7D Burnout (when pressure persists past capacity) or drifts to S6A Enthusiastic Overuse (when external pressure converts to internal enthusiasm). All reasonable.

**Falsifiability:** Moderate. Normative social influence is testable — remove the peer reference (change teams, roles, social context) and S6D Social Overuse users should reduce AI usage faster than S6A Enthusiastic Overuse or S6C Driven Overuse users. But the model doesn't explicitly predict this. It should.

### 10. S7A Maturity: Metacognitive calibration anchor is excellent

**The claim:** S7A Maturity (Maturity) is anchored to "metacognitive calibration — accurate self-assessment of when one's own judgment is better than the tool's. The mature user has an internal model of the tool's failure modes (where it hallucinates, where it sycophants, where it confidently averages out the interesting answer) and routes work to avoid those modes."

**Fit:** Excellent. This is precise. Metacognitive calibration is Lichtenstein and Fischhoff's work on confidence-accuracy alignment. The model correctly predicts that S7A Maturity users have a *working model of the tool's failure modes*, not just general confidence. This is much more specific than "calibration under uncertainty" for S2T Trust Evaluation.

**Conflict:** None. The transitions and behavioral claims align with metacognitive calibration predictions.

**Falsifiability:** Good. You could test this by asking S7A Maturity users to explain where the AI fails in their domain, comparing their explanations to actual failure patterns. S7A Maturity users should have more accurate models of failure modes than S6 users. The model predicts regression when "a capability jump invalidates the calibration" — testable by observing whether S7A Maturity users regress to S3 Ego Shock after model releases more frequently than the baseline.

This is a good example of mechanism anchoring done right.

### 11. S7B Identity Expansion: Extended-self anchor is too broad to be falsifiable

**The claim:** S7B Identity Expansion (Identity Expansion) is anchored to "extended-self / tool incorporation — the documented tendency of humans to incorporate tools into their self-concept. The carpenter and the hammer; the writer and the typewriter; the photographer and the camera. With AI the integration is deeper because the tool participates in cognition rather than just executing it, which is why the identity claim feels different from 'I'm good with Photoshop.' Adjacent literature: Belk's work on the extended self in consumer behavior; the broader phenomenology-of-technology literature on tool-self continuity."

**Fit problem:** Extended-self is *too broad*. Every person who uses a tool regularly will incorporate it into their self-concept to some degree. The carpenter doesn't think "I am the person who operates this hammer"; they just become better at carpentry. The model claims S7B Identity Expansion is "partly defin[es] themselves through this expansion" — but extended-self theory doesn't predict *identity centrality*, it predicts that tools become familiar and reliable and feel like an extension of the body or mind.

The distinction the model tries to make is: "A novelist who uses AI carefully to polish their voice is in S7A Maturity; a person who couldn't write fiction before AI and now identifies as a writer-with-AI is in S7B Identity Expansion." But that distinction is *identity-creation*, not *tool incorporation*. It's a different mechanism — the tool enabled a capability that became identity-constitutive. Extended-self doesn't predict that some tools become identity-constitutive and others don't.

**Conflict:** Real. The model treats S7B Identity Expansion as a distinct end state from S7A Maturity (maturity), but if both are tool-incorporating, the difference must be something other than incorporation. The model says the difference is *identity expansion* — doing something you couldn't before and making it part of who you are. But "extended-self" doesn't predict that. Belk's extended-self is about *possessions* (someone identifies with their car, clothes, collection), not about *capabilities*. The model is using a consumer-behavior mechanism to explain cognitive capability-identity fusion. That's a mismatch.

**Falsifiability:** Very weak. The anchor allows any identity-shift post-AI to be classified as S7B Identity Expansion. There's no prediction of what wouldn't count as S7B Identity Expansion. If a person uses AI to improve a skill they already had (which the model says is S7A Maturity), could that still be identity-strengthening (which sounds like S7B Identity Expansion)? The model doesn't say. The anchor is post-hoc — you see someone calling themselves "a writer-with-AI" and assign them to S7B Identity Expansion, but the anchor doesn't predict when this identity claim will arise.

### 12. S7C Ethical Integration: Meaning-making anchor is vague

**The claim:** S7C Ethical Integration (Ethical/Philosophical Integration) is anchored to "meaning-making — the broader cognitive process of integrating a personally significant experience into a coherent worldview. Adjacent literature: post-traumatic growth research, which documents that confrontation with destabilizing experience can yield a more articulated worldview rather than a return to the prior state."

**Fit problem:** Meaning-making is *way too broad*. Any reflection on AI could be meaning-making. The model says S7C Ethical Integration is "sustained reflection on bias, intellectual property, authenticity, labor displacement, environmental cost, societal effects." But why is that meaning-making rather than just *thinking about ethics*? Meaning-making in the post-traumatic-growth literature means integrating trauma into a revised sense of life purpose and worldview. The model treats S7C Ethical Integration as sustained ethical thinking, which might or might not involve meaning-making in that deep sense.

**Conflict:** Real. The model says "When it appears alone, the person typically uses AI minimally and treats engagement with the technology as primarily a thinking subject." This suggests S7C Ethical Integration is characterized by *minimal use* despite ethical reflection — the person's thinking leads them *away from* AI use. But meaning-making doesn't predict withdrawal; it predicts integration. The model's description of S7C Ethical Integration as "rarely a sole end state" and usually co-occurring with S7A Maturity or S7B Identity Expansion suggests the genuine psychological process is *ethical deliberation within continued use*, not meaning-making in the integrative sense. The anchor doesn't fit the behavior.

**Falsifiability:** Weak. You can't test "meaning-making" without asking the person what their worldview now includes about AI. But that's self-report contamination. The model would need to specify what observable behavior changes would count as evidence of meaning-making — public advocacy, changed ethical boundaries, specific life changes in response to AI ethical concerns. Without that, it's just a name for "thinking about ethics."

### 13. S7D Burnout: Resource-depletion anchor is solid

**The claim:** S7D Burnout (Burnout / Withdrawal) is anchored to "resource depletion in the cognitive-control sense — sustained high-effort engagement (whether enthusiastic in S6A Enthusiastic Overuse, anxious in S6B Dependent Overuse, driven in S6C Driven Overuse, or socially compelled in S6D Social Overuse) draws on finite regulatory resources. When depletion crosses a threshold, withdrawal restores the resource. Adjacent literature: cognitive-control fatigue research and the broader burnout literature in occupational psychology (Maslach), allowing for the unresolved debate about whether 'depletion' is a literal energy mechanism or a motivation shift."

**Fit:** Good. This is standard burnout theory. Ego depletion (Baumeister) or resource depletion (Maslach) are well-established mechanisms for withdrawal after sustained high-effort engagement. The model correctly notes the debate about whether this is a literal energy mechanism or a motivation shift — that intellectual honesty is valuable.

**Conflict:** Minimal. The model claims S7D Burnout is "reachable from any S6 state and from sustained S7B Identity Expansion or S7F Evangelism intensity." This aligns with depletion theory — high-effort states (whether driven by reward, anxiety, goals, or social pressure) deplete resources. That's correct.

**Falsifiability:** Moderate. You could test whether S7D Burnout exits are shorter after vacations or other recovery periods (supporting literal depletion) or whether they're driven by *meaning* shifts (supporting motivation-shift view). The model could make this testable by specifying what kind of recovery breaks the depletion — rest, meaning change, or both?

### 14. S7F Evangelism: Generativity anchor is correct but under-defended

**The claim:** S7F Evangelism (Influence / Evangelism) is anchored to "generativity (Erikson's term, broadened from its original developmental-stage context — the drive to invest in the next cohort's success). The same mechanism that explains why senior practitioners across many domains turn to mentoring and teaching once their own competence is settled. AI provides an unusually sharp opportunity for this because the cohort needing guidance is large and the experience required to guide them is a few years rather than a few decades."

**Fit:** Good. Erikson's generativity is a real thing. The model's claim that it's particularly pronounced in AI adoption (because there's a large cohort learning rapidly) is reasonable.

**Conflict:** Real. The model includes a note: "*Note: the 'S3 Ego Shock prerequisite for stable S7F Evangelism' claim is currently conjecture. A future longitudinal study could refute it by documenting stable S7F Evangelism users who never passed through identity-disruptive AI experiences.*" This note admits the anchor doesn't predict one of the model's own claims. If generativity is the mechanism, why would prior identity disruption be necessary? Erikson's theory doesn't predict that. The model is adding a *constraint* that the anchor doesn't support.

**Falsifiability:** Weak. The model correctly identifies this as conjecture — the claim that S3 Ego Shock is a prerequisite for stable S7F Evangelism is unmeasured. This is intellectual honesty, but it means the anchor isn't carrying the weight of the state description. The anchor is generativity; the actual predictor might be "prior identity threat + current expertise + desire to help," which is more complex.

### 15. Dropout: Practical severity is straightforward; emotional severity is too broad

**The claim:** Practical dropout is "expectancy violation in the usability sense. The tool failed to do what its perceived capability promised. Emotional severity → threat-driven avoidance. Continuing use predicts further psychological cost, so the person stops."

**Fit problem:** Expectancy violation (the gap between expected and actual capability) for practical dropout is solid — the tool didn't work as expected. But "threat-driven avoidance" for emotional dropout is underspecified. The model identifies threat as the cause, but threat exists in S2D Defensive Resistance, S3 Ego Shock, and S3B Bargaining as well. What distinguishes emotional dropout from those states?

The model's "operational test (the reversibility check)" is supposed to disambiguate: "Provide the dropout with a tool that demonstrably solves their cited failure. If they restart, practical severity was high. If they don't, emotional severity was driving the exit." But this test has confounds:

- If someone drops out due to identity threat (S3 Ego Shock) and you give them a better tool, they might still not restart because the threat remains. The tool quality doesn't matter if the person's sense of self is still disrupted.
- If someone drops out due to social pressure (S6D Social Overuse) and that pressure is removed, they'll restart even if the tool is mediocre. The tool quality isn't the determining factor.

**Conflict:** Real. The emotional-severity anchor treats dropout as avoidance of continued psychological cost. But S3B Bargaining is *not dropout* — it's bounded adoption where the person uses the tool within narrow limits *because* identity threat persists. So what's the difference between "S3B Bargaining uses the tool for X but avoids Y due to threat" and "emotional dropout avoids the tool entirely due to threat"? The model doesn't say. The anchor should predict that boundary-setting (S3B Bargaining) is driven by the same mechanism as withdrawal (emotional dropout), just with different outcomes.

**Falsifiability:** Moderate. The reversibility test is executable, but it's contaminated by multiple causes. You'd need to control for whether the threat itself is resolved (new role, time, external validation). Without that control, "they still won't use it even with a better tool" could mean emotional threat, social pressure, learned helplessness, or identity shift. The mechanism anchor doesn't disambiguate.

### 16. S1 Initial Encounter: Novelty appraisal anchor is reasonable but not falsifiable for this state

**The claim:** S1 Initial Encounter (Initial Encounter) is anchored to "novelty appraisal — the brain's first-pass classification of an unfamiliar stimulus as relevant or irrelevant, threatening or benign. Standard cognitive-appraisal terrain (Lazarus and Folkman's work on stress appraisal is the closest classical reference: people first decide *what is this and does it matter to me*, then decide *what can I do about it*)."

**Fit:** Reasonable. Lazarus's appraisal theory is the standard model for how people respond to new stimuli. First, appraisal; then, coping response.

**Falsifiability:** Very weak. The model claims S1 Initial Encounter is "stance is unformed" and "emotional flavor (curiosity, skepticism, threat) depends on Identity Stakes, not on this state itself." But if emotional flavor depends on Identity Stakes, then appraisal isn't a state-level mechanism — it's determined by the axes. The anchor is doing no work for the state itself. You can't test S1 Initial Encounter's appraisal mechanism independently of the axes that determine what the appraisal concludes.

**Conflict:** Minor. The model says S1 Initial Encounter can transition directly to S5 Understanding "for low stakes with prior conceptual familiarity." But novelty appraisal should proceed through S2T Trust Evaluation or S2D Defensive Resistance evaluation before reaching Understanding — appraisal is just the initial classification, not the full evaluation. The direct S1 Initial Encounter→S5 Understanding path suggests something other than appraisal is operating (perhaps prior schema compatibility?). The anchor doesn't explain it.

## Recommendations

1. **Fix S3 Ego Shock's compound anchor.** S3 Ego Shock is the emotional core of the model. V5 anchors it to "self-efficacy collapse plus terror management," but doesn't specify which is primary or what happens when they come apart. Specify a decision rule. Either (a) make S3 Ego Shock primarily self-efficacy collapse in a valued domain and move existential-threat cases to a separate frame or state, or (b) specify what initiates terror management versus efficacy collapse: "If a person faces capability replacement (AI does my job), the primary mechanism is efficacy collapse. If a person confronts replaceability (I have no unique role), the primary mechanism is terror management. Both occur in high-stakes/high-delegation contexts, but the transition behavior differs," or (c) provide a timeline: initial appraisal triggers efficacy collapse; if the person can't downgrade AI's capability or narrow their identity, existential threat emerges after weeks of continued exposure. Pick one and defend it.

2. **Reframe the S2T Trust Evaluation/S2D Defensive Resistance fork's anchors.** Reframe S2T Trust Evaluation's anchor as "risk appraisal under evaluative context" or "motivated evaluation of utility and ease-of-use." This acknowledges that both S2T Trust Evaluation and S2D Defensive Resistance are calibration processes, but contextually different in stakes. Or drop the separate anchor for S2T Trust Evaluation and just say: "The S2T Trust Evaluation/S2D Defensive Resistance fork is determined by Identity Stakes; both states involve testing the tool, but identity threat determines whether the testing is fair or defensive." This is more honest about what the model is actually claiming.

3. **Anchor S5 Understanding's dual-component stability or downgrade it.** S5 Understanding's "internal reframing + social normalization" is the most falsifiable claim in the model but has no mechanism anchor and is marked as conjecture. Either anchor it (with a mechanism explaining why both components are necessary) or move it entirely to the "Limits of operationalization" section and drop it from the state description. If you keep the dual-component claim, add a social-mechanism anchor: schema integration (cognitive) plus social normalization (external), where internal coherence without social validation leads to S6D Social Overuse and social validation without internal reframing leads to S2D Defensive Resistance.

4. **Reframe S7B Identity Expansion's anchor or tighten the definition.** "Extended-self" is too broad to distinguish S7B Identity Expansion (identity expansion) from S7A Maturity (mature bounded adoption of an existing identity). Reframe as "capability-driven identity expansion — acquiring a capability via AI that becomes identity-constitutive because it was previously out of reach." Then add a falsifiable boundary: S7B Identity Expansion users will report that the capability is now part of how they see themselves ("I'm a writer now"); S7A Maturity users will report that the capability is how they practice their existing role better ("I'm a better writer").

5. **Strengthen S7F Evangelism's S3 Ego Shock-prerequisite claim or drop it.** Either accept that S7F Evangelism's transitions are partially unanchored and remove the S3 Ego Shock-prerequisite from the state description, treating it as a heuristic rather than a structural claim. Or extend the anchor to "generativity post-identity-disruption," and specify what role prior S3 Ego Shock experience plays: people who've passed through S3 Ego Shock can authentically guide others through it because they've lived it.

6. **Clarify dropout's emotional-severity mechanism.** Redefine emotional dropout as "withdrawal driven by threat-recovery-blocking conditions — situations where the person perceives no path to resolving the threat (identity won't shift, efficacy can't rebuild, pressure won't relent)." Then add recovery conditions for each: identity threat → identity reconstruction or domain shift; efficacy threat → efficacy-building or role change; pressure → context change or network shift. The reversibility test should then predict that emotional dropouts won't return until recovery conditions are met, even with a better tool.

7. **Rename S6B Dependent Overuse and revise its transitions.** Either retitle S6B Dependent Overuse as "Learned-helplessness overuse" and cite Seligman and Maier instead of Bandura, revising the transitions to reflect the actual difficulty of escape; or reframe the anchor as "efficacy displacement" but specify: confidence in the AI replaces confidence in self specifically for *this task*; confidence in other domains may remain intact. Bandura's concept becomes useful once localized to domain-specific efficacy rather than global confidence erosion.

8. **Add falsifiable predictions to anchors that currently lack them.** Most anchors are post-hoc descriptions. S3B Bargaining (scope limitation), S7A Maturity (metacognitive calibration), and S7D Burnout (resource depletion) earn their anchors by predicting something. The others should too:
   - **S6A Enthusiastic Overuse (variable-reward):** Predict that low-variance AI causes faster exit than high-variance AI.
   - **S6C Driven Overuse (goal-substitution):** Predict that S6C Driven Overuse users will optimize efficiency past the point where it damages their superordinate goals.
   - **S2D Defensive Resistance (identity-protection):** Predict that S2D Defensive Resistance users will re-evaluate the tool more fairly if you first affirm their identity in the domain.
   - **S6D Social Overuse (normative social influence):** Predict that S6D Social Overuse is more context-dependent than S6A Enthusiastic Overuse or S6C Driven Overuse — change the peer context and S6D Social Overuse collapses.

9. **Accept that some anchors are decorative — and reframe the version-bump claim accordingly.** S1 Initial Encounter's novelty appraisal and S7C Ethical Integration's meaning-making are post-hoc. They describe the states correctly but don't predict anything the model doesn't already claim. This doesn't make V5 wrong, but it means the version-bump claim ("mechanism anchoring justifies V5") is overstated. In a V5 discussion or follow-up, reframe the achievement: "V5 adds mechanism anchoring to improve credibility and to ground future empirical work. Some anchors (S3B Bargaining, S7A Maturity) make strong falsifiable predictions. Others (S1 Initial Encounter, S7C Ethical Integration) are primarily descriptive. All of them provide handholds for the next version to test."
