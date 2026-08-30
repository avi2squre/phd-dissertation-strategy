# LIT-026 - LLMs (Almost) Never Abstain Under Medical Uncertainty

## Bibliographic record

- **ID:** LIT-026
- **Full citation:** Cocchieri, A., Ragazzi, L., Tagliavini, G., and Moro, G. (2026). LLMs (Almost) Never Abstain Under Medical Uncertainty. In *Proceedings of the 64th Annual Meeting of the Association for Computational Linguistics (Volume 1: Long Papers)*, 29573-29613. Association for Computational Linguistics.
- **Authors:** Alessio Cocchieri; Luca Ragazzi; Giuseppe Tagliavini; Gianluca Moro
- **Year:** 2026
- **Venue / publisher:** 64th Annual Meeting of the Association for Computational Linguistics, Volume 1: Long Papers / Association for Computational Linguistics
- **Source type:** Conference paper; benchmark paper
- **Peer-reviewed:** Yes
- **DOI:** 10.18653/v1/2026.acl-long.1365
- **PMID:** None identified
- **arXiv / other identifier:** ACL Anthology 2026.acl-long.1365
- **Official URL:** https://aclanthology.org/2026.acl-long.1365/
- **Open-access URL, if any:** https://aclanthology.org/2026.acl-long.1365.pdf
- **Date added:** 2026-08-30
- **Last verified:** 2026-08-30 (bibliographic metadata and abstract only)
- **Status:** SCREENED

## Why this source matters

Stream 02 cited MedQAbstain in its 2026-07-29 historical critique as evidence that medical abstention already had a dedicated benchmark. This record identifies the exact paper and keeps the broader crowding inference separate.

## What the source actually establishes

At `SCREENED` depth, the official ACL Anthology metadata and abstract establish that:

1. The paper introduces MedQAbstain, a benchmark for medical abstention under uncertainty.
2. The benchmark modifies medical multiple-choice question-answering settings by removing the gold answer and adding an explicit abstention option.
3. The abstract reports that the evaluated state-of-the-art language models systematically overcommitted and rarely abstained, including settings where the question was hidden.

No claim beyond the official metadata and abstract was checked during this provenance pass.

## Project interpretation

**Historical Stream 02 inference:** MedQAbstain meant that “predict failures and abstain” alone was unlikely to be a sufficient dissertation novelty claim; Stream 02 therefore linked abstention to an evidence-state representation and multi-action policy.

This inference is preserved as provenance. It has not been independently validated through a full-text review or broader abstention-literature search.

## What this source does NOT establish

- It does not establish that medical abstention research is saturated.
- It does not establish a general controller spanning retrieval, clarification, belief preservation, belief revision, and human deferral.
- It does not establish clinical benefit from abstention outside the benchmark design.
- It does not establish how unnecessary-abstention cost should be weighted.
- This screening does not verify the project's historical interpretation of the results.

## Methods / data / evaluation relevance

- **Methods:** Benchmark construction for abstention under medical uncertainty, per abstract; details not assessed.
- **Datasets / populations:** Repurposed medical multiple-choice datasets are described in the abstract; exact datasets not assessed.
- **Baselines / comparators:** Evaluated language models are mentioned generally; identities and configurations not assessed.
- **Evaluation metrics:** Abstention behavior and self-reported confidence/calibration are named; details not assessed.
- **Failure modes / limitations:** Overcommitment is reported in the abstract; study limitations not assessed.
- **Reproducibility / code / data availability:** Not assessed in this screening.

## Candidate programs informed

- Candidate 04:
  - **Contextualizes:** medical abstention as an existing benchmarked problem.
  - **Why:** Stream 02 used it to motivate a broader evidence-state and selective-action hypothesis; no candidate definition is changed here.

## Research-gap implications

The source is sufficient to identify one dedicated 2026 medical-abstention benchmark. It is not sufficient to infer the breadth, maturity, or saturation of the abstention field.

## Advisor / resource implications

Not assessed at screening depth.

## Publication / artifact implications

The benchmark illustrates that abstention behavior can be made an explicit evaluation object. No venue or artifact strategy is inferred from the abstract alone.

## Provenance - where this source is used

- **Discussions:** `discussions/discussion_02/2026-07-29_independent-review-and-evidence-state-thesis.md`
- **Analyses:** none
- **Candidate files:** none modified
- **Decisions:** none
- **Meeting materials:** none

## Conflicting or complementary sources

- `LIT-024` MedCite
- `LIT-025` LINS
- `LIT-002` HEG-TKG
- `LIT-004` ChronoMedKG

## Open questions prompted by this source

1. How would the benchmark's abstention setting extend to sequential actions and changing evidence?
2. What utility model would balance harmful answers against unnecessary abstention or deferral?

## Notes

This record resulted from the minimal bibliographic verification authorized for Stream 02 reconstruction. No full text or related-work search was performed.
