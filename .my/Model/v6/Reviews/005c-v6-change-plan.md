# 005c — V6 Change Plan (from 005p)

Implementation plan derived from [005p-missing-populations-plain.md](005p-missing-populations-plain.md) and modeller decisions. Each item maps to a specific file and specific change. Findings are accepted, modified, or rejected by letter, matching the modeller's annotations on 005p.

---

## Accepted findings and changes

### P1 — Add Cognitive Disabilities and Neurodivergence section to `populations.md`

**Finding:** 005p § 1. Accepted in full.

**File:** `populations.md`

**Change:** Add a new section "Cognitive Disabilities and Neurodivergence" after the existing "AI as Assistive Technology" section:

> **Cognitive Disabilities and Neurodivergence**
>
> This model assumes the user's baseline capability exists independently of AI. For users with conditions affecting working memory, attention, or executive function (for example, dyslexia, ADHD, or acquired cognitive disability), that assumption does not hold cleanly.
>
> Two distinctions from the main model:
>
> - The **assistive versus competitive** line breaks down. A dyslexic writer who uses AI for editing may experience it simultaneously as an access tool (assistive) and as a tool replicating their professional skill (competitive). The model has no vocabulary for that dual role.
> - **S3E Ego Shock** may not apply where the skill was never fully achievable without assistance. The identity-replication threat requires that the person could do the thing before. Where that baseline was never clean, the threat reads differently.
>
> This population likely warrants its own framework rather than an extension of this one. The gap is noted, not resolved.

---

### P2 — Add Involuntary AI Exposure scope boundary to `populations.md`

**Finding:** 005p § 2. Accepted in full as a scope boundary.

**File:** `populations.md`

**Change:** Add a new section "Involuntary AI Exposure" after the existing "Economic Displacement" section:

> **Involuntary AI Exposure**
>
> This model assumes the person is someone who encounters AI and decides what to do with it. It does not apply to people who are the *subject* of AI — evaluated, filtered, or managed by systems they did not choose.
>
> Examples: insurance claimants processed by AI claims systems, students whose work is graded algorithmically, job candidates filtered before a human reads their materials, bank customers monitored by fraud AI. These people may feel doubt about process fairness, anxiety about misclassification, or anger at opaque systems. But they have not had an S1 Initial Encounter in the model's sense — they made no delegation decision, and the model's machinery does not apply.
>
> Involuntary exposure is a growing situation for large populations. It requires a different framework, not outlined here.

---

### P3 — Note Western secular ethics scope in S2P state file

**Finding:** 005p § 3. Partially accepted. The modeller has limited knowledge of other cultural and religious frameworks; a scope note is appropriate rather than an attempt to extend the diagnostic frame.

**File:** `states/S2P-pre-emptive-non-adoption.md`

**Change:** Add a scope note in the Diagnostic difficulty section, after the current four signals, before "Most real cases are mixed":

> **Scope note:** The diagnostic signals above (cross-domain consistency, evidence response, emotional register, identity-threat removal) are drawn from Western secular ethics traditions — privacy advocacy, labour rights, open-source ethics. They are not validated for religious rejection of AI (where the commitment is to a doctrinal position rather than a values framework of the kind described here) or for community-embedded rejection (where the stance is inherited from collective memory of technological disruption rather than individual ethical reasoning). The modeller does not have sufficient knowledge of other cultural frameworks to extend the diagnostic frame to those contexts.

No change to `populations.md` beyond the existing Pre-emptive Non-Adoption section.

---

### P4 — Note knowledge-worker scope in S3X and Non-Knowledge-Work section

**Finding:** 005p § 4. Partially accepted. The distinction between white-collar narrowing and service/care/manual elimination is real. However, the robotic displacement of care, service, and manual jobs is economically and technologically very unclear. The model should note the gap without speculating on the path.

**File 1:** `states/S3X-structural-displacement.md` — add a scope note to the opening or the Entry condition section:

> **Scope note:** S3X is written for knowledge workers, where displacement follows a narrowing pattern: the collaborative footprint shrinks until no viable position remains. Care, service, and manual roles face a different mechanism — potential total elimination through robotics rather than narrowing through AI capability. How that path differs psychologically is not described here. The robotic displacement trajectory is economically and technologically unclear at the time of writing, and the model does not speculate on it.

**File 2:** `populations.md` Non-Knowledge-Work Domains section — add a sentence at the end:

> The future robotic displacement of care, service, and manual roles is a further step beyond current AI capability and is not described in this model.

---

### P5 — Remove AI researchers and engineers from the out-of-scope list

**Finding:** 005p § 5. Rejected. AI researchers and engineers are not structurally different from other knowledge workers. They have professional identities built around a domain. They can feel threatened when their understanding is undermined. They may tend toward S2T rather than S2D (their identity is built around understanding AI, making open evaluation more comfortable), but the model applies. No special population is needed — it would overcomplicate the model for a small group.

**File:** `Model6.md`

**Change:** Remove the bullet "Users who are already AI experts (AI researchers, engineers, ML practitioners whose professional identity is *about* AI)" from the scope exclusion list.

---

### P6 — Add brief note on market-driven non-adoption to `populations.md`

**Finding:** 005p § 6. Modified. The population 005p describes (teachers at AI-free schools, artisans in no-AI markets) has likely already traversed the model. Their non-adoption is probably not pre-encounter — it follows integration experience. The frame that best describes them is closer to a values-based S7-adjacent decision than a new population: they value the economic position that non-adoption preserves, and they may express that as principled reasoning. That overlap with S2P and the pre-emptive Non-Adoption section is noted, not resolved with a new category.

**File:** `populations.md` Pre-emptive Non-Adoption section — add a note at the end:

> A related but distinct pattern: some practitioners reach non-use after traversing the model, not before it. Their market or professional context economically rewards AI-free work (handmade goods, AI-free therapeutic practice, AI-restricted regulatory roles). This is not S2D or S3B — it is a post-integration decision. It may be expressed as principled reasoning, but the underlying driver is economic. The model does not currently have a state for this position; it sits adjacent to S7E Ethical Integration or an undescribed S7 variant.

---

## Rejected findings (no change)

### Finding 7 — AI-native users (005p § 7)

AI-native users — children and teenagers who have not yet formed a professional identity — do not yet exist as a population this model can observe or describe usefully. `populations.md` already marks the gap. No further expansion.

### Finding 8 — Non-English and non-Western populations (005p § 8)

The critique is valid in principle but overstated in practice. A large part of the world's population speaks English and is substantially influenced by Western professional culture, including across East Asia, South Asia, and urban Africa. The model's Western-psychology basis is fine print, not a critical scope failure. The S2P state file note added in P3 covers the most specific practical misclassification risk (diagnosing culturally-grounded non-adoption as S2D). No separate section in `populations.md`.
