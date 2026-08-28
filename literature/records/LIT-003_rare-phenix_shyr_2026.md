# LIT-003 — RARE-PHENIX: An artificial intelligence framework for end-to-end rare disease phenotyping from clinical notes using large language models

## Bibliographic record

- **ID:** LIT-003
- **Full citation:** Shyr C, et al. An artificial intelligence framework for end-to-end rare disease phenotyping from clinical notes using large language models (RARE-PHENIX). arXiv:2602.20324, 2026.
- **Authors:** Shyr C and co-authors (full author list to be recorded from the paper; Vanderbilt and Yale affiliations per the stream's reading)
- **Year:** 2026
- **Venue / publisher:** preprint
- **Source type:** preprint
- **Peer-reviewed:** Unclear (not checked since 2026-07-22)
- **DOI:** none recorded
- **PMID:** none recorded
- **arXiv / other identifier:** arXiv:2602.20324
- **Official URL:** https://arxiv.org/abs/2602.20324
- **Open-access URL, if any:** same
- **Date added:** 2026-08-28
- **Last verified:** 2026-08-28 (identifier as recorded in the stream; the full text was read from the arXiv HTML version on 2026-07-22 and the false-negative analysis re-verified against the text on 2026-08-06)
- **Status:** READ

## Why this source matters

The reference pipeline for the CIL-FLARE project's phenotyping aim, shared by the clinical collaborator. The stream's July proposal targets its standardization step. Its error analysis is the empirical basis for the granularity argument.

## What the source actually establishes

1. A three-module pipeline: (1) extraction of free-text phenotype mentions by a fine-tuned LLM (several open models and a hosted model were tried, with instruction fine-tuning or few-shot prompting, trained on a rare-disease corpus and synthetic narratives); (2) standardization by retrieval-augmented generation, embedding each extracted string, retrieving the ten nearest Human Phenotype Ontology terms, and having an LLM choose one (or none); (3) prioritization by a supervised learning-to-rank model (gradient-boosted) over the patient's terms using informativeness features derived from disease-phenotype annotation resources, taking the top k.
2. Developed on an undiagnosed-disease cohort of several thousand patients and externally tested on an independent institutional cohort of patients and their notes; reported to outperform a fine-tuned transformer baseline (LIT-009) on an ontology-similarity measure (0.70 versus 0.58).
3. Error analysis: false positives arise primarily from ontology granularity (a parent term chosen over a more specific child). Manual review of false negatives found that the large majority (97 percent of reviewed instances) were not extraction failures but arose from how phenotypes are documented; in several cases the model extracted a semantically related or higher-level concept.
4. Each module improves performance when added sequentially. The authors acknowledge limitations around gold-standard curation and the need for prospective validation.

## Project interpretation

- Module 2 makes an irreversible commitment judged only by the model that made it; Module 3 cannot repair it because it only reorders terms that exist. *Inference from the architecture.*
- A granularity error yields a false positive and a false negative simultaneously, so fixing granularity would improve precision and recall together. *Inference from item 3.*
- The false negatives attributed to documentation style are partly candidates that were produced at the wrong level (item 3), which is what a verification step could act on; and partly surface-form mismatches where the right term never entered the retrieved pool, which no downstream step can recover. The paper does not split these. *Inference; the split is unknown.*
- Because ground truth in this setting is a phenotype list rather than a disease label, the pipeline never needs the diagnosis, which is why inserting a disease-anchored verifier creates the anchor problem. *Inference.*

## What this source does NOT establish

- **Novelty:** end-to-end framing is the authors' claim; the record does not survey competing pipelines.
- **Saturation:** not addressed.
- **Generalizability:** two cohorts; one external test site.
- **Causal claims:** the sequential-improvement result is an ablation, not a mechanism.
- **Deployment readiness:** hosted-model components would not run inside a data enclave.
- **Comparative superiority:** compared against one fine-tuned baseline on one similarity measure.

## Methods / data / evaluation relevance

- **Methods:** LLM fine-tuning for span extraction; embedding retrieval over an ontology; LLM selection; learning-to-rank.
- **Datasets / populations:** undiagnosed-disease network patients; an institutional cohort with clinical notes.
- **Baselines / comparators:** a fine-tuned transformer phenotype recognizer (LIT-009); ablations of each module.
- **Evaluation metrics:** ontology-similarity score; precision and recall against curated phenotype lists; top-k curves.
- **Failure modes / limitations:** granularity; linguistic variation in documentation; irreversible standardization; hosted components.
- **Reproducibility / code / data availability:** not recorded in the stream; check the paper.

## Candidate programs informed

- Candidate 02 (neuro-symbolic + metacognitive):
  - Supports / challenges / contextualizes: contextualizes and supplies the concrete gap.
  - Why: the ontology mapping is the symbolic half; the unverified commitment is where symbolic verification would be inserted.
- Candidate 04 (evaluation, verification, safety):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: the paper's own error analysis is an example of the evaluation that tells you where verification could help.

## Research-gap implications

Cautiously: the paper identifies granularity as its dominant error and leaves the standardization step self-judged. Whether verification-in-the-loop for ontology mapping is unexplored elsewhere is not established by this record.

## Advisor / resource implications

The CIL-FLARE setting requires running extraction on notes inside an enclave with local models only; the hosted components of this pipeline would need substitutes. Ground-truth phenotype lists require clinician curation.

## Publication / artifact implications

Contribution types suggested: a verified standardization step with an ablation showing precision and recall moving together; an error taxonomy separating surface-form from granularity failures. Internal strategic interpretation is kept out of this record.

## Provenance — where this source is used

- Discussions: `discussions/discussion_03/2026-07-23_rare-phenix-verification-proposal.md`; `discussions/discussion_03/2026-08-06_hegtkg-and-two-paper-synthesis.md`; `discussions/discussion_03/2026-08-20_neurosymbolic-framing-and-advisor-sequencing.md`; `discussions/discussion_03/2026-08-20_diagnostic-state-trajectory-question.md`; `discussions/discussion_03/2026-08-22_cohort-feasibility-evidence.md`
- Analyses: none yet
- Candidate files: none yet
- Decisions: none
- Meeting materials: journal-club decks of 2026-07-23 and 2026-08-06 (not in repository)

## Conflicting or complementary sources

- LIT-001: the verifier the stream proposes to insert.
- LIT-006, LIT-007: the ontology being mapped to.
- LIT-009, LIT-013: extraction tools compared against or considered as local substitutes.

## Open questions prompted by this source

1. What fraction of the reported false negatives are recoverable (correct term in the retrieved pool, wrong level chosen) versus unrecoverable (correct term never retrieved)?
2. Does verifying candidates against a disease class before selection improve precision and recall together, as the granularity argument predicts?

## Notes

The stream initially misattributed the 97 percent false-negative finding to extraction; corrected on re-reading the paper's text. The correction is archived in the proposal entry.
