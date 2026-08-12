# Publishing

How to make the model citable, findable, and criticisable, without an institutional affiliation and without a budget.

## What is being published, and as what

The model is a **conceptual framework**, not an empirical finding. This determines the venue, the framing, and what can honestly be claimed.

Theoretical and conceptual contributions are a legitimate publication category. Papers that propose a vocabulary and a structure, and set out how it could be tested, are normal and valuable. The failure mode is not publishing theory — it is publishing theory dressed as evidence.

**The honest framing, used consistently everywhere:**

> A descriptive framework proposing that psychological adaptation to AI in professional work is better modelled as domain-specific positions with modulating conditions than as a linear adoption process. The framework is untested. Its falsifiable predictions are specified.

That last sentence is what makes the work publishable rather than an opinion piece. **The predictions are the contribution as much as the model is.**

## The publication set

Four artefacts, each serving a different purpose. All are free.

### 1. The repository — the living version

**Purpose.** The working source of truth, versioned, revisable, and open to issues and pull requests.

**Requirements:**

- A clear licence. **CC BY 4.0** for the documents — attribution required, derivatives permitted, which maximises spread and adaptation. **MIT** for any code. Avoid non-commercial clauses: they block exactly the practitioner and academic uses that would generate feedback, in exchange for preventing a commercial exploitation that is unlikely and would be visible anyway.
- Frozen version folders. The V3 through V7 structure already does this and it is the right pattern. A reader who cites V7 must be able to read V7 unchanged in five years.
- Issues open, and an explicit statement that critique is wanted.
- A prominent epistemic status in the README, above everything else.

### 2. The archived version — the citable object

**Purpose.** A permanent identifier so the model can be cited and so it cannot silently change under a citation.

**Method.** Zenodo, connected to the repository, minting a DOI per release. Free, permanent, and it accepts non-institutional deposits with no gatekeeping.

**Why this matters more than it appears.** A DOI converts the work from a link that might rot into a citable object. It costs nothing and it is the single highest-leverage administrative act available. It also allows the model to be referenced in a preprint, in an article, and by any practitioner who wants to say where their framework came from.

### 3. The preprint — the academic entry point

**Purpose.** Reach readers who will not read a repository, and invite expert critique.

**Venue.** **PsyArXiv** is the natural home for a psychological framework and accepts preprints from unaffiliated authors. **SocArXiv** is an alternative where the framing leans occupational. **arXiv** requires endorsement in most relevant categories, which is a real barrier without an affiliation and is not worth fighting.

**What the preprint contains.** Not the whole design set. A single self-contained paper: the problem, what existing frameworks do not cover, the positions and axes, the graph, the falsifiable predictions, and the limitations. The full model set stays in the repository and is cited from the paper.

**Realistic length.** Shorter than the design set by a large factor. The discipline of compression will improve the model, because anything that cannot be justified in a paper probably should not be in the framework.

**On peer review.** A journal submission is possible and worth considering, particularly to venues that publish theoretical work in occupational psychology or human-computer interaction. It is slow, the rejection probability without an affiliation is high, and it should not block anything. The preprint comes first regardless; a journal version can follow if there is appetite.

### 4. The public site — the readable entry point

Phase 0 of [06-website-platform.md](06-website-platform.md). Most readers will arrive from a search engine and will not read a paper or a repository.

## Versioning and citation

The project's existing version discipline is unusually good and should be maintained.

| Rule | Reason |
| --- | --- |
| Each version is a frozen folder | A citation must resolve to what was cited |
| Prior versions are never edited to retrofit changes | The record of how thinking changed is part of the contribution |
| Each release gets a DOI | Citable at the version level |
| Retired identifiers are never reused with new meanings | This is why V7 dropped numbers. It should be stated in the publication, because it is a real methodological point about model notation |

## Authorship and standing

The absence of an institutional affiliation is a genuine disadvantage for reach and a smaller one for legitimacy than it appears. The practical mitigations:

- **State the position plainly.** An independent researcher who is explicit about it is in a better position than one who obscures it. Overclaiming affiliation or expertise would be far more damaging than having neither.
- **Lead with the limitations.** Work that states its own weaknesses precisely reads as more credible, not less, to the readers whose opinion matters.
- **Let the falsifiers do the work.** A framework that specifies how it could be refuted signals seriousness more effectively than any credential.
- **The domain expertise is real and relevant.** A practising software engineer writing about professional identity under AI capability change has direct access to the phenomenon. This should be stated as the basis of the observations, which also correctly frames them as observations rather than data.

## Getting it read

Publication is not distribution. Concrete routes, ordered by likely return:

| Route | Notes |
| --- | --- |
| Articles for specific audiences | The main mechanism. See [08-articles.md](08-articles.md) |
| Direct approach to researchers in adjacent fields | A short, specific message asking whether the framework duplicates existing work is more likely to get a reply than one asking for endorsement, and the answer is more useful |
| Practitioner communities | Engineering leadership, coaching, and organisational development communities have the readers most likely to use it |
| Conference or meetup talks | Local and practitioner events are accessible without affiliation and produce better feedback than online posting |
| Responding substantively where the topic is discussed | Slow, but it reaches exactly the right people |

**What not to do.** Press releases, engagement-optimised summaries that drop the caveats, and anything that describes the framework as research findings. The model's credibility is the only asset the project has, and it is spent permanently on first misuse.

## An explicit call for what is missing

Every publication artefact should carry a short, specific statement of what the project needs. Vague invitations to collaborate produce nothing; specific requests occasionally work.

> This framework has not been tested. Three things would advance it, and none require funding the author does not have: anonymised workflow data on review-to-production ratios, a second rater willing to classify a small set of cases independently, and a student project able to run the discriminability study properly. Contact details follow.

This converts every reader into a possible collaborator and is free to include.

## What honesty requires in every artefact

- The epistemic status appears before the content, not after it.
- No claim of validation, evidence base, or scientific status.
- Conjectures marked as conjectures, in the published version and not only in the working documents.
- Prior work credited properly, including any case where an existing construct turns out to be better supported than the model's version of it.
- Where the model changes in response to critique, the change is visible rather than quietly applied.

The last point is a genuine opportunity. A framework whose author publicly revises it under criticism accrues credibility that no amount of initial polish can buy, and the V6 review corpus shows the practice already exists in the project. Making that visible is worth more than presenting a finished object.
