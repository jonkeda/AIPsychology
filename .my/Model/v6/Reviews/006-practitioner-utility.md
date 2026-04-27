# Practitioner Utility Review — Model V6

## TL;DR

- **Observable diagnostics are half-baked:** observation-guide helps with S2T/S2D and S3B/S7M (those work), but PEN/S2D split is theoretically clean and practically unreliable in a single conversation. You cannot diagnose states fast enough to use this in most real interventions.
- **Related literature is decorative:** knowing that S3E connects to self-efficacy collapse does not tell a manager what to do. It's vocabulary padding, not intervention guidance.
- **The dropout reversibility test is elegant but impractical:** requires resources most workplaces do not have — spare tools, testing time, permission to experiment.
- **S3X is correctly out of scope:** the model honestly says "this is no longer a psychology problem" — right. But practitioners are stuck with those people anyway and get no guidance.
- **Interventions are defined only negatively:** the model excels at telling you *what not to do* (the common mistakes table). It does not tell you *what to do instead*.
- **Multi-domain people are unhandled:** the model says people occupy states per-domain. When someone is S2D in writing but S5 in email on the same day, how do you actually manage that person? Unspecified.
- **Healthiness framing is reasonable but not grounded:** the claim that 6+ months in S3E Ego Shock is "clinical distress" is plausible but unvalidated. V6 should not claim a clinical boundary it has not tested.
- **V6 works as vocabulary, not as a tool:** if the goal is *shared language in a 1:1 conversation*, V6 delivers. If the goal is *diagnosis and intervention protocol*, V6 is incomplete.

---

## Findings

### 1. Observation-guide enables fast diagnosis for three state pairs; fails entirely for PEN vs S2D

The observation markers in `observation-guide.md` are genuinely useful for **S2T vs S2D** (ask whether they updated their view; S2T will have, S2D won't) and **S3B vs S7M** (ask which tasks they won't delegate; S3B will say identity-domain, S7M will say reliability). These signals work in a real conversation without extensive observation.

**For S6 states** (distinguishing S6E Enthusiastic Overuse, S6D Dependent Overuse, S6R Driven Overuse, S6S Social Overuse), the guide tells you to look at affect, drivers, and what would change behaviour. This is learnable and practitioners can probably identify the driver correctly 60–70% of the time after a few conversations.

**For PEN vs S2D**, the observation-guide explicitly states: "none reliable on a single observation." The three signals (cross-domain consistency, evidence response, emotional register) **require observation over time**. In practice, a manager in a one-off conversation with someone who says "I have values-based concerns about AI" cannot reliably separate:
- Someone who has genuinely evaluated AI against their values and decided no (PEN), from
- Someone who is defending their competence and using ethical language as a cover story (S2D Defensive Resistance plus rhetoric).

The guide says most real cases are mixed — true and important — but this means the diagnosis is actually: "this could be either, and here's how to find out over weeks." For practitioners who need to know today whether someone's objection is values-grounded (stable, respect it) or threat-driven (address the threat), the tool fails.

**Fix:** Reframe PEN diagnostics as longitudinal-only. Remove it from the single-conversation section of observation-guide. Add a separate section: "Signals that only emerge over weeks" with a clear timeline estimate (4–6 weeks of varied contexts). This is honest; the current framing suggests you can diagnose it in a conversation.

### 2. Related-literature lines are vocabulary-anchoring, not intervention-guidance — practitioners do not need to know about self-efficacy collapse to help someone

The model explicitly reframes related literature as "vocabulary, not mechanism." For S3E Ego Shock (self-efficacy collapse plus terror management), S6E Enthusiastic Overuse (variable reward structures), and S7M Maturity (metacognitive calibration), the academic anchors are:
- Correct as descriptive frames.
- Legible to readers with psychology training.
- Useless for a manager trying to figure out what to say or do in a 1:1.

A manager who learns that S3E involves self-efficacy collapse does not thereby know: should I reassure this person? Should I push them to try again? Should I give them a smaller task? Should I leave them alone? The related-literature anchor points at what kind of phenomenon S3E *is*, not how to respond to it.

The `observation-guide.md` table "Common manager mistakes by state" is more useful than all the related literature combined — it tells you what *not* to do. But the model has no analogous "what to do" table, because it is descriptive, not prescriptive.

**Fix:** Acknowledge in `Model6.md` that related-literature vocabulary is useful primarily for cross-disciplinary communication and for future empirical grounding, not for practitioners. Add a note: "For intervention-focused practitioners, see the manager-mistakes table in observation-guide.md for guidance on what not to do. V6 does not yet provide prescriptive intervention protocols." This prevents practitioners from reading related literature and expecting it to guide their actions.

### 3. The dropout reversibility test is operationally elegant but practically out of reach for most workplaces — requires spare tools, testing permission, and time

The reversibility test is conceptually clean: provide a tool that demonstrably solves the person's stated problem. If they restart using AI, practical severity was high. If they don't, emotional severity was driving the exit.

**In practice, this requires:**
- Having a tool that solves the exact problem the person cited (not always available).
- Permission from leadership to test it with one person, one conversation, tracking the outcome (rare in most orgs).
- Time to run the test and observe the result (days to weeks).
- A person who is willing to re-engage after they have already dropped out (high friction).

**Worse:** The model admits inter-rater reliability on the 0–10 severity axes has not been established. So even if you run a reversibility test and see whether they restart, you cannot score the axes with confidence. The test is testable in principle (marked **Testable** in the model), but inter-rater reliability must be established first. Without it, two practitioners scoring the same dropout case could land on opposite ends of the plane (high practical / low emotional vs. low practical / high emotional), and both claim the model supports their view.

**Fix:** Add a section to `dropout.md`: "Operational constraints on the reversibility test" that lists the resources required, the time horizon, and the prerequisite of scoring calibration. Mark the 0–10 axes explicitly as **Conjecture — scoring reliability not established**. This prevents practitioners from running a test that looks like an operationalisation but actually relies on unvalidated scoring.

### 4. S3X Structural Displacement is correctly out of scope; the result is that practitioners have no handle on a real population

The model correctly identifies S3X Structural Displacement (a translator's market collapses because AI now does translation; a paralegal's document-review role is eliminated) as **structural, not psychological**. The identity crisis is real but the root problem is economic: there is no viable adaptation within the domain because no viable role remains.

The observation markers — person describes the problem in economic terms, failed bargaining narrowings, question shifted from "how do I adapt?" to "what work is left?" — are accurate and usable.

**But then the model steps back.** It correctly says: "this is no longer a psychology problem." The three transitions (occupational transition to a new domain, principled exit, adversarial advocacy) are named but not developed. For a manager with an S3X person on their team, V6 offers:
- Clear diagnosis: yes, the role is structurally gone.
- No guidance: what do I actually do with this person?

The model defers to "labour protection, economic redistribution, or regulation" but does not address the person in front of you: Do they need career-transition support? Retraining? Economic bridge? Psychological support during transition? Are they eligible for any of these? The answer, from V6, is: not my domain.

**This is honest.** The model should not prescribe economic interventions it is not equipped to handle. **But it is incomplete.** A working tool for practitioners would either:
1. Extend S3X to include guidance on transition support and resource matching, or
2. Describe in `populations.md` or a separate guide what practitioners should do when they identify S3X (refer to career services, help with retraining budget, etc.).

**Fix:** Add a section to `usage.md`: "When you identify S3X Structural Displacement" with concrete referral pathways: career services, retraining programs, severance-negotiation support, economic-transition counseling. This does not make V6 prescriptive; it makes it complete by pointing practitioners to the right domain experts. Without this, the model correctly diagnoses a problem and then leaves the practitioner helpless.

### 5. The distinction between PEN Pre-emptive Non-Adoption and S2D Defensive Resistance collapses in real conversations — the model's own signals require weeks to distinguish

PEN Pre-emptive Non-Adoption (states/PEN-pre-emptive-non-adoption.md) is defined as **values-grounded refusal before testing**. S2D Defensive Resistance is **identity-protection through dismissal of evidence**.

The model lists three distinguishing signals:
1. **Cross-domain consistency:** Does the objection apply across domains, even where identity is not at stake?
2. **Evidence response:** Does the position hold when the stated concern is demonstrably addressed?
3. **Emotional register:** Anxiety suggests S2D; moral conviction suggests PEN.

The model admits these are **"none reliable on a single observation."** All three require **behavioural observation over multiple weeks and contexts.**

**In practice:** A person who says "I think AI training data practices are exploitative and I won't use it" could be:
- **Genuine PEN:** has a values-based stance grounded in ethical conviction, and that stance is stable across domains.
- **S2D with ethical language:** is protecting competence (fear of replacement) and has learned to frame it in ethical terms because that sounds better than "I'm afraid I'll look stupid."

The observation-guide signals tell you: wait 4–6 weeks, see if the person applies the objection to low-stakes domains where identity is not at risk (e.g., using AI for travel planning). If they refuse there too, it's probably PEN. If they use AI happily in low-stakes domains but wall it off from their core work, it's probably S2D.

**For a manager or coach in a first conversation, this is not actionable.** You have to guess, and the cost of guessing wrong is high:
- Misidentify as PEN and respect the boundary → you miss an identity threat that needs support.
- Misidentify as S2D and push back on the "ethics" → you dismiss a genuine values stance and damage trust.

**Fix:** Reframe the PEN vs S2D section of observation-guide as explicitly longitudinal. Add: "First conversation diagnosis is unreliable. If the person expresses ethical objections, note them and observe the next four weeks. See whether the objection generalizes to low-identity-stakes domains. Do not try to resolve this in the first conversation." This prevents premature closure on diagnosis and acknowledges the model's limitation.

### 6. The observation-guide tells practitioners what *not* to do by state, but does not tell them what *to* do — model is half of an intervention framework

The `observation-guide.md` table "Common manager mistakes by state" is the most practically useful piece of V6:
- Don't skip S1 Initial Encounter with a mandate.
- Don't argue with S2D Defensive Resistance's evidence; it hardens the position.
- Don't reassure someone in S3E Ego Shock; it feels dismissive.
- Don't reward output volume in S6E Enthusiastic Overuse.
- Don't make AI use publicly visible if you have S6S Social Overuse.

These are **negations: what to stop doing.** They work because they prevent the common harm. But the model does not provide: what *to do instead*.

For S3E Ego Shock, the guide says "don't bring data, don't reassure, don't rush." What should you do? The model is silent. Presumably: sit with the person, acknowledge the threat, go slow, work on identity recovery. But V6 does not say this, so practitioners infer it or make it up.

For S6D Dependent Overuse, the guide says "don't praise AI-augmented output without acknowledging the person's contribution." What should you do? Presumably: rebuild independent confidence, give them tasks where they have to rely on their own judgment, celebrate their solo work. Again, inference required.

**This is a significant gap.** A working intervention framework needs both the negative (what not to do) and the positive (what to do). V6 provides the negative. Building the positive requires empirical testing or practitioner input that the model does not yet have.

**Fix:** In `usage.md`, add a section: "What V6 does not provide — the next layer." State explicitly: "V6 identifies states and tells practitioners what responses will worsen the situation. It does not yet provide prescriptive intervention protocols for what to do in each state. Developing these requires empirical testing or practitioner input. See recommendations below." Then list what a V7 intervention layer should address. This is honest about the limitation and sets up future development.

### 7. The model handles multi-domain people as a conceptual matter but provides no guidance for managing them in practice

V6 explicitly says: "States are per-domain. The same person can be S2D Defensive Resistance in writing, S5 Understanding in email, and S7M Maturity in travel planning — all on the same day."

**This is true and important.** It correctly rejects the idea that a person has a single state.

**In practice, this creates a coordination problem the model does not address.** A manager has an employee who is:
- S2D Defensive Resistance about AI in their core domain (writes case law for clients).
- S5 Understanding about AI for research and document retrieval.
- S6E Enthusiastic Overuse of AI for routine coding tasks.

What does the manager do? The model says the three states are independent and have independent modulation axes. So the manager should:
- Apply S2D interventions (don't argue) to the writing domain.
- Let them run at S5 for research (stable and healthy).
- Watch for burnout in the S6E coding domain.

**But:** These domains are not independent. If the employee builds confidence in S6E coding and gets a win, does that carry over and push S2D writing toward S2T Trust Evaluation? If S2D writing fails and they feel like a failure, does that poison their confidence in S5 and S6E? If the manager applies different intervention strategies in different domains, does that feel incoherent or manipulative to the employee?

The model has no answer to these questions. It correctly identifies that people are multi-domain. It does not address the **cross-domain interference and transfer** that happens in real people with real psychologies.

**Fix:** Add a section to `social-context.md` or `usage.md`: "Multi-domain coordination and cross-domain transfer" with the following structures:
- Cross-domain wins: A confidence win in one domain can reduce identity stakes in another. Do not assume state transitions are independent.
- Cross-domain setbacks: Identity threats in one domain (S3E) can amplify defensiveness in other domains (push S2T toward S2D).
- Intervention consistency: When managing someone across multiple domains, is it better to apply the same communication strategy across domains (even if it is suboptimal for one) for coherence, or to tailor to each domain? Unclear, but the question should be named.

This does not solve the problem but it prevents practitioners from assuming state transitions are independent when they are managing people.

### 8. Healthiness framing is reasonable but the clinical boundary (6+ months in S3E = clinical distress) is asserted without evidence

The `healthiness.md` file maps states to a sustainability frame:
- **Sustainable:** S7M Maturity, S5 Understanding, S3B Bargaining.
- **Sustainable with cost:** S6E Enthusiastic, S6R Driven, S6S Social.
- **Transitional only:** S3E Ego Shock, S2T Trust Evaluation, S2D Defensive Resistance, S1 Initial Encounter.
- **Recovery:** S7B Burnout.
- **Corrosive:** S6D Dependent, sustained S2D.
- **Legitimate, not pathological:** S3X.

**This is sensible.** It avoids pathologizing normal variation and correctly identifies that S3B and S7M are stable, not end states to rush toward.

**But:** The model states: "Sustained S3E (six-plus months unresolved) is within the range of clinical distress." This is plausible. Six months of identity threat with no progress is painful and can load clinical symptoms. **But the model has not validated this boundary.** V6 is descriptive-first and admits it is untested. Claiming a clinical threshold without testing it is a step toward pathologization that V6 should not take.

Similar claims: "S6R and S6S are sustainable only as long as external pressure does not exceed personal capacity." True, but where is the breaking point? At what workload does S6R flip to unsustainable? The model does not say.

**Fix:** Rewrite the clinical statement in `healthiness.md` as: **Conjecture —** sustained S3E beyond six months is plausibly within a range that matches clinical distress presentations, but this boundary has not been validated. Change the framing from "is within the range" (a claim) to "is plausibly within the range" (a hypothesis). Do the same for any healthiness claim that specifies a threshold. This preserves the interpretive value without overclaiming.

### 9. V6 works as a vocabulary framework, not as an operationalised diagnostic tool — the cost of moving from "shared language" to "usable protocol" is higher than the model acknowledges

The model's own `usage.md` file makes an important distinction:
- **What V6 can be used for:** Recognition, vocabulary, intervention mapping, dropout triage, regression anticipation, org-design conversations.
- **What V6 cannot be used for:** Diagnosis (no validated test), prediction (no transition probabilities), quantitative measurement (inter-rater reliability not established), universal claims (untested), clinical therapy, performance management.

**The gap between these two lists is the gap between a shared vocabulary and a working tool.**

If the goal is "my team and I use the same language for states" — V6 delivers. A manager can read it in one day, start using the terms in 1:1s, and have clearer conversations. This is real value.

**If the goal is "I can diagnose where someone is in under one conversation and plan an evidence-based intervention" — V6 does not deliver.** The observation-guide helps but does not eliminate uncertainty. The dropout axes are helpful but not scored reliably. The intervention negations (what not to do) are useful but incomplete (no prescriptions). The multi-domain reality is acknowledged but not navigated. PEN vs S2D requires weeks to diagnose.

The model acknowledges all of this — it is honest about its epistemic status. **But this honesty should lead practitioners to a clear conclusion: V6 is a map, not a protocol.** Maps are useful. They orient you. They prevent catastrophic errors. They are not enough to navigate alone.

**Fix:** Reframe the header of `usage.md` to reflect this: "What V6 is: A shared vocabulary and conceptual map." Then in the main text: "V6 is designed to help practitioners recognise patterns and avoid harm. It is not yet designed to support diagnosis or empirical intervention protocols. Until V6 has been tested and scored-for-reliability, treat it as a conversation tool and orientation guide, not as a diagnostic instrument."

---

## Recommendations

Listed in priority order for addressing practitioner utility:

1. **Reframe the observation-guide's PEN diagnostics as longitudinal-only (Finding 5).** The current framing suggests single-conversation diagnosis is possible; it is not. Adding a clear 4–6 week observation timeline prevents misdiagnosis and high-stakes guess-making.

2. **Add a "What V6 does not provide" section to usage.md (Finding 6).** Explicitly state that the model provides negations (what not to do) but not prescriptions (what to do). Set expectations for practitioners. This prevents the frustration of reading the model and finding no intervention protocols.

3. **Add multi-domain coordination guidance to social-context.md (Finding 7).** Acknowledge cross-domain transfer and interference. Raise the question of intervention consistency across domains. This prevents practitioners from treating state transitions as independent when they are managing real people.

4. **Revise related-literature framing in Model6.md to clarify that it is not intervention guidance (Finding 2).** Add: "For practitioners seeking intervention guidance, see the manager-mistakes table in observation-guide.md. Related literature is useful for cross-disciplinary communication and future empirical grounding, not for action in the moment."

5. **Revise clinical boundary in healthiness.md from claim to conjecture (Finding 8).** Change "sustained S3E is within the range of clinical distress" to "sustained S3E is plausibly within the range of clinical distress — this boundary is untested." Do this for all healthiness claims that assert thresholds.

6. **Add operational constraints to dropout.md on the reversibility test (Finding 3).** List resources required, time horizon, prerequisite scoring calibration. Mark 0–10 scoring as **Conjecture** with reliability not established. This prevents running a test that appears operational but relies on unvalidated scoring.

7. **Add referral pathways to S3X guidance (Finding 4).** In `usage.md`, create a section "When you identify S3X Structural Displacement" with concrete next steps: career services, retraining budgets, economic-transition counseling. This makes the model complete without overreach.

8. **Clarify in Model6.md that V6 is a map, not a protocol (Finding 9).** In the "What kind of model this is" section, add: "This is a conceptual map and shared vocabulary. Until it is tested and scored for reliability, it is not a diagnostic instrument or treatment protocol. Use it to recognise patterns and avoid harm. Use it for conversation. Do not use it alone to diagnose or plan interventions."