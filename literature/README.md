# Literature Archive

This directory is the canonical archive for scientific and scholarly literature used during dissertation brainstorming, candidate-program development, comparison, and later faculty-brief preparation.

The goal is not merely to collect links. The archive should make it possible to trace:

`source -> extracted claim -> analysis/discussion -> candidate program -> decision`

## What belongs here

Include literature that materially informs the project, such as:

- peer-reviewed journal articles
- conference papers
- systematic reviews and meta-analyses
- methodological papers
- benchmark and evaluation papers
- preprints when sufficiently relevant and clearly labeled
- scholarly perspective, roadmap, or consensus articles
- other research literature that directly informs scientific novelty, feasibility, methods, evaluation, or research gaps

High-quality industry reports, official institutional sources, faculty profiles, government sources, and market evidence remain valid project sources, but they should be cataloged through the broader `sources/` and `evidence/` structure rather than being treated as scientific literature.

## Directory structure

- `index.md` — master literature registry
- `records/` — structured notes for individual sources
- `records/TEMPLATE.md` — required source-note template

## Literature indexing rule

Any paper or scholarly article that materially influences a candidate definition, novelty claim, research-gap claim, methodological recommendation, ranking, or faculty-facing statement should be entered into `index.md` and, when substantively used, should receive an individual record in `records/`.

A source being mentioned in a discussion does not automatically make its conclusions accepted evidence.

## Source IDs

Assign stable IDs sequentially:

- `LIT-001`
- `LIT-002`
- `LIT-003`
- etc.

Use the same ID in the index, source record, evidence notes, analyses, and decisions when practical.

Do not reuse an ID for a different source.

## Reading / verification status

Use one of these statuses:

- `DISCOVERED` — identified but not yet examined sufficiently
- `SCREENED` — title/abstract or equivalent has been checked
- `READ` — substantive content has been examined
- `VERIFIED` — bibliographic details and the claims used in this project have been checked against the source
- `RETIRED` — previously relevant but no longer relied upon; preserve the record and explain why

Do not use `DISCOVERED` or `SCREENED` sources as strong support for detailed scientific claims that require full-text examination.

## Evidence discipline

For each substantively used source, distinguish:

- what the source actually reports
- what the project infers from it
- what it does not establish
- limitations relevant to our use
- whether the source supports, challenges, or merely contextualizes a candidate

Scientific novelty should never be inferred from one paper alone. Novelty and saturation claims should be based on a sufficiently broad literature view.

## Provenance discipline

Each source record should identify where the source was used, for example:

- `discussion_01/...`
- `discussion_02/...`
- `discussion_03/...`
- `analysis/analysis_01/...`
- `analysis/analysis_02/...`
- `analysis/analysis_03/...`
- `candidate_programs/...`
- `decisions/decision_log.md`
- `meeting_materials/...`

This allows later reviewers to reconstruct why a source mattered.

## Copyright and file-storage rule

Do not place copyrighted full-text PDFs in the repository unless redistribution/storage is clearly permitted and there is a reason to keep a repository copy.

Normally store:

- full citation
- DOI / PMID / arXiv identifier / official URL
- open-access or publisher link where appropriate
- structured notes and extracted project-relevant claims

If an openly licensed or otherwise permitted local copy is stored later, record its license/status and repository path in the source record.

## Relationship to other project directories

`literature/` = the scholarly source archive and reading provenance.

`evidence/` = distilled claims and evidence used to compare dissertation programs.

`sources/` = broader source registry and source-type guidance, including official and industry material.

`discussions/` = reasoning history.

`analysis/` = independent synthesis and critique.

`decisions/` = accepted project state.

These layers should remain distinct.