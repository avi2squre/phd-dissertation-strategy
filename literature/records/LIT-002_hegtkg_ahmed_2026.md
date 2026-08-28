# LIT-002 — The Provenance Gap in Clinical AI: Evidence-Traceable Temporal Knowledge Graphs for Rare Disease Reasoning (HEG-TKG)

## Bibliographic record

- **ID:** LIT-002
- **Full citation:** Ahmed MS, Dusanic M, Kirschner MN, Nyoungui E, Zschüntzsch J, Galke Poech L, Röttger R. The Provenance Gap in Clinical AI: Evidence-Traceable Temporal Knowledge Graphs for Rare Disease Reasoning. arXiv:2604.17114, v2, 3 May 2026.
- **Authors:** Md Shamim Ahmed, Maja Dusanic, Moritz Nikolai Kirschner, Elisabeth Nyoungui, Jana Zschüntzsch, Lukas Galke Poech, Richard Röttger
- **Year:** 2026
- **Venue / publisher:** preprint (University of Southern Denmark; Universitätsmedizin Göttingen)
- **Source type:** preprint
- **Peer-reviewed:** No (no evidence of publication found as of 2026-08-05)
- **DOI:** none
- **PMID:** none
- **arXiv / other identifier:** arXiv:2604.17114 (v2)
- **Official URL:** https://arxiv.org/abs/2604.17114
- **Open-access URL, if any:** same
- **Date added:** 2026-08-28
- **Last verified:** 2026-08-28 (identifier and authors read from the paper's first page; claims below were checked against the paper and its supplement during 2026-08-03 to 2026-08-06, including a full re-verification pass of every table used, and not re-checked at archiving)
- **Status:** READ

## Why this source matters

Second close reading in stream 03 and the source of the "supply-before" half of the two-paper synthesis. Presented at journal club on 2026-08-06. Also the source of two evaluation-design findings that bear on Candidate 04.

## What the source actually establishes

1. Five frontier models were evaluated on 36 clinician-validated scenarios across three neuromuscular disease pairs. Without citation prompts, no model returned a clinically relevant PubMed identifier. With a single instruction to cite, models produced roughly 160 to 580 identifiers each; roughly 79 to 83 percent resolved to real papers in the wrong field and 6 to 8 percent did not exist. The strongest citation-prompted model reached 15.3 percent relevance.
2. The proposed system builds a temporal knowledge graph whose edges carry PubMed identifiers, quality tiers (GOLD, SILVER, BRONZE), and temporal anchors, and a synthesis model that copies identifiers present in its context. Its output-cited identifiers resolved at 100 percent versus 0 percent for both baselines; the paper's Provenance Gap measure roughly halved.
3. Three neurologists rated the system's verifiability significantly higher on all three raters; the temporal-precision dimension was not significant for any rater.
4. A second-order (entailment) audit found about 53 percent of claim-citation pairs directly entailed by the cited abstract, about 46 percent neutral, and about 1 percent contradicted. The measured inline citation rate was well below 100 percent.
5. Blind LLM judges rated the citation-free baseline highly on verifiability with inter-rater agreement below chance; supplied with a PubMed audit, the same judges reversed their ratings and agreement rose sharply.
6. Construction of the curated backbone was by a single annotator with no inter-annotator agreement (conceded by the authors); most retrieved evidence is in the lowest tier.
7. The retrieval baseline (guideline RAG) was given text without graph structure, identifiers, or tiers; clinicians did not rate that arm.
8. Feature coverage of the system trails the unaided model on several scenario types with overlapping confidence intervals; the feature matcher is substring-based with a high false-negative rate (conceded).
9. Local-model configurations are reported only as preliminary estimates; error-resistance to injected incorrect statements was measured on one hosted model only.
10. The pipeline is configuration-driven; adding a disease pair requires a configuration file rather than code changes. Construction cost is non-trivial (thousands of abstracts through two models plus curation).

## Project interpretation

- What is shared with LIT-001 is one level up from mechanism: both identify a class of output that parametric memory is unreliable for and route around it by sourcing that output externally. The strategies are complementary: supplying identifiers eliminates fabrication but not misattribution (item 4), which a Review-style check would target; the paper has no such check at inference. *Inference; stream 03's framing, stated as such in the presentation.*
- "Graph structure is required for traceability" does not follow from the experiment because the retrieval arm was denied identifiers (item 7). The defensible claim is that identifiers must travel with evidence to the point of synthesis. *Inference.*
- Tier labels record how a claim was found, not how established it is. *Inference from the paper's own outputs.*
- The substring matcher's false negatives (item 8) and LIT-003's linguistic-variation false negatives are the same error class in two tasks. *Inference.*

## What this source does NOT establish

- **Novelty:** it does not survey citation-aware retrieval systems; a citation-aware RAG baseline was never run.
- **Saturation:** not addressed.
- **Generalizability:** three disease pairs, 36 scenarios, three raters; local-model results preliminary.
- **Causal claims:** what drives per-pair coverage differences cannot be determined from the data (overlapping intervals, matcher false negatives).
- **Deployment readiness:** the privacy-compliant configuration is the least tested.
- **Comparative superiority:** superiority is established against baselines designed without identifiers, not against a comparable citation-aware system.

## Methods / data / evaluation relevance

- **Methods:** multi-model literature extraction; curated backbone plus literature tiers; temporal anchoring; Cypher retrieval over a property graph; synthesis with in-context identifiers.
- **Datasets / populations:** three neuromuscular disease pairs; 36 scenarios; PubMed and PMC abstracts.
- **Baselines / comparators:** unaided models; guideline RAG without identifiers.
- **Evaluation metrics:** Evidence Traceability Score, Feature Coverage, Provenance Gap, five-dimension clinician rubric, LLM-judge rubric, entailment audit.
- **Failure modes / limitations:** items 4 to 9 above; several metric-definition issues found by an independent second reader (inert correlation coefficients; a denominator mismatch requiring clamping; a degenerate case where saying nothing scores perfectly).
- **Reproducibility / code / data availability:** code repository reported; check the paper for the link and license.

## Candidate programs informed

- Candidate 04 (evaluation, verification, safety):
  - Supports / challenges / contextualizes: supports the need for external-resolver evaluation.
  - Why: items 4 and 5 show that model-based assessment of verifiability inverts the truth and that resolvable citations can still be misattributed.
- Candidate 02 (neuro-symbolic + metacognitive):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: a supply-before architecture that lacks the verify-after half; the combined system is unbuilt.
- Candidate 01 (trustworthy agentic AI):
  - Supports / challenges / contextualizes: contextualizes.
  - Why: provenance traveling with evidence to synthesis is a design requirement for agentic clinical workflows.

## Research-gap implications

Cautiously: no examined paper both supplies identifiers and verifies attachment. Whether such systems exist elsewhere is not established by this record.

## Advisor / resource implications

Enclave deployment would require the local-model configuration, which is the least tested. Building a disease-specific graph is expensive and was single-annotator here. A related question raised in the stream: whether a literature graph is needed at all when the local data are timestamped notes and codes.

## Publication / artifact implications

Contribution types suggested: evaluation methodology for verifiability (external resolution plus entailment); a supply-plus-verify system; a temporal substrate (see LIT-004). Internal strategic interpretation is kept out of this record.

## Provenance — where this source is used

- Discussions: `discussions/discussion_03/2026-08-06_hegtkg-and-two-paper-synthesis.md`; `discussions/discussion_03/2026-08-20_neurosymbolic-framing-and-advisor-sequencing.md`; `discussions/discussion_03/2026-08-20_diagnostic-state-trajectory-question.md`; `discussions/discussion_03/2026-08-22_cohort-feasibility-evidence.md`
- Analyses: none yet
- Candidate files: none yet
- Decisions: none
- Meeting materials: journal-club deck of 2026-08-06 (not in repository)

## Conflicting or complementary sources

- LIT-001: complementary (verify-after); not cited by this paper.
- LIT-004: same lead and senior authors; larger-scale temporal graph with a benchmark; positioned in the stream as the next step.
- LIT-005: named by this paper as inadequate in coverage.

## Open questions prompted by this source

1. Would a citation-aware retrieval baseline close most of the Provenance Gap without a graph?
2. What entailment rate is achievable when attachment is verified at inference?
3. How do the results change under the local-model configuration a hospital would run?

## Notes

The paper shipped with a version-mismatched self-citation, noted in the stream as an irony for a provenance paper and not as a substantive criticism.
