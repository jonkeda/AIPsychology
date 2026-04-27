---
applyTo: ".my/reviews/**"
---

# Writing Style Guide — Reviews

These rules apply to any review, critique, or feedback document written into `.my/reviews/**` (typically reviews of the psychological models in `Model/`).

## Audience

The reader is a 56-year-old software engineer with **little academic background and little psychology background**. Write for that reader. Not for an academic. Not for a peer reviewer at a journal.

If a sentence would only make sense to someone with a psychology degree, rewrite it.

## Tone

- **Blunt and direct.** No hedging, no diplomacy, no "this is a thought-provoking contribution."
- Say what's wrong. Say why. Move on.
- Disagreement is fine. Softening language is not.
- Do not flatter. Do not pad.

## Structure

Every review uses this shape:

1. **TL;DR** — 3–8 bullet points. The reader should be able to stop here and know what changed in their head.
2. **Findings** — the actual critique. Numbered. One issue per item.
3. **Recommendations** — concrete proposed changes, prioritized.

No preamble. No "In this review I will…". Start with the TL;DR.

### Finding headings are verdicts, not topics

Write the heading as a complete claim about what is wrong. The reader should know the conclusion before reading the body.

Good: `### 2. The ⚡ marker on S3B Bargaining is overstated`
Bad: `### 2. S3B Bargaining — ⚡ usage`

If the finding is about a claim the model makes that can be tested, append `— testable` to the heading. If it cannot yet be tested, append `— not yet tested`.

Good: `### 3. "Most people cycle through more than once" — testable`

### Fix: belongs inside the finding

Put a `**Fix:**` line at the end of every finding body, immediately below the problem description. Do not wait for the Recommendations section. Recommendations re-lists priorities; `Fix:` is where the reader finds out what to change.

The Recommendations section should still exist and list the fixes in priority order, but it should not be the only place they appear.

## File naming and numbering

Reviews must be numbered so the chronological order is obvious from the filename alone.

- Format: `NNN-<slug>.md` where `NNN` is a zero-padded sequence number starting at `001`.
- The number is **assigned at creation time** based on the highest existing number in the same folder, plus one. Do not renumber existing files when adding a new one.
- The slug describes the review (`001-model4-falsifiability.md`, `002-v3-v4-diff.md`, …).
- Subfolders restart their own sequence (e.g., `Goals1/001-…`, `Goals1/002-…`).
- Multi-part reviews keep one number and append `.partN`: `003-foo.md`, `003-foo.part2.md`, `003-foo.part3.md`. The number is the *review's* index, not the file's.
- When linking between reviews, link by filename. The number doubles as the citation key.

## ⚡ External-trigger markers (when reviewing the models)

If a review touches the ⚡ trigger convention used in the Model documents, the rule the model is supposed to follow is:

- A state carries ⚡ if and only if there is at least one **named external event** (model release, mandate, media wave, regulatory change, peer adoption shift, AI failure) that materially changes the *probability* of entering or leaving that state.
- States that change only through internal cognition or ambient social context do not carry ⚡.
- The marker means "this transition has a discrete, dateable cause." If a reviewer can't name the event, the marker shouldn't be there.

Reviews that find ⚡ inconsistencies should hold the model to that rule, not to a softer "looks plausible" reading.

## Length

Tiered:

- **Executive summary on top** (TL;DR + a 1-paragraph verdict). Must be readable in under 2 minutes.
- **Deep dive below**, as long as the substance requires. Don't pad to look thorough; don't truncate to look concise.

If the deep dive is long, add a short table of contents after the TL;DR.

## Splitting across multiple files

If a review would be cut off by output/token limits, **split it across multiple files** rather than truncating or summarizing away substance.

- Naming: `<review-name>.md`, `<review-name>.part2.md`, `<review-name>.part3.md`, …
- The first file always contains the full TL;DR and verdict, plus a `## Continued in` section listing the follow-up files in order.
- Each follow-up file starts with a one-line back-reference: `Continuation of [<review-name>.md](<review-name>.md). Part N of M.`
- Don't repeat content across parts. Pick up where the previous part stopped.
- Prefer splitting on **section boundaries** (e.g., Findings 1–8 in part 1, Findings 9–15 + Recommendations in part 2), not mid-finding.

Better to deliver the full critique across 3 files than a watered-down version in 1.

## Language rules

- **Plain English first.** Short sentences. Concrete nouns. Active voice.
- **Jargon is allowed, but define it on first use** in one short parenthetical. Examples:
  - "cognitive dissonance (the discomfort of holding two beliefs that contradict each other)"
  - "self-efficacy (a person's belief that they can actually do the thing)"
- After the first definition, you may use the term freely.
- Avoid Latin abbreviations (i.e., e.g., cf., etc.) — write "for example", "such as", "compare with".
- Avoid academic throat-clearing ("It is worth noting that…", "One might argue…"). Just say it.

### State labels need a plain gloss every time they appear in a new finding

Every state label (S2D, S3B, S7A, and so on) must have a short plain-English gloss on its first appearance in each finding where it shows up. Use a parenthetical immediately after the label.

Example: `S3B Bargaining (where someone makes a deal with themselves to use AI for some things but not others)`

After the first definition inside a finding, you may use the label alone for the rest of that finding. But if the label reappears in a new finding, gloss it again there.

Do not assume the reader remembers what a state means from three findings earlier.

### Use conversational signposts to guide the reader

Before a numbered list, a test protocol, or a chain of logic, use a short cue phrase: "Here's how:", "Here's the trap:", "Here's why:", "Four things can go wrong:". This tells the reader what is coming and why they should read it.

Do not use a bullet list where a short cued paragraph is clearer. Lists are for parallel items. Narrative with a signpost is for causation and sequence.

## Citing prior work

When referencing existing theories or authors:

- Mention by name + a **one-sentence plain-English gloss** of what it says.
- No formal citations, no bibliography, no page numbers.
- Example: "This overlaps with the Technology Acceptance Model (Davis, 1989) — the idea that people adopt tech mostly based on whether they think it's useful and whether they think it's easy to use."
- If a name adds nothing for the reader, drop it.

## Concreteness

- **Specific where it matters, general where it doesn't.**
- Any critique of a *specific stage, transition, or claim* must point at it directly — quote the line or name the section. No vague "Stage 4 feels weak."
- High-level observations about the model as a whole can stay general, but should still be falsifiable ("the model has no failure mode for X" is fine; "the model feels off" is not).
- When a finding describes a testable claim and proposes a study, include a rough sample size, time horizon, and cost estimate. A ballpark that is wrong by 50% is more useful than nothing. Example: "40 people across two model releases, about $50k." Keep it to one line.

## Actionability

- **Prefer fixes.** Most critiques should end with a concrete proposed change: rename, merge, split, add, delete, reorder, or define.
- **Open questions are allowed** when no good fix is obvious — but mark them clearly as `Open question:` so they aren't mistaken for findings.
- Do not list a problem and walk away unless you've explicitly flagged it as an open question.

## Software-engineering analogies

The reader is a software engineer. SE analogies (state machines, type systems, edge cases, invariants, dead code, API contracts) are allowed **sparingly** — only when they genuinely clarify a psychological point faster than plain language would. Don't force them. Don't use them as decoration.

## Formatting

- Markdown. Headings, bullets, numbered lists.
- Bold for the one or two words in a finding that carry the point. Don't bold whole sentences.
- Code fences only for literal quotes from the model or for structured diagrams.
- No emojis unless the source model uses them and you're referring to one.

## What NOT to do

- Don't review the prose quality unless prose quality is the explicit goal of that review.
- Don't restate the model back to the author — they wrote it.
- Don't grade ("7/10", "B+"). Say what's broken and what to change.
- Don't end with "Overall, this is a strong contribution…". End with the last recommendation.
