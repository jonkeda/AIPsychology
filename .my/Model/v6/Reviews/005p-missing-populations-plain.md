This is a simpler rewrite of [005-missing-populations.md](005-missing-populations.md). Same findings, plain language. If you've read the original and it landed, skip this one.

# Missing Populations & Edge Cases — Plain Language

## TL;DR

- **Cognitive disabilities are completely absent.** For someone with ADHD or dyslexia, the line between "AI helps me do something I couldn't do alone" and "AI replaces a skill I built my identity around" is blurry. The model has no language for that.
- **The model assumes you are using AI, not having AI used on you.** Insurance claimants, students graded by AI, job candidates filtered by AI — none of them chose to interact with AI. The model's machinery doesn't apply to them.
- **PEN (Pre-emptive Non-Adoption — rejecting AI based on values before trying it) only covers Western secular ethics.** Religious or community-based rejection gets misclassified as fear-of-incompetence.
- **S3X (Structural Displacement — the state where viable AI-collaborative work no longer exists) was written for white-collar workers.** Care workers, drivers, and cashiers face total job elimination, with no "collaborate with AI instead" fallback. The model doesn't handle that path.
- **AI researchers and engineers are excluded from scope, but the reason isn't explained clearly.** For them, the threat runs backwards — AI failing is the problem, not AI succeeding.
- **Some people's livelihood depends on not adopting AI.** Teachers at AI-free schools, handmade artisans. This is different from fear, values, or displacement — it's economic pressure. The model has no frame for it.
- The model is written for Western English-speaking knowledge workers. Applied to non-Western populations, the concept of "professional identity threat" maps onto different social structures and will produce wrong answers.
- Eight populations are either missing or badly handled. Two need scope boundaries right now, before someone misapplies the model. The rest need honest gap-marking in populations.md.

## Findings

### 1. Cognitive disabilities and neurodivergence have no vocabulary in the model — not even as out-of-scope notes

The model assumes everyone has normal working memory, attention, and executive function. It doesn't say that, but every state description leans on it.

A dyslexic writer who uses AI for editing and transcription has two things happening at once. The AI is removing a barrier (assistive). It's also doing the thing their professional identity is built around (competitive). The model treats those as separate situations. For this person, they're the same act.

A person with ADHD who uses AI to hold context and generate options — AI doesn't just help them, it's what makes their work possible at all. If their role is later automated away, does S3X apply? The model says S3X applies when "viable AI-collaborative work no longer exists." But for this person, collaborative work was always the only kind that existed. The label inverts.

**Fix:** Add a "Cognitive Disabilities and Neurodivergence" section to `populations.md`. Cover three points: (1) the assistive-versus-competitive distinction breaks down for this group; (2) S3E identity threat (the fear that AI is replicating your skill) may not apply when the skill was never fully achievable without help; (3) the path into S3X may not go through a narrowing collaborative phase — it may just be sudden elimination. Mark this as a gap needing research. Do not try to extend the model here.

---

### 2. Involuntary AI exposure — having AI used on you, not using it yourself — is entirely absent from the model

The model assumes the person is someone who encounters AI and decides what to do with it. It has no vocabulary for a person who is the *subject* of AI — someone AI acts on without their choice.

Examples: An insurance company runs AI claims processing. The claimant didn't choose to use AI; it was used on them. A school grades essays with AI. The student didn't adopt anything — they were evaluated by a system they didn't consent to. An employer uses AI to screen job applications. The candidate was filtered before any human read their materials.

These people feel things: doubt that the process was fair, anxiety about being misclassified, anger at rules they can't see or appeal. But they don't have an S1 (Initial Encounter — the entry point where a person first meaningfully engages with AI as something to use). They never engaged. There is no delegation decision, no bargaining, no scope adjustment.

This is not a small edge case. AI is increasingly being deployed as decision infrastructure — AI acting on people rather than people using AI tools. Involuntary exposure is becoming the common situation for large populations.

**Fix:** Add an "Involuntary AI Exposure" section to `populations.md`. Say: (1) this model does not apply to people whose primary AI experience is being evaluated or managed by AI they didn't choose; (2) examples include insurance claimants, graded students, job candidates, and bank customers monitored for fraud; (3) they need a separate framework, not outlined here. This is a scope boundary to prevent misapplication, not a problem to solve.

---

### 3. **PEN** assumes Western secular ethics and will misclassify religious and cultural rejection

PEN (Pre-emptive Non-Adoption) is defined around prior ethical frameworks such as privacy advocacy, open-source ethics, and labour rights. Those are all modern Western secular ideas.

The model has no vocabulary for religious rejection (AI as against divine will, as soulless, as contrary to traditional vocational ethics), non-Western ethics (such as Ubuntu community-over-individual philosophy, Buddhist right livelihood, or Confucian relational duty), or community-embedded rejection (communities that watched technology destroy their industries and reject it based on shared memory, not individual ethical reasoning).

PEN's diagnostic signals assume: the person's values apply consistently across domains; their position shifts if you address their stated concern; their emotion looks like moral conviction, not fear. These signals fail for religious rejection (a person may reject AI at work but use AI-assisted prayer tools — that's not cross-domain consistency) and for community-embedded rejection (which won't shift based on technical evidence because it was never about technical details).

The practical problem: a practitioner sees a religiously-grounded non-adopter and classifies them as S2D (Defensive Resistance — the state where someone resists AI to protect their sense of competence). They apply the wrong toolkit — offering low-stakes trial use, providing identity reassurance — when the person's position won't shift regardless of what the AI can do.

**Fix:** Narrow PEN's definition in `states/PEN-pre-emptive-non-adoption.md`. Change "prior ethical frameworks applied to technology (privacy advocacy, open-source ethics, labour rights)" to "Western secular ethics frameworks focused on individual rights and labour economics." Add a "Religious and Cultural Non-Adoption" section to `populations.md`: (1) PEN covers Western secular rejection only; (2) religious rejection and community-embedded rejection are out of scope; (3) the diagnostic signals for separating PEN from S2D don't work for these groups.

---

### 4. **S3X** was written for white-collar knowledge workers and fails for care, service, and manual jobs

S3X (Structural Displacement) describes a narrowing. The translator becomes an AI-output editor. The paralegal becomes a legal strategy specialist. There is always something left to transition into.

That narrowing doesn't exist for care workers (home care, nursing aides, personal assistance — there is no "AI-collaborative care" role; you cannot manage an AI that holds someone's hand), drivers (delivery, taxi, bus — "human oversight of autonomous vehicles" is not a commercial role the economics support), retail and service workers (cashier, barista, receptionist — "manage the AI checkout system" is not a real job at the same wage level), or manual tradespeople (plumbers, electricians, construction workers — the work either requires human hands or it doesn't).

For these workers, S3X isn't reached through a pathway that narrows until nothing is left. It's reached through immediate total elimination. That distinction matters because the psychological path is different — not "my domain is shrinking," but "my job is just gone."

The model lists "adversarial advocacy" (regulation, labour protection, collective action) as one exit from S3X. For care and service workers, this is probably the main exit. The current description buries it.

**Fix:** Expand `states/S3X-structural-displacement.md` to distinguish two entry conditions: (1) white-collar displacement, where a collaborative pathway existed but became unviable; (2) service, care, and manual displacement, where there was never a collaborative pathway. In the transitions section, mark adversarial advocacy as the most probable exit for the second type, not an afterthought. Add a note in `populations.md`: care, service, and manual workers reach S3X through different entry conditions and face different exit options.

---

### 5. AI researchers and engineers are excluded from scope without explaining why that exclusion matters

The model says people whose professional identity is *about* AI — researchers, engineers, ML practitioners — are out of scope. That's a reasonable boundary. But the model doesn't explain the structural reason, which makes the exclusion look arbitrary.

The reason matters: the threat structure is inverted. The model's machinery says that when AI succeeds at your skill, you feel threatened (S3E identity threat). For an AI researcher, when AI succeeds, it's affirming — that's what they're trying to make happen. When AI fails, breaks unexpectedly, or hallucinates, that threatens them. Their identity says "I understand this system." The system behaving in ways they didn't predict undermines that.

There's a second dynamic: many AI practitioners feel anxiety not because AI threatens their job, but because they understand the system well enough to know where it fails. They see the overstated claims, the training-data gaps, the adversarial fragility. That's not S3E or S3B (Bargaining — drawing personal limits on AI use). It's something else entirely.

**Fix:** Expand the AI experts note in `populations.md` from one line to a short paragraph: (1) this population is excluded because the threat structure is inverted — AI failure is the threat, not success; (2) do not apply S2D or S3E to an AI researcher who seems anxious — they are probably working through capability transparency or deployment risk, not skill-replication fear; (3) a separate model for this population hasn't been built.

---

### 6. People whose livelihood depends on *not* adopting AI are invisible to the model

There is a real group whose economic position requires avoiding AI — not out of fear, not out of values, not because they've been displaced, but because their market or community demands it. Examples: teachers at schools where parents pay specifically for AI-free education, therapists at practices that market themselves as human-only care, regulatory specialists who exist because AI use is restricted, artisans in markets where "handmade, no AI" is the value proposition.

These people are not in S2D — they're not resisting out of fear. They're not in S3X — they haven't been displaced. They're not in PEN — their stance isn't values-based. If the market demand shifted tomorrow, many of them would use AI immediately.

A key problem: their stated position on AI may not reflect their actual opinion. A therapist might think AI-assisted therapy is fine, but cannot offer it without losing clients. A teacher might find AI genuinely useful, but cannot use it without losing their job. That makes observation-based classification unreliable for this group.

This is structurally similar to the economic access barrier already noted in populations.md (some people stay in S3B indefinitely because they can't afford access). The direction is reversed: economic pressure prevents adoption instead of enabling it.

**Fix:** Add an "Economic Incentive for Non-Adoption" section to `populations.md`: (1) some people face market or community conditions that make non-adoption economically rational; (2) this is distinct from S2D, S3X, and PEN; (3) their stated position may not reflect their actual opinion, making diagnosis unreliable; (4) interventions designed for identity protection — reassurance, low-stakes trial use — will not work here; the block is economic, not psychological.

---

### 7. AI-native users (children and teens) are described as a shortcut, not a population

The populations.md note on AI-native users says they "often bypass S1, S2D, and S3E" and follow the path S0 → S5 (direct integration) or S0 → S7I (Identity Expansion). Three things are missing.

**Developmental stage is not acknowledged.** A 14-year-old using AI throughout school has a forming identity. A 22-year-old entering the workforce as an AI-native has a stabilizing one. These are psychologically different situations. The model collapses both into "identity not yet formed, therefore no identity threat."

**The S0 → S5 path has no internal states.** S5 (Understanding — a stable, deliberate relationship with AI reached after testing it and forming a measured position) implies real work: trial, failure, adjustment, integration. How does a 16-year-old arrive there? The model says they skip S2D and S3E but doesn't say what they do instead. "Using AI as default without ever questioning it" is not S5 — S5 requires deliberate engagement. This might be a variant of S6 (Overuse) or a gap.

**School and workplace are conflated.** A 17-year-old in school has external permission structures around AI (the school allows or mandates it). A 22-year-old entering their first job arrives with economic stakes and colleagues who may resent their fluency. The psychological situation probably changes at that boundary. The model doesn't say.

**Fix:** Expand the AI-Native Users section in `populations.md`. Write one full paragraph per developmental stage: (1) school-age users before professional identity has formed — what is the arc? What triggers S6 Overuse risk if there is no S3E or S3B moderating use? (2) AI-native workforce entrants — does the arrival of economic stakes change the dynamics? Acknowledge the model doesn't yet have complete descriptions for either stage. Do not invent new states; mark the gaps.

---

### 8. The model is built for Western English-speaking knowledge workers and will misfire elsewhere

The model uses English, cites English-language psychology (Bandura, Lazarus, Festinger, Prochaska), and assumes Western professional identity — the idea that your sense of self is built around your individual skills and professional achievements.

That assumption doesn't hold everywhere. In many East Asian, African, and South American cultural contexts, identity is relational — built around family role, community standing, or position in a hierarchy, not personal skill. A person in that context whose skill is replicated by AI may not feel S3E (personal identity threat). They may feel family shame or loss of community standing. That is a different thing, with different causes and different responses.

The bargaining in S3B assumes individual scope-setting ("I will use AI for X but not Y"). In family-network or community-network economies, the scope-setting is social — "this family will not use AI for this work." That's a different mechanism.

What counts as a "domain" (the bounded skill set the model uses as its unit of analysis) is also culturally loaded. In contexts where work is embedded in social obligation or hierarchical relationships, "domain" may not be a meaningful unit at all.

**Fix:** Add a "Non-English and Non-Western Populations" section to `populations.md`: (1) this model is built on Western psychology and Western assumptions about individual professional identity; (2) identity threat, domain scoping, and resolutions such as S7M (Maturity) and S7I (Identity Expansion) operate differently in collectivist, relational, and hierarchical contexts; (3) applying this model to non-Western populations without cultural translation risks misclassification and wrong interventions; (4) that translation work has not been done. This is a critical scope boundary, not fine-print.

---

## Recommendations

**Priority 1 — add scope boundaries before anyone misapplies the model:**

1. Add **Involuntary AI Exposure** to `populations.md`. State clearly: this model does not apply to people who are evaluated or managed by AI they didn't choose. They need a separate framework.
2. Add **Non-English and Non-Western Populations** to `populations.md`. State that identity threat, domain scoping, and resolution states operate differently in collectivist and relational contexts. Translation work is needed.

**Priority 2 — narrow and clarify existing framings:**

3. Narrow **PEN** in `states/PEN-pre-emptive-non-adoption.md` to Western secular ethics. Add a **Religious and Cultural Non-Adoption** note to `populations.md` with diagnostic warnings about misclassification as S2D.
4. Expand **S3X** in `states/S3X-structural-displacement.md` to distinguish white-collar narrowing from service-work elimination. Add a note in `populations.md` that care, service, and manual workers face different entry conditions and different exit options, with adversarial advocacy as the most likely resolution.

**Priority 3 — extend existing sections with honest gap-marking:**

5. Expand the **AI Researchers and Practitioners** note in `populations.md` to state the inversion explicitly: they are threatened by AI failure, not success.
6. Add **Cognitive Disabilities and Neurodivergence** to `populations.md`. Mark as a gap requiring research.
7. Add **Economic Incentive for Non-Adoption** to `populations.md`. Distinguish from S2D, S3X, and PEN.
8. Expand **AI-Native Users** in `populations.md`. Separate school-age from workforce-entry. Mark both descriptions as incomplete.
