# Decisions

Every open decision for V7. Each is stated as a question, followed by options as a task list. **The recommended option is already checked.** The reasoning follows each set.

A decision is only listed here if it is genuinely open — if reasonable people working from the same material could pick differently. Settled matters are in the model files.

Decisions are grouped by what they affect. Within each group they are ordered by how much else depends on them.

---

# Group A — Identifiers and structure

## D-A1. What replaces the S-number scheme?

- [X] **Two-letter mnemonic codes with word-named families.** `NE` No Engagement, `FC` First Contact, `OE` Open Evaluation, `GE` Guarded Evaluation, `VR` Values Refusal, `IS` Identity Shock, `SB` Scope Boundary, `CU` Calibrated Use, `OU` Overuse, `OL` Oversight Load, `IP` Integrated Practice, `BO` Burnout, `SD` Structural Displacement, `DX` Disengagement.
- [ ] Renumber the S-scheme to close the `S4` gap and regroup families.
- [ ] Keep V6 identifiers unchanged and document the gap and the family mismatches.
- [ ] Drop short codes entirely; use full names only.

**Why the recommendation.** The numbering is the source of the model's most persistent misreading. Ordinal identifiers imply an order the model explicitly denies, and no disclaimer survives contact with a ladder. Renumbering makes it worse rather than better: the pre-V7 proposal would have made `S5` mean Understanding in one version and Overuse in the next, so every V6 review document becomes actively misleading rather than merely outdated. Mnemonic codes carry no order, no arithmetic, and no family promise, and they allow new positions to be added without disturbing anything. Full names only would be cleanest of all but is unusable in tables and in the multi-domain notation practitioners need.

**Cost of the recommendation, stated honestly.** Every V6 document needs translation, the review corpus refers to retired tokens, and anyone fluent in V6 has to relearn. The translation table in [02-identifiers.md](02-identifiers.md) is exact and one-directional, which makes the cost finite.

## D-A2. Should the six renames go ahead?

Defensive Resistance → Guarded Evaluation, Ego Shock → Identity Shock, Bargaining → Scope Boundary, Understanding → Calibrated Use, Pre-emptive Non-Adoption → Values Refusal, Evangelism → Advocacy.

- [X] **Rename all six.** The old names carry evaluative or theoretical freight the model does not intend.
- [ ] Rename only the two worst offenders (Bargaining, Defensive Resistance) and keep the rest.
- [ ] Keep all V6 names and change only the codes.

**Why the recommendation.** If the codes are changing anyway, the marginal cost of fixing the names is near zero, and this is the only opportunity to fix them without a second disruption. Each name was doing damage: "Resistance" takes the organisation's side against the person, "Bargaining" imports the Kübler-Ross association the model spends paragraphs denying, "Understanding" implies everything before it was misunderstanding, "Ego" invokes an apparatus the model cannot support.

## D-A3. Is `OL` Oversight Load a position or an attribute?

- [X] **A position in the Working family, marked provisional pending the Verification Burden study.**
- [ ] An attribute of `CU` Calibrated Use and `OU` Overuse only — the Verification Burden axis already carries it.
- [ ] Not in V7 at all; revisit when there is evidence.

**Why the recommendation.** The deciding argument is the exit structure, not the phenomenology. `OL` Oversight Load routes to `BO` Burnout through a mechanism that has nothing to do with the person's own usage choices. Folding it into `OU` Overuse attributes the load to decisions the person frequently did not make, which is exactly the misdiagnosis the model exists to prevent. Marking it provisional is honest about the evidence, and the falsifier is unusually clean: if raw usage volume predicts burnout as well as verification burden does, `OL` Oversight Load collapses into `OU` Overuse and the model is simpler for it.

## D-A4. Should `DX` Disengagement be a named position?

- [X] **Yes. Name it, give it the two severity axes, and let every position have an edge to it.**
- [ ] Keep it as a cross-cutting concept outside the position set, as in V6.

**Why the recommendation.** "Reachable from everywhere" describes an edge set. It is not a reason to leave a thing unnamed, and the V6 arrangement meant the most common real-world outcome in the whole model had no identifier and could not appear in a position statement.

## D-A5. Does market-driven non-use need its own position?

Practitioners who arrive at non-use after traversing the model, because their market rewards demonstrably AI-free work.

- [X] **No. Record as `DX` Disengagement with low severities and a stated reason.**
- [ ] Yes — a new position in the Exit family.
- [ ] Yes — an attribute of `IP` Integrated Practice, since the person integrated and then chose out.

**Why the recommendation.** The psychological content is thin. The person made a business decision they are comfortable with, and the model's machinery — identity threat, defensive updating, ceilings — has nothing to explain. Adding a position for a case the model does not illuminate is how state counts get to eighteen.

---

# Group B — Model stance

## D-B1. Descriptive, prescriptive, or description plus declared editorial?

- [X] **Description plus a separately labelled editorial annex.** The model layer carries no evaluative language; one clearly signed annex states which positions the author considers sustainable.
- [ ] Pure description. Delete the sustainability material entirely.
- [ ] Openly prescriptive. Name target positions and say so.

**Why the recommendation.** V6 claimed pure description while shipping a ranking, which is the incoherence behind several reviewer objections. Of the three coherent resolutions, the annex is best. Pure deletion discards genuinely useful practitioner material — the observation that sustained `OU` Overuse: anxiety corrodes and that `IS` Identity Shock is not a place to live is worth having. Open prescription requires evidence the model does not have, and would license using position labels to push people, which is the misuse the model most needs to prevent. The annex separates the author's judgement from the map cleanly enough that a practitioner can discard one and keep the other.

**Consequence to accept.** The model becomes less immediately actionable. Practitioners wanting a target will not find one.

## D-B2. What is the sustainability annex called, and where does it live?

- [X] **`sustainability-annex.md`, outside the model file set, opening with an explicit statement that it is the author's opinion.**
- [ ] Keep the V6 name `healthiness.md` inside the model set.
- [ ] Fold the content into each position description as a "cost" note.

**Why the recommendation.** "Healthiness" is clinical vocabulary the model has no standing to use. Folding cost notes into position descriptions reintroduces exactly the evaluative language D-B1 removes, one paragraph at a time.

## D-B3. Do `OE` Open Evaluation and `GE` Guarded Evaluation stay as separate positions?

- [X] **Yes, separate — pending the asymmetric-updating study, which is a defined falsifier.**
- [ ] Collapse into one Evaluation position with a `stance: open | guarded` attribute.

**Why the recommendation.** They present identically in a snapshot, which is a real argument for collapsing. But their downstream trajectories diverge sharply — `OE` Open Evaluation reaches `CU` Calibrated Use directly, `GE` Guarded Evaluation almost never does without passing through the Disruption family — and a model whose whole purpose is anticipating trajectory should not merge nodes with different exits. The falsifier is already specified: if bidirectional updating fails to separate them in a real sample, they collapse in V8 with the evidence in hand rather than on argument.

## D-B4. Does `VR` Values Refusal stay a position?

- [X] **Yes, with the scope limit stated and the falsifier specified.**
- [ ] Demote to an attribute of `GE` Guarded Evaluation (`ethical-overlay: present`).

**Why the recommendation.** The domain-transfer signal is genuinely discriminating — a values position holds in domains where the person has no competence to defend, and a competence position dressed in ethical language does not. That is a real distinction with a real test. The V6 review that recommended demotion was right that most observed cases are mixed, but mixed cases are an argument for better diagnostics, not for deleting one of the two things being mixed.

## D-B5. How is the cohort question handled?

- [X] **A cohort property (`pre-AI`, `concurrent`, `AI-native`) with a claim about which families transfer.**
- [ ] Keep V6's exclusion of AI-native users from scope.
- [ ] Extend the model fully to AI-native users.

**Why the recommendation.** The exclusion has become impractical — a team assessment silent about a third of the team is not usable. Full extension is unsupportable, because the Disruption family requires a baseline competence to threaten and the AI-native case may not have one. The property records the distinction and makes a falsifiable claim about what transfers, which is the most that can be said honestly.

---

# Group C — Axes

## D-C1. Does Identity Stakes get a third level?

- [X] **Yes — Low, Moderate, High.**
- [ ] Keep the binary.
- [ ] Move to a continuous 0–10 scale.

**Why the recommendation.** Most real cases sit between the binary's two values, and forcing a choice discards information. A continuous scale implies a measurement precision that does not exist and would invite arithmetic the model cannot support.

## D-C2. Does the delegation scale extend to D5?

- [X] **Yes. D5 is objective delegation — the person specifies an outcome and does not observe the process.**
- [ ] Keep D1–D4 and treat long-horizon execution as extended D4.
- [ ] Restructure the scale entirely around what the person retains rather than what they hand over.

**Why the recommendation.** D5 is qualitatively different, not merely more. At D4 the person can locate their contribution; at D5 the honest answer is that they decided the thing should exist and decided it was good enough. That difference does psychological work the existing scale cannot express. The third option is attractive and should be revisited in V8 — "what the person retains" may be the better organising principle for the whole axis — but restructuring the axis and adding a level in the same version makes both changes unevaluable.

## D-C3. Is Verification Burden an axis?

- [X] **Yes — a fourth axis, per-workflow, with `exceeded` as the significant level.**
- [ ] An attribute of `OL` Oversight Load only.
- [ ] Not in V7.

**Why the recommendation.** It varies independently of position — two people with identical burden can hold very different positions, one satisfied and one drowning — which is the definition of an axis rather than a state property. It is also the most measurable construct the model has, since verification time comes out of ordinary workflow data without instrumenting the person.

## D-C4. Is Attribution Exposure a fifth axis?

Whether the person's AI use is visible and disclosed, and whether they are credited for the output.

- [ ] Yes — add it as a fifth axis.
- [X] **No. Record it in the social context layer for now and revisit in V8.**
- [ ] Add it as an attribute of `IP` Integrated Practice: ethical and `OU` Overuse: social.

**Why the recommendation.** It is real and it matters, particularly in creative fields where disclosure norms are hardening. But four axes is already at the limit of what a practitioner can hold in a conversation, and its effects currently run through `OU` Overuse: social and `IP` Integrated Practice: ethical without much loss. Adding a fifth axis in the same version as a fourth would make neither assessable.

## D-C5. Is the Delegation Ceiling tool-specific or domain-specific?

- [ ] Purely domain-specific, as in V6.
- [X] **Primarily domain-specific with a stated conjecture that it is partly tool-specific, and a study to settle it.**
- [ ] Redefine as tool-specific.

**Why the recommendation.** Tool deprecation appears to reset ceilings — trust built with one system does not fully transfer to its replacement. That observation is too consistent to ignore and too unstudied to build on. Recording it as a marked conjecture with a defined study is the correct weight.

---

# Group D — Measurement and validation

## D-D1. What is validated first?

- [X] **Inter-rater reliability on position classification, before anything else.**
- [ ] Construct validity of the axes first.
- [ ] Predictive validity of the transitions first.
- [ ] A large descriptive survey first, to establish base rates.

**Why the recommendation.** If two trained raters cannot agree on which position a person is in, every other study is measuring noise and no result from them means anything. Reliability is also the cheapest study in the programme and the one most likely to force a structural change early — the `SB` Scope Boundary versus `IP` Integrated Practice: mastery and `OE` Open Evaluation versus `GE` Guarded Evaluation pairs are where the model is most likely to fail, and finding that out before investing in longitudinal work is worth a great deal. See [20-testing.md](20-testing.md).

## D-D2. How is contamination from model exposure handled?

Once a person knows the model, self-report becomes a performance of it.

- [X] **Validation samples must be model-naive. Instruments must describe behaviour without naming positions.**
- [ ] Accept contamination and correct for it statistically.
- [ ] Use only exposed participants, since they can self-locate more accurately.

**Why the recommendation.** There is no correction for demand characteristics of this magnitude, and self-location by an exposed participant measures how well they read the model, not where they are. Model-naive sampling gets harder every month the model circulates, which is an argument for running the reliability and instrument work early rather than a reason to abandon the requirement.

## D-D3. Does the model ship a self-report instrument?

- [ ] Yes — a validated questionnaire is the highest-value deliverable.
- [X] **Not yet. Ship a structured interview protocol and behavioural indicators; build the questionnaire only after reliability is established.**
- [ ] Never. The constructs are not questionnaire-tractable.

**Why the recommendation.** A questionnaire published before reliability is established would be used as a diagnostic instrument regardless of any disclaimer attached to it, and the misuse would be attributed to the model. "Never" is too strong — several constructs are tractable — but the order matters, and shipping the instrument last is the only way to avoid the harm.

## D-D4. Is the 0–10 dropout severity scale kept?

- [ ] **Keep with anchors, and state plainly that inter-rater reliability is unestablished.**
- [X] Replace with a three-level ordinal scale.
- [ ] Drop the numbers; keep the two-axis quadrant only.

**Why the recommendation.** The quadrant is what practitioners actually use and the numbers add little, which argues for the third option. But the anchors are good, the scale is already in circulation, and reducing precision now would need reversing if the reliability study comes back acceptable. Keep and flag.

---

# Group E — Scope

## D-E1. Does the model describe collective positions?

Teams, departments, and professions visibly move as units.

- [ ] Yes — add a collective layer in V7.
- [X] **No. Record the gap explicitly and design the individual model so a collective layer can be added later without restructuring.**
- [ ] Treat aggregated individual positions as the collective position.

**Why the recommendation.** The gap is real and the individual frame genuinely misses it. But a collective layer is a substantial modelling problem — collective positions are not sums of individual ones, and a profession negotiating a scope boundary through its standards body is a different kind of object from a person doing it. Attempting it in the same version as the identifier change would compromise both. The third option is actively wrong and should be blocked explicitly, because it is what people will do by default.

## D-E2. Does the model take a position on skill atrophy under sustained delegation?

- [ ] Yes — state the expected mechanism and mark it conjecture.
- [X] **No. Record it as the model's largest open question and specify the study.**
- [ ] Yes — treat sustained D4/D5 use as producing atrophy by definition.

**Why the recommendation.** This is the question every practitioner eventually asks and the one the model is least equipped to answer. Taking a position without evidence would be the model's most consequential overclaim, and the third option builds the conclusion into the definition, which makes it unfalsifiable. Marking it as the largest open question is not evasion — it is the accurate description of the state of knowledge, and the study is specified in [20-testing.md](20-testing.md).

## D-E3. Do involuntary-exposure and assistive-use populations stay out of scope?

- [X] **Yes, both, with the reasons stated and the gaps named.**
- [ ] Extend the model to cover involuntary exposure.
- [ ] Extend to assistive use.

**Why the recommendation.** Both would require the model's core vocabulary to mean something different. Involuntary exposure has no delegation decision, so there is no `FC` First Contact in the model's sense. Assistive use breaks the assistive-versus-competitive distinction the Disruption family rests on. Naming the gaps is more useful than a bad extension, because a named gap tells a practitioner to look elsewhere and a bad extension tells them they have an answer.

---

# Sequencing

The decisions are not independent. This order avoids rework.

| Order | Decisions                    | Why here                                                    |
| ----- | ---------------------------- | ----------------------------------------------------------- |
| 1     | D-A1, D-A2                   | Every other document depends on the identifiers             |
| 2     | D-B1, D-B2                   | The stance determines what language is permitted throughout |
| 3     | D-C1, D-C2, D-C3             | Axes are referenced by every position description           |
| 4     | D-A3, D-A4, D-A5, D-B3, D-B4 | Position set can now be finalised                           |
| 5     | D-B5, D-E1, D-E2, D-E3       | Scope statements                                            |
| 6     | D-D1 to D-D4, D-C4, D-C5     | Validation programme; can proceed in parallel with writing  |

## Decisions deliberately deferred to V8

Recorded so they are not rediscovered as novel.

- Restructuring the delegation axis around what the person retains rather than what they hand over (D-C2, third option).
- Attribution Exposure as a fifth axis (D-C4).
- A collective layer (D-E1).
- Collapsing `OE` Open Evaluation and `GE` Guarded Evaluation, if the updating study fails to separate them (D-B3).
- Demoting `VR` Values Refusal, if the stability study shows it resolves under threat removal (D-B4).
- Collapsing `OL` Oversight Load into `OU` Overuse, if verification burden does not out-predict usage volume (D-A3).

Three of the six are contingent on studies specified in [20-testing.md](20-testing.md). That is the intended design: the model should shrink when evidence says it should, and each of these has a defined condition under which it does.
