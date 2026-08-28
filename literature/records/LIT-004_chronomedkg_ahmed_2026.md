# LIT-004 — ChronoMedKG: A Temporally-Grounded Biomedical Knowledge Graph and Benchmark for Clinical Reasoning

## Bibliographic record

- **ID:** LIT-004
- **Full citation:** Ahmed MS, Firoozbakht F, Galke Poech L, Baumbach J, Röttger R. ChronoMedKG: A Temporally-Grounded Biomedical Knowledge Graph and Benchmark for Clinical Reasoning. arXiv:2605.22734, v1, 21 May 2026.
- **Authors:** Md Shamim Ahmed, Farzaneh Firoozbakht, Lukas Galke Poech, Jan Baumbach, Richard Röttger
- **Year:** 2026
- **Venue / publisher:** preprint (University of Southern Denmark; University of Hamburg); formatted as a datasets-and-benchmarks submission
- **Source type:** preprint; dataset and benchmark paper
- **Peer-reviewed:** No (as of the stream's reading)
- **DOI:** dataset DOI 10.5281/zenodo.19697542 (paper itself has no DOI recorded)
- **PMID:** none
- **arXiv / other identifier:** arXiv:2605.22734 (v1); code: https://gitlab.sdu.dk/screen4care/chronomedkg
- **Official URL:** https://arxiv.org/abs/2605.22734
- **Open-access URL, if any:** same; dataset on Zenodo
- **Date added:** 2026-08-28
- **Last verified:** 2026-08-28 (identifiers, authors, and abstract read from the paper's first page; content examined on 2026-08-05 for comparison with LIT-002)
- **Status:** READ

## Why this source matters

Read when deciding which paper to present on 2026-08-06. Not presented, but it changed the stream's assessment of LIT-002's scale and pointed at the temporal dimension the clinical collaborator had identified as critical for context identification.

## What the source actually establishes

1. A temporal biomedical knowledge graph of 460,497 evidence-linked triples, filtered from about 13 million raw extractions, covering 13,431 diseases; each association carries temporal components (onset window or progression stage), PubMed-traceable evidence, and a multi-signal credibility score.
2. Construction by a disease-autonomous multi-agent pipeline in which multiple frontier LLMs independently extract from PubMed and PMC; relations are kept only if supported by multi-model consensus, credibility filtering, and ontology alignment.
3. Reported 92.7 percent agreement against Orphadata; temporal grounding added for 6,250 diseases absent from HPOA, Orphadata, and Phenopackets, including 1,657 Orphanet-coded rare diseases.
4. ChronoTQA benchmark: 3,341 questions across eight task types (six temporal, two static controls) plus a 12-question probe. Frontier LLMs lose roughly 30 points from static to temporal questions; retrieval from the graph rescues 47 to 65 percent of long-tail failures versus 17 to 29 percent for retrieval from HPOA.
5. The paper names PrimeKG, Hetionet, and iKraph as lacking the temporal dimension; HPOA provides only coarse onset categories.
6. Dataset and code are public (Zenodo DOI, GitLab).

## Project interpretation

- Choosing fresh, this is the methodologically stronger paper for the temporal question (scale, external validation, public benchmark), while LIT-002 has the more striking single result. *Inference; stream's assessment.*
- Together with LIT-002, this paper's framing that existing graphs are inadequate connects to the July finding that verification is only as good as the underlying graph. *Inference.*
- Multi-model consensus as a construction filter is the transferable mechanism: two models must independently agree before a relation is kept. *Inference; the stream initially drew this as discarding disagreements and corrected it on reading the construction pseudocode, which keeps and labels rather than discards.*

## What this source does NOT establish

- **Novelty:** not surveyed here beyond the paper's own comparison table.
- **Saturation:** not addressed.
- **Generalizability:** clinician validation was at a small (six-disease) scale per the stream's reading; the residual error rate after consensus is about 7 percent; the credibility score is only partially populated; one retrieval tier never triggered in practice.
- **Causal claims:** none made.
- **Deployment readiness:** the graph is a resource, not a clinical system.
- **Comparative superiority:** link-prediction comparisons are affected by the larger entity space.

## Methods / data / evaluation relevance

- **Methods:** multi-agent literature extraction; consensus filtering; credibility scoring; ontology alignment; retrieval augmentation; benchmark construction.
- **Datasets / populations:** PubMed and PMC literature; 13,431 diseases; ChronoTQA.
- **Baselines / comparators:** HPOA-based retrieval; unaided frontier models.
- **Evaluation metrics:** agreement with Orphadata; benchmark accuracy by task type; rescue rate on long-tail failures.
- **Failure modes / limitations:** residual incorrect entries; partial credibility population; small-scale clinician validation.
- **Reproducibility / code / data availability:** public dataset and code.

## Candidate programs informed

- Family 5 (biomedical KG + LLM reasoning):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: a large public temporal substrate reduces the "build your own graph" cost that LIT-002 illustrates.
- Candidate 02:
  - Supports / challenges / contextualizes: contextualizes.
  - Why: a temporal symbolic substrate for verification of time-anchored claims.
- Candidate 04:
  - Supports / challenges / contextualizes: contextualizes.
  - Why: the static-to-temporal accuracy drop is an evaluation finding; the benchmark is reusable.

## Research-gap implications

Cautiously: the paper documents that temporal grounding is missing from major graphs and supplies it at scale. Any gap claim about temporal verification of clinical output must account for this resource existing.

## Advisor / resource implications

Public artifacts lower infrastructure cost. Using the graph inside an enclave would require importing it through the governed transfer process.

## Publication / artifact implications

An example of a datasets-and-benchmarks contribution type with public DOI and code, which is a reusable-artifact pattern. Internal strategic interpretation is kept out of this record.

## Provenance — where this source is used

- Discussions: `discussions/discussion_03/2026-08-06_hegtkg-and-two-paper-synthesis.md`
- Analyses: none yet
- Candidate files: none yet
- Decisions: none
- Meeting materials: mentioned in the 2026-08-06 deck's closing as a next step (not in repository)

## Conflicting or complementary sources

- LIT-002: same lead and senior authors; provenance-focused predecessor.
- LIT-005: named inadequate for lacking temporality.
- LIT-006, LIT-007: the ontology's annotation resource (HPOA) is the comparison baseline.

## Open questions prompted by this source

1. Can the graph serve as the verification substrate for time-anchored claims extracted from clinical notes, rather than as a retrieval source for question answering?
2. How much of the residual error concentrates in rare diseases, where the project's use would be?

## Notes

Read for comparison; the decision to keep presenting LIT-002 was made on commitment and timeline grounds, not on quality grounds. That reasoning is archived in the synthesis entry.
