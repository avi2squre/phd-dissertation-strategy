# LIT-025 - LINS: A General Medical Q&A Framework for Enhancing the Quality and Credibility of LLM-Generated Responses

## Bibliographic record

- **ID:** LIT-025
- **Full citation:** Wang, S., Zhao, F., Bu, D., et al. (2025). LINS: A general medical Q&A framework for enhancing the quality and credibility of LLM-generated responses. *Nature Communications*, 16, 9076.
- **Authors:** Sheng Wang; Fangyuan Zhao; Dechao Bu; Yunwei Lu; Ming Gong; Hongjie Liu; Zhaohui Yang; Xiaoxi Zeng; Zhiyuan Yuan; Baoping Wan; Jingbo Sun; Yang Wu; Lianhe Zhao; Xirun Wan; Wei Huang; Tao Wang; Mengtong Xu; Jianjun Luo; Jingjia Liu; Jianjun Zheng; Wei Zhang; Kang Zhang; Hongjia Zhang; Shu Wang; RunSheng Chen; Yi Zhao
- **Year:** 2025
- **Venue / publisher:** Nature Communications / Springer Nature
- **Source type:** Journal article
- **Peer-reviewed:** Yes
- **DOI:** 10.1038/s41467-025-64142-2
- **PMID:** None identified on the official article page during targeted verification
- **arXiv / other identifier:** Nature Communications volume 16, article 9076
- **Official URL:** https://www.nature.com/articles/s41467-025-64142-2
- **Open-access URL, if any:** https://www.nature.com/articles/s41467-025-64142-2.pdf
- **Date added:** 2026-08-30
- **Last verified:** 2026-08-30 (bibliographic metadata and abstract only)
- **Status:** SCREENED

## Why this source matters

Stream 02 cited LINS in its 2026-07-29 historical critique as evidence that medical response generation using current, evidence-traceable retrieval was already an active research direction. This record identifies the article without importing its conclusions into the current project.

## What the source actually establishes

At `SCREENED` depth, the official publication metadata and abstract establish that:

1. LINS is presented as a general retrieval-augmented medical question-answering framework intended to gather current, high-quality medical knowledge and produce evidence-traceable responses.
2. The abstract reports evaluation on 15,530 objective questions and two physician-curated clinical test sets.
3. The abstract reports improvements in evidence validity, medical expertise, timeliness, and overall credibility relative to the evaluated comparison conditions.

No claim beyond the official metadata and abstract was checked during this provenance pass.

## Project interpretation

**Historical Stream 02 inference:** LINS weakened a simple novelty claim based only on retrieving current medical evidence and producing traceable responses.

This inference is preserved as provenance. It has not been independently validated through a full-text review or comprehensive comparison.

## What this source does NOT establish

- It does not establish that evidence-grounded medical agents are a saturated field.
- It does not establish longitudinal patient-state tracking or a selective controller for answering, asking, revising, preserving belief, or deferring.
- It does not establish generalizability beyond the paper's evaluated questions and clinical test sets.
- It does not establish deployment readiness or adoption.
- This screening does not verify the project's historical interpretation of the results.

## Methods / data / evaluation relevance

- **Methods:** Retrieval-augmented medical question answering with evidence-traceable output, per abstract; details not assessed.
- **Datasets / populations:** 15,530 objective questions and two physician-curated clinical test sets are reported in the abstract; composition not assessed.
- **Baselines / comparators:** Not assessed in this screening.
- **Evaluation metrics:** Evidence validity, expertise, timeliness, and credibility are named; operational definitions not assessed.
- **Failure modes / limitations:** Not assessed in this screening.
- **Reproducibility / code / data availability:** Not assessed in this screening.

## Candidate programs informed

- Candidate 04:
  - **Contextualizes:** evidence-traceable and current medical response generation as existing work.
  - **Why:** Stream 02 used it to qualify the novelty of a provenance-only direction; no candidate definition is changed here.

## Research-gap implications

The source is sufficient to identify one peer-reviewed 2025 framework addressing current, traceable medical responses. It is not sufficient to infer the overall state, saturation, or residual gap of the field.

## Advisor / resource implications

Not assessed at screening depth.

## Publication / artifact implications

The paper is a historical example of a system paired with large-scale and physician-curated evaluation. No publication or artifact recommendation is inferred from the abstract alone.

## Provenance - where this source is used

- **Discussions:** `discussions/discussion_02/2026-07-29_independent-review-and-evidence-state-thesis.md`
- **Analyses:** none
- **Candidate files:** none modified
- **Decisions:** none
- **Meeting materials:** none

## Conflicting or complementary sources

- `LIT-024` MedCite
- `LIT-002` HEG-TKG
- `LIT-004` ChronoMedKG

## Open questions prompted by this source

1. How does LINS treat contradictions, supersession, patient applicability, and belief updates over time?
2. Which parts of its reported evaluation would overlap with or leave room for evidence-state selective control?

## Notes

This record resulted from the minimal bibliographic verification authorized for Stream 02 reconstruction. No full text or related-work search was performed.
