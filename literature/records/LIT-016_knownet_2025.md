# LIT-016 — KnowNet (mentor-lab visualization and validation system)

## Bibliographic record

- **ID:** LIT-016
- **Full citation:** to verify
- **Authors:** to verify (research mentor's lab)
- **Year:** 2025 (per stream; to verify)
- **Venue / publisher:** to verify
- **Source type:** system/tool paper (to confirm)
- **Peer-reviewed:** Unclear
- **DOI:** to verify
- **PMID:** to verify
- **arXiv / other identifier:** to verify
- **Official URL:** to verify
- **Open-access URL, if any:** to verify
- **Date added:** 2026-08-28
- **Last verified:** not verified
- **Status:** READ

## Why this source matters

This is the paper the user's own explorer tool was measured against at the 2026-05-29 meeting with the research mentor, and the comparison triggered the era's pivot: the user's conclusion that the visualization tool should be the byproduct rather than the project. It also carries one of the stream's July novelty claims.

The READ status reflects the user's own reading before the 2026-05-29 meeting (stated in the stream on 2026-07-07: the user had read it and articulated the differences from his tool). The stream itself worked from that reading and from the paper's stated future-work section, not from a fresh in-stream close read.

## What the source actually establishes

As used in the stream (each item should be re-verified against the paper before reuse):

1. It presents a system built on the same lab knowledge graph the user's tool uses (node and edge counts quoted in the stream matched the user's own numbers).
2. It validates LLM output against the knowledge graph structurally, using a three-tier validation label (support / relevant / unsure).
3. Its own future-work section proposes a tree-based exploration navigator.

## Project interpretation

**Inference (July 2026, stream 03):** the system has no bibliometric evidence-rigor weighting (study type, recency, citation structure, corroboration), so a rigor-weighted agentic layer over the same substrate remained an open contribution. This is a novelty-bearing claim resting on the user's reading plus the stream's summary; it has not been verified against the full text as a separate step.

**Inference:** because the paper's future work claims the tree-based navigator, pursuing the user's exploration-path idea risked landing inside already-claimed territory and inside the visualization framing the mentor had steered away from. This reasoning is archived in the funnel entry.

## What this source does NOT establish

- It does not establish that no rigor-weighted system exists elsewhere; the gap claim was scoped to this lab's stack and was never the product of a broad literature search.
- It does not establish anything about verification of clinical extraction (its setting is the lab's repurposing-oriented graph).

## Methods / data / evaluation relevance

- **Methods:** structural KG matching for validation of LLM output; visualization.
- **Datasets / populations:** the lab's integrated knowledge graph (LIT-021).
- **Failure modes / limitations:** as used here, the relevant boundary is the absence of bibliometric weighting (project claim, to verify).
- **Reproducibility / code / data availability:** to verify.

## Candidate programs informed

- Family 5 (biomedical KG + LLM reasoning):
  - Contextualizes.
  - Why: defines what the lab's own stack already does, which is the baseline any KG-adjacent candidate must exceed.
- Candidate 04:
  - Contextualizes.
  - Why: its structural three-tier validation is a comparison point for any evaluation-of-verification design.

## Research-gap implications

Only the narrow claim: within the lab's own stack, bibliometric rigor weighting was absent as of the user's reading. No field-level gap should be inferred from this source.

## Advisor / resource implications

The system is from the research mentor's lab; any work extending or critiquing it happens inside an existing collaboration context.

## Publication / artifact implications

None recorded beyond the strategic reasoning archived in the funnel entry.

## Provenance — where this source is used

- Discussions: `discussion_03/2026-07-13_direction-funnel-niches-to-aim1.md`
- Analyses: none yet
- Candidate files: none (definitions not frozen)
- Decisions: none

## Conflicting or complementary sources

- LIT-021: the substrate graph this system runs on.
- LIT-017: a different confidence-scoring approach (LLM-judged) the stream contrasted with bibliometric rigor.

## Open questions prompted by this source

1. Verify the bibliographic details and the "no bibliometric weighting" claim against the full text.
2. Whether the tree-based navigator was subsequently published, which would close that door explicitly.

## Notes

Registered 2026-08-28 during archival of the stream's earlier threads.
