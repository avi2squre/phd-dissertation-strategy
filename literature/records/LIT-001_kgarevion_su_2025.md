# LIT-001 — KGARevion: An AI Agent for Knowledge-Intensive Biomedical QA

## Bibliographic record

- **ID:** LIT-001
- **Full citation:** Su X, Wang Y, Gao S, Liu X, Giunchiglia V, Clevert D-A, Zitnik M. KGARevion: An AI Agent for Knowledge-Intensive Biomedical QA. Published as a conference paper at ICLR 2025.
- **Authors:** Xiaorui Su, Yibo Wang, Shanghua Gao, Xiaolong Liu, Valentina Giunchiglia, Djork-Arné Clevert, Marinka Zitnik
- **Year:** 2025
- **Venue / publisher:** International Conference on Learning Representations (ICLR) 2025
- **Source type:** conference paper
- **Peer-reviewed:** Yes
- **DOI:** not recorded
- **PMID:** none
- **arXiv / other identifier:** arXiv:2410.04660 (v2, 3 Mar 2025)
- **Official URL:** https://arxiv.org/abs/2410.04660
- **Open-access URL, if any:** same
- **Date added:** 2026-08-28
- **Last verified:** 2026-08-28 (identifier and author list read from the paper's first page; claims below were checked against the paper during 2026-07-21 to 2026-07-23 and not re-checked at archiving)
- **Status:** READ

## Why this source matters

First close reading in stream 03 and the origin of the architectural principle the stream keeps returning to: generate freely with a model, then verify against an independent structured source. Presented at journal club on 2026-07-23.

## What the source actually establishes

1. A biomedical question-answering agent with four actions: Generate (LLM proposes candidate triplets, one per answer option in the choice-aware setting), Review (maps entities to pretrained structural embeddings of a knowledge graph, fuses them with a fixed textual relation description, and a LoRA-fine-tuned model outputs True or False), Revise (swaps head or tail of a False triplet and resubmits, up to k rounds), Answer (reasons over the verified set only).
2. Review is fine-tuned once, offline, on triplet-completion data from the graph; structural embeddings are kept fixed; relation descriptions come from a fixed template table; no online learning at inference.
3. Entities absent from the graph are retained as "incomplete knowledge" rather than rejected.
4. Ablations: removing Review costs about nine accuracy points on multiple-choice benchmarks and about four on open-ended ones, averaged across seven datasets; removing Revise costs about three points on the MedDDx family; the number of Revise rounds that works best varies by model and dataset.
5. Option reordering moves raw LLM accuracy by roughly 8 to 16 points and the agent by roughly 1.5 to 4.
6. Replacing the underlying graph (PrimeKG, LIT-005, with OGB-biokg) changes accuracy from 0.69 to 0.67.
7. Open-ended questions are scored by a stated formula rather than by exact match; the agent's open-ended results are weaker than its multiple-choice results.

## Project interpretation

- Review is a pure function of (head, relation, tail): every input is deterministic, so the same triplet always receives the same verdict, and Revise cannot rescue a Review false negative. *Inference from items 2 and 1; traced in `discussions/discussion_03/2026-07-23_kgarevion-verification-analysis.md`.*
- The transferable idea is the architecture, not the component. Because the graph is used to verify rather than to retrieve, the method is not welded to a particular graph (item 6). *Inference.*
- Review does more than a database lookup: it scores triplets that are not literal edges using structural position. *Inference from the mechanism; illustrated on a toy example, not measured.*
- Revise's measured benefit has no mechanism the paper supplies or the stream could defend. Four proposed mechanisms failed. *Inference; recorded as unresolved.*

## What this source does NOT establish

- **Novelty:** it is one verification architecture; it does not establish that verify-after is the best strategy or that the design space is unexplored.
- **Saturation:** nothing about how many similar systems exist.
- **Generalizability:** results are on biomedical QA benchmarks with a fixed graph; no clinical-note or extraction setting.
- **Causal claims:** the ablations are averages; gold-standard and MedDDx subsets move in opposite directions, so per-dataset conclusions are not supported by the headline numbers.
- **Deployment readiness:** none claimed; the soft-constraint handling of unmappable entities is a safety gap for any entity the graph has not seen.
- **Comparative superiority:** compared against raw LLMs and prompting baselines, not against other verification designs.

## Methods / data / evaluation relevance

- **Methods:** LLM generation; knowledge-graph embedding (TransE-style) alignment with LLM via attention and feed-forward fusion; LoRA fine-tuning for a True/False head; iterative revision.
- **Datasets / populations:** seven biomedical QA benchmarks including gold-standard sets and the MedDDx family (basic, intermediate, expert), multiple-choice and open-ended forms.
- **Baselines / comparators:** raw LLMs, prompting strategies, ablated variants.
- **Evaluation metrics:** accuracy; a stated scoring formula for open-ended answers; robustness to option reordering.
- **Failure modes / limitations:** unmappable entities pass unverified; hierarchy is poorly handled by translation-style embeddings, which matters for ontologies where parent-child is the relation of interest; Revise unexplained.
- **Reproducibility / code / data availability:** not recorded in the stream; check the paper.

## Candidate programs informed

- Candidate 02 (neuro-symbolic + metacognitive):
  - Supports / challenges / contextualizes: contextualizes (concrete instance) and cautions (adding a verifier is not sufficient; the verifier has holes).
  - Why: it is neural generation plus symbolic verification with measured effects and identified gaps.
- Candidate 04 (evaluation, verification, safety):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: the reordering result is a reliability measurement, and determinism of the verifier is an exploitable property for evaluation.
- Family 5 (biomedical KG + LLM reasoning):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: graph as verification substrate rather than retrieval source.

## Research-gap implications

Cautiously: the paper leaves its own Revise component unexplained and handles unmappable entities permissively. Whether either is an open problem in the field is not established by this one source.

## Advisor / resource implications

Reproducing the method requires a knowledge graph with pretrained structural embeddings, a fine-tuning run, and GPU access; the stream did not attempt it. The July proposal would additionally need a disease-phenotype graph aligned to the Human Phenotype Ontology (LIT-006, LIT-007).

## Publication / artifact implications

Contribution types this suggests: a verification component with an evaluation of what verification buys; a reliability benchmark (reordering, distractor similarity). Internal strategic interpretation is kept out of this record.

## Provenance — where this source is used

- Discussions: `discussions/discussion_03/2026-07-23_kgarevion-verification-analysis.md`; `discussions/discussion_03/2026-07-23_rare-phenix-verification-proposal.md`; `discussions/discussion_03/2026-08-06_hegtkg-and-two-paper-synthesis.md`; `discussions/discussion_03/2026-08-20_neurosymbolic-framing-and-advisor-sequencing.md`
- Analyses: none yet
- Candidate files: none yet
- Decisions: none
- Meeting materials: journal-club deck of 2026-07-23 (not in repository)

## Conflicting or complementary sources

- LIT-002: complementary; opposite strategy for the same diagnosis (supply-before versus verify-after). Does not cite LIT-001.
- LIT-003: the pipeline the stream proposes to combine with this verifier.
- LIT-005: the graph used; named inadequate by LIT-002 and LIT-004 on different grounds.

## Open questions prompted by this source

1. What mechanism, if any, explains Revise's benefit on the hardest distractor set?
2. How should unmappable entities be handled so that verification degrades visibly rather than silently?
3. Does a verifier built on translation-style embeddings transfer to an ontology whose key relation is hierarchical?

## Notes

The paper never expands the name; the stream's guess that it fuses "Review" and "Revision" is speculation. The word "agent" is used in the singular throughout the paper.
