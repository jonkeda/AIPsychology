---
applyTo: ".my/Model/**"
---

# Writing Style Guide — Model Documents

These rules apply to the psychological-model documents under `.my/Model/**` (e.g. `Model3.md`, future `Model4.md`, `Model5.md`, …).

## Audience

**Mixed.** Two readers must both be able to use the document:

1. A 56-year-old software engineer with little academic or psychology background.
2. An academic-leaning reviewer who expects rigor.

When the two pull in opposite directions: write the substance for the academic reader, but never let a sentence be unreadable to the engineer. If a paragraph only works for one of the two, rewrite it.

## Tone

**More formal than the reviews guide, but not stiff.**

- Descriptive and precise, not chatty.
- Third person. Avoid "I" and "you" outside of stage-quote examples ("AI won't work" style).
- No marketing language, no hype, no rhetorical questions to the reader.
- Hedging is allowed where the underlying claim is genuinely uncertain ("often", "tends to", "may"). Don't hedge to sound humble — hedge to be accurate.
- No throat-clearing ("It is worth noting that…"). State the claim.

## Language

- **Plain-English-first, jargon-allowed.** Define each piece of jargon on first use in a short parenthetical or inline gloss. Same rule as the reviews guide.
- Reuse defined terms consistently. If you call it "ego shock" once, don't switch to "identity rupture" later.
- Avoid Latin abbreviations (i.e., e.g., cf., etc.) — write "for example", "such as", "compare with".
- Prefer concrete behavioral language over abstract psychological language when both work.

## Structure

**No required template.** Each version may organize itself however best fits its content.

Soft expectations (not rules):

- Open with a one- or two-paragraph statement of what the model is and what it claims.
- Define axes/dimensions before the stages that use them.
- Use tables for anything matrix-shaped (delegation × stage, dropout types, end states).
- Use headings generously. The document should be navigable by table of contents alone.

## Versioning & file layout

- **One subfolder per version**, even if the version is a single file.
  - `.my/Model/v3/Model3.md`
  - `.my/Model/v4/Model4.md`
  - `.my/Model/v5/Model5.md`
- The subfolder also holds **all supporting docs for that version** (diagrams, source material, notes, derived artifacts). Don't scatter version-specific files into `.my/Model/` root.
- The previous version's folder is **frozen**. Never edit a prior version's documents to retrofit changes — start a new version instead.
- **No changelog required.** Don't include "Summary of Changes from vN-1 to vN" tables unless the change is genuinely useful as part of the new model's exposition. Git history is the changelog.

## Splitting across multiple files

A model version may be split into multiple files **only when the single-file size would risk hitting context/token limits during reading or editing** by an LLM. Don't split for stylistic reasons.

When splitting:

- Naming follows the reviews-guide convention: `Model4.md`, `Model4.part2.md`, `Model4.part3.md`, …
- The first file (`Model4.md`) is the entry point: it states what the model is, lists the axes, and contains a `## Continued in` section linking the parts in order.
- Each follow-up part starts with a one-line back-reference: `Continuation of [Model4.md](Model4.md). Part N of M.`
- Split on **section boundaries** (e.g., stages 0–4 in part 1, stages 5–7 + dropout + cultural in part 2). Never split mid-stage or mid-table.
- Don't duplicate content across parts.

All parts live in the same version subfolder.

## Diagrams

Diagrams are **optional but encouraged** where they clarify faster than prose:

- Mermaid state diagrams for stage transitions.
- Mermaid flowcharts for branching paths (e.g., 1A vs 1B).
- ASCII tables/diagrams are acceptable for small matrices.

Rules:

- Every diagram must be referenced from the surrounding prose. No floating diagrams.
- Diagrams supplement; they never replace a written description of the same content.
- Keep diagrams readable when rendered in plain markdown viewers — don't rely on color or interactivity.

## Tables

Use tables for any content where the natural shape is a grid:

- Delegation level × psychological weight
- Stage × example experience
- Dropout type × characteristics
- End state × description

Each table should have a one-sentence lead-in explaining what the table shows.

## Stages, axes, and named constructs

When the model introduces a named construct (a stage, axis, end state, dropout type):

- Give it a **short label** (`Stage 3`, `Stage 3B`, `D2`, `7F`) and a **descriptive name** (`Ego Shock`, `Bargaining`, `Task execution`, `Influence / Evangelism`).
- Open with a **one-line quoted "voice of the person"** where applicable — this is the engineer-friendly anchor (e.g., *"AI won't work. It's overhyped."*).
- Follow with a short paragraph stating what the construct *is* in plain language.
- Then the formal/structural details: transitions, triggers, sub-types, modulating axes.

Keep this order consistent across stages within a version. Different versions may evolve the order, but within one document it must be uniform.

## Claims and evidence

The model is descriptive, not empirical — but every claim should be at least **plausibly falsifiable in principle**.

- Avoid claims that are tautological or that explain every outcome post-hoc.
- When a claim rests on a known body of work (e.g., cognitive dissonance, self-efficacy, Technology Acceptance Model), name it inline with a one-sentence gloss. No formal citations, no bibliography.
- Mark genuinely speculative material as such ("This is hypothesized, not observed:" or similar).

## Formatting

- Markdown. Headings, bullets, numbered lists, tables.
- Bold for the key word(s) in a claim. Don't bold whole sentences.
- Code fences only for diagrams or literal example prompts.
- Use `⚡` (or a similarly stable ASCII marker) consistently for external triggers across stages — pick one and stick with it within a version.
- No emojis as decoration.

## What NOT to do

- Don't retrofit older versions. Start a new subfolder.
- Don't pad with restatements ("As mentioned above…").
- Don't summarize the model back to itself in a closing section.
- Don't include changelogs unless they're substantively useful.
- Don't mix model content with review/critique content. Reviews go under `.my/reviews/`.
