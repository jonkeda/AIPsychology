# Review E — Missing Populations & Edge Cases

## TL;DR

- **Cognitive disabilities and neurodivergence completely absent** from scope, populations.md, and state descriptions. A person with ADHD or processing disorder may experience AI threat differently (reduced cognitive load vs skill replication) and may not traverse the model's identity-protection arc at all.
- **Involuntary AI exposure** (being evaluated or replaced *by* AI, not using it) is structurally absent. Insurance adjuster, hiring manager, student-being-graded are subjects, not users. They need their own population section or explicit scope boundary.
- **PEN (Pre-emptive Non-Adoption) covers only Western secular ethics.** Religious rejection of AI (divine will, soul-based objections, traditional labour ethics) does not fit the stated entry conditions or the distinction from S2D. Narrowing is needed, or framework expansion.
- **S3X (Structural Displacement) models only white-collar loss.** Care work, manual trades, and service roles face full role elimination but don't have a "collaborative work" pathway to S3X entry. The state applies to them only partially.
- **AI researchers and practitioners explicitly excluded but not explored.** Their professional identity *is* AI. This creates inversion: they experience S3E-like identity threat when AI *fails*, not when it succeeds. Frame is backwards for this population.
- **Economic dependence on non-adoption is invisible.** Teachers in private schools, workers in communities hostile to AI, regulatory specialists — their livelihood requires resisting adoption. This is distinct from S2D (competence protection) and S3X (displacement). Needs its own frame or scope limit.

## Findings

### 1. Cognitive disabilities and neurodivergence have no vocabulary in the model — not even as out-of-scope notes

The model assumes standard executive function, working memory, and attention capacity. A person with ADHD, dyslexia, processing disorder, or traumatic brain injury experiences AI's cognitive impact differently.

For example: A dyslexic writer uses AI for transcription/editing support. The model frames this as assistive tech (which it partially is) but the writer's professional identity *is* built on writing. When AI does the writing, it is simultaneously: (a) removing the assistive load, and (b) replicating a skill they built their identity around. The model has no way to describe this person being in two states at once in the same domain.

Another example: A person with working-memory limitations relies on AI to hold context and generate options, allowing them to do work they could not otherwise do. This is assistive, but it also means their capability is genuinely newly-enabled (not replicated). If they later face role displacement, is S3X the right frame? The model says S3X applies when "viable AI-collaborative work no longer exists." But for this person, collaborative work is the only work that was ever viable. The language inverts.

**Plain gloss:** Assistive technology (where AI provides access) and skill replication (where AI competes with existing skill) are not binary. Cognitive disabilities blur the boundary.

**Fix:** Add a section to `populations.md` titled "Cognitive Disabilities and Neurodivergence." Three sentences at minimum: (1) the assistive-vs-competitive distinction breaks down; (2) S3E identity threat may not apply when the skill being "replicated" was never fully achievable by the person; (3) S3X Structural Displacement may be reached without a collaborative-work pathway, because collaborative work is the baseline, not a negotiated position. Do not attempt to extend the model here; explicitly mark this as a gap requiring research.

---

### 2. Involuntary AI exposure — being subject to AI rather than using it — is entirely absent from the model's vocabulary

The model frames the user as an agent who encounters AI and decides whether to adopt it. It does not frame the person as a *subject* being evaluated, replaced, or managed *by* AI.

Example cases: An insurance company implements AI claims adjudication. The claimant never chooses to use AI; it is used *on* them. A school implements AI grading. The student is not an AI user; the student is being evaluated by AI. An employer implements AI for hiring decisions. The candidate is being filtered by AI they did not consent to. A bank implements AI for fraud detection that flags transactions. The account holder is being monitored by AI.

These people experience psychological impact: doubt about fairness, loss of human discretion, anxiety about being misclassified, anger at rules they don't understand. But they do not fit the model's machinery. They have no S1 (Initial Encounter), no delegation-level choice, no bargaining-scope negotiation. They are passively exposed.

This is not a minor edge case. As AI deployment moves from productivity tools to decision-infrastructure, involuntary exposure is becoming the dominant mode for large populations.

The model's scope statement says it applies to "the person's first substantive exposure to AI." For involuntary subjects, that exposure is never to a tool they control. Do they not have a first encounter? Or is S1 fundamentally different for subjects?

**Plain gloss:** Using AI (user perspective) and having AI used on you (subject perspective) are not just different degrees of the same thing — they are structurally different. The model's state graph assumes user agency at every step.

**Fix:** Add a section to `populations.md` titled "Involuntary AI Exposure" or "People as Subjects Rather than Users." State clearly: (1) this model does not apply to people whose primary AI exposure is as a subject of AI decision-making, not as a user of AI tools; (2) these populations include claimants, students being graded, job candidates, account holders monitored by AI; (3) they require a separate descriptive framework (not outlined here). Mark this as out-of-scope to prevent misapplication, not as a limitation to overcome.

---

### 3. PEN (Pre-emptive Non-Adoption) assumes a narrow Western secular-ethics frame and will misclassify religious and cultural rejections

PEN is defined as "values-grounded ethical appraisal" based on "prior ethical frameworks applied to technology (privacy advocacy, open-source ethics, labour rights)."

These are all modern Western secular frameworks. The model provides no vocabulary for:
- Religious rejection (AI as against divine will, as soulless, as contrary to traditional vocational ethics).
- Non-Western ethical frameworks (Ubuntu ethics, Buddhist concepts of right livelihood, Confucian relational duty).
- Cultural rejection rooted in community identity rather than individual values (communities that have witnessed technology destroy their industries and reject it wholesale, not through reasoned ethical appraisal).
- Intergenerational trauma around tool displacement (Appalachian communities, Indigenous communities) where the objection is embedded in family and community memory, not formulated as a modern ethical argument.

The PEN diagnostic signals assume: (1) cross-domain consistency (the person's values apply consistently), (2) evidence response (the person's position shifts if the concern is addressed), and (3) emotional register of moral conviction, not fear. These signals will fail for religious rejection (which may not be cross-domain consistent — a person may reject AI in work but use it for prayer/meditation support) and for community-embedded rejection (which cannot be addressed by technical evidence because it is not primarily about technical details).

A practitioner will easily misclassify a religiously-grounded non-adopter as S2D (Defensive Resistance — competence-protection cognition) and apply the wrong toolkit (offering low-stakes entry, identity-reassurance) when the person's actual stance is values-based and will not shift regardless of AI capability.

**Plain gloss:** PEN's definition of "values" is culturally narrow. Religious, cultural, and trauma-embedded objections get classified as S2D fear-of-incompetence instead of being recognized as legitimate non-adoption positions.

**Fix:** Narrow PEN's definition in `states/PEN-pre-emptive-non-adoption.md`. Change "prior ethical frameworks applied to technology (privacy advocacy, open-source ethics, labour rights)" to "secular ethical frameworks emphasising individual rights and labour economics." Then add a section to `populations.md` titled "Religious and Cultural Non-Adoption." State: (1) PEN describes Western secular values-based rejection only; (2) religious rejection (against divine will, traditional ethics) and community-embedded rejection (family/cultural memory of displacement) are out-of-scope; (3) these populations are real, their non-adoption is legitimate, and the model's diagnostic signals for separating values-based from defensive rejection do not apply to them. This is a scope limit, not a flaw — but it must be stated clearly.

---

### 4. S3X (Structural Displacement) applies only to knowledge-work roles with a clear "collaborative" pathway; it fails for manual, care, and service work where displacement is total

S3X is defined as "viable AI-collaborative work no longer exists in their domain." The state is reached when "role is being eliminated" or when "the person's remaining domain is too small to constitute a viable livelihood."

These descriptions work for translators (becomes AI output editor), paralegals (becomes legal strategy specialist), and writers (becomes AI prompt engineer). They work for white-collar roles where there is a scalable collaborative option.

They do not work for:
- **Care workers** (home care, nursing, personal assistance). Collaborative care does not exist. AI might support scheduling, health monitoring, or record-keeping, but it does not collaborate in the work of physical care or human attention. A person dependent on personal-care income cannot pivot to "managing AI care systems."
- **Drivers** (delivery, taxi, bus). Collaborative driving does not exist as a commercial role. The person cannot transition to "managing autonomous vehicles"; the economics do not support that role.
- **Retail and service work** (cashier, barista, receptionist). Collaborative service is economically unviable. A cashier cannot transition to "managing the AI checkout system."
- **Manual trades** (plumbing, electrical, construction). There is no intermediate "human oversight of AI" tier; either the work requires human hands or it does not.

For these workers, S3X is reached through full economic elimination, not through narrowing of a remaining collaborative domain. The state description assumes a residual domain to protect or transition into. These workers have no such residuum.

The model's current language ("occupational identity disruption in the job-displacement literature") is right, but S3X's transitions assume white-collar pathways. The "adversarial advocacy" exit (regulation, labour protection, activist resistance) is the most realistic resolution for care and service workers. But the state description leaves this underexplored.

**Plain gloss:** S3X says "there is no collaborative work left." For care and service work, there was never any collaborative work to begin with. The psychological path to S3X is different (not a narrowing that fails, but a realization that the job is not automatable in a hybrid way). The transition options are different too.

**Fix:** Expand `states/S3X-structural-displacement.md` to add an "Entry condition variants" subsection. Distinguish: (1) white-collar displacement where a collaborative pathway existed but was rendered unviable, and (2) service/care/manual displacement where collaborative work never existed as a commercial option. Then expand the transitions section: for service-work displacement, mark "adversarial advocacy" (regulation, labour protection, collective action) as the most probable exit, not an afterthought. Finally, add a note to `populations.md` under the non-knowledge-work section: "Workers in care, service, and manual trades face full role displacement, not narrowing of a collaborative domain. S3X applies to them, but with different entry conditions and different transition options."

---

### 5. AI researchers and practitioners are excluded from scope without acknowledgement of the inversion this creates

The model states: "Users who are already AI experts (AI researchers, engineers, ML practitioners whose professional identity is *about* AI) are out of scope."

This is reasonable as a scope boundary, but it hides a structural inversion. For these users, S3E-like identity threat happens when **AI fails**, not when AI succeeds. Their professional identity is "person who builds and understands AI." When AI breaks, misses edge cases, hallucinates, or behaves unexpectedly, it threatens their core identity ("I understand this system"). When AI succeeds, it is identity-affirming.

This is the opposite of the model's machinery, where success in a domain (AI replicating the skill) triggers S3E threat. For AI researchers, success is the affirmation; failure is the threat.

There is also a secondary dynamic: many AI practitioners experience anxiety about AI deployment *because they understand it too well* — they know the gaps, the training data issues, the adversarial-example fragility, the way the field is overstating current capabilities. This is not identity-threat (S3E) or bargaining-scope (S3B); it is informed pessimism about a product they are supposed to champion.

**Plain gloss:** AI researchers and AI practitioners have inverted incentives. They are not covered by the model, but the inversion should be stated explicitly, not just implied by exclusion.

**Fix:** Add a subsection to `populations.md` under "Users who are already AI experts." Expand to one paragraph: (1) the model is out-of-scope for people whose professional identity is *about* AI because the threat structure is inverted (they are threatened by AI failure, not success), (2) this inversion is important and should not be misapplied (do not assume an AI researcher in S2D or S3E is working through skill-replication threat — they are probably working through capability transparency or deployment-risk fear), (3) a separate model for this population is not sketched here. One sentence is not enough to make this inversion clear.

---

### 6. Economic dependence on non-adoption — people whose livelihood requires *resisting* AI adoption — is not covered and cannot be accurately framed as S2D or any other state

There exists a population whose economic position depends on *not* adopting AI. Examples:

- **Teachers at private schools** where parents explicitly pay for "AI-free education."
- **Therapists and counsellors** in communities or practice styles that market human-only care.
- **Regulatory specialists** who help firms navigate restrictions on AI (job exists because AI is restricted).
- **Workers in communities explicitly hostile to AI** (Luddite-sympathetic communities, off-grid communities, conservative labour strongholds).
- **Artisans in "handmade" and "human-made" markets** where the economic value proposition is explicitly non-AI.

These people are not in S2D (Defensive Resistance), which is identity-protection cognition triggered by threat. They are not in S3X, which assumes displacement. They are not in PEN, which is values-based non-adoption. Their non-adoption is *economically enforced*. If the market demand or community expectation shifted, their rational choice would flip immediately.

This is structurally similar to economic access barriers (mentioned in populations.md: "A person in S3B may remain indefinitely because they cannot afford access"). But the direction is reversed. Economic barriers prevent access; economic incentives prevent adoption.

The person's stance toward AI might be neutral or positive, but their economic position requires visibly rejecting it. A therapist might think AI-assisted therapy is fine, but cannot market it because the business model depends on clients who reject AI. A teacher might find AI genuinely useful, but cannot use it because the school's positioning depends on non-adoption.

**Plain gloss:** A person whose paycheck depends on *not* adopting AI is in a different structural position from someone protecting identity or resisting based on values. The model has no frame for economically-enforced non-adoption.

**Fix:** Add a section to `populations.md` titled "Economic Incentive for Non-Adoption." State: (1) some people face market or community pressure that makes non-adoption economically rational; (2) these are not S2D (fear-driven) or S3X (displaced) or PEN (values-driven) — they are structurally distinct; (3) their stance on AI might not reflect their true belief, making observational diagnosis difficult; (4) interventions that work for identity-protection (reassurance, low-stakes entry) will not work for economic incentive structures (requires market or community shift). Two or three sentences at minimum; this is not a trivial edge case.

---

### 7. AI-native users (children/teens) are described as a pathway, not as a population, and the pathway description is incomplete

The populations.md section on "AI-Native Users" says they "often bypass S1, S2D, and S3E" and follow: S0 → S5 (direct integration) or S0 → S7I (identity expansion).

This is a sketch, not a model. Three problems:

**First, developmental stage is not acknowledged.** A 14-year-old using AI throughout school has a very different psychological profile from a 22-year-old entering the workforce as an AI-native. Adolescents are still forming identity; post-adolescents have identity stability and are integrating AI into it. The model collapses both into "identity not yet formed, so no identity threat."

**Second, the "direct S0 → S5" pathway has no internal states.** S5 Understanding is defined as the person having engaged, tested, integrated, and formed a measured stance. How does a 16-year-old arrive at Understanding? What is the step-by-step journey? The model says they skip S2D/S3E but gives no alternative machinery. Is there an S-state that describes "using AI as a default without having tested alternatives"? That's not S5 (which involves deliberate integration); it might be a fifth variant of S6 Overuse, or it might be a distinct state.

**Third, schooling and workplace entry are conflated.** An AI-native in school has external permission structures (school allows or mandates AI). An AI-native entering the workplace enters a domain with economic stakes and potentially defensive colleagues. Does the psychological state change at that boundary? Probably yes, but the model does not say.

**Plain gloss:** "AI-native users bypass the threat states" is true but useless. There needs to be a step-by-step description of what they experience instead, and it needs to separate childhood/adolescent use (before identity is formed) from post-adolescent AI-native entry (identity stabilizing as AI enters the domain).

**Fix:** Expand the AI-Native Users section in `populations.md` from three sentences to one full paragraph per developmental stage: (1) for school-aged users who grew up with AI (prior to professional identity formation), what is the learning arc? Do they skip to S5, or is there an intermediate state? What triggers S6 Overuse risk in this population if there is no S3E or S3B to moderate? (2) For AI-native workforce entrants (22–25, entering first job where AI is standard), does the dynamics change again when economic stakes arrive? Acknowledge that the model does not yet have a complete description of either pathway. Do not invent states; mark the gap.

---

### 8. Non-English and non-Western populations are not explicitly addressed, even though the model's vocabulary and related-literature connections are culturally embedded

The model uses English, cites English-language psychology (Bandura, Lazarus, Festinger, Prochaska), and assumes Western professional norms (the concept of "craft," "expertise," "professional identity" as Western constructs).

**First, identity threat operates differently across cultures.** In individualist Western contexts, identity is built around personal skill and professional achievement. In collectivist and relational contexts (East Asian, African, South American models), identity is relational — embedded in family role, community standing, or hierarchical position. A person in a collectivist culture whose professional skill is replicated by AI may not experience S3E (personal identity threat) but may experience family or community shame. The threat structure is different.

**Second, the bargaining in S3B works differently if the economy is not individual-skill-based.** S3B works by narrowing personal scope ("I will use AI for X but not Y"). In economies where work is distributed through family or community networks, the scope-narrowing is social, not personal. "I will not let this family member use AI for X" is not the same as "I will not use AI for X."

**Third, non-Western professional norms don't map to the model's assumptions.** The model assumes a domain is a bounded skill set. In contexts where work is embedded in social networks or hierarchical obligation, what counts as a "domain" is ambiguous.

**Plain gloss:** The model is written in and for a Western English-speaking knowledge-worker context. Applied to non-Western populations, the state machinery will misfire on what counts as identity, what counts as a domain, and what constitutes a resolution like S7M Maturity or S7I Identity Expansion.

**Fix:** Add a note to `populations.md` titled "Non-English and Non-Western Populations." State clearly: (1) this model is built on Western English-language psychology and Western concepts of individual professional identity; (2) identity threat, domain scoping, and status resolutions operate differently in collectivist, relational, and hierarchical contexts; (3) applying this model to non-Western populations without cultural-linguistic translation risks misclassification and inappropriate interventions; (4) translation and adaptation work is needed and is not sketched here. This is not optional fine-print. It is a critical scope boundary.

---

## Recommendations

**Priority 1 (add to scope boundaries before anyone misapplies the model):**
- Add **Involuntary AI Exposure** section to `populations.md`. Make clear: this model does not apply to people being evaluated/managed *by* AI. They need a separate framework.
- Add **Non-English and Non-Western Populations** section to `populations.md`. State that identity threat, domains, and resolutions map differently in collectivist and relational contexts. Translation work is needed.

**Priority 2 (narrow and clarify existing framings):**
- Narrow **PEN definition** in `states/PEN-pre-emptive-non-adoption.md` to "Western secular ethics." Add **Religious and Cultural Non-Adoption** to `populations.md`. Mark as out-of-scope with diagnostic warnings.
- Narrow **S3X** language in `states/S3X-structural-displacement.md` to acknowledge white-collar displacement as the primary case. Add note to `populations.md` on service/care/manual displacement: different entry conditions, different likely exits.

**Priority 3 (extend existing sections with honest gap-marking):**
- Expand **AI-Native Users** section in `populations.md`: separate school-age (pre-identity) from workforce-entry (post-identity-formation). Mark as incomplete.
- Add **Cognitive Disabilities and Neurodivergence** section to `populations.md`. Mark as a gap requiring research; do not attempt model extension.
- Expand **AI Experts (Researchers/Practitioners)** note in `populations.md`. State the inversion explicitly: threat from failure, not success.
- Add **Economic Incentive for Non-Adoption** section to `populations.md`. Distinguish from S2D, S3X, and PEN.

Do not attempt to extend the model to cover these populations. Mark gaps clearly. The model's value is in describing knowledge-work identity threat. Extending it to involuntary exposure, religious rejection, care-work displacement, and collectivist contexts requires separate work, not model patches.