# LIT-021 — ADInt knowledge graph (mentor lab)

## Bibliographic record

- **ID:** LIT-021
- **Full citation:** to verify
- **Authors:** to verify (research mentor's lab)
- **Year:** 2024
- **Venue / publisher:** Scientific Reports (per stream; to verify)
- **Source type:** journal article (resource/method)
- **Peer-reviewed:** Yes (assuming venue confirms)
- **DOI / PMID:** to verify
- **Official URL:** to verify
- **Date added:** 2026-08-28
- **Last verified:** not verified
- **Status:** READ

## Why this source matters

This is the substrate of the user's own demonstrated work: the explorer tool the user built (graph browsing, shortest-path finding, evidence panel with literature identifiers) runs on this knowledge graph, and the early-era and June-July direction reasoning treated it as the user's built-in differentiator and lab entry point. Any candidate that extends the lab's KG stack starts here.

## What the source actually establishes

As used in the stream (re-verify before reuse):

1. An integrated biomedical knowledge graph built for the lab's dietary-supplement and Alzheimer's-related drug-repurposing work, published with link-prediction results.
2. Scale on the order of 162 thousand nodes and 1.0 million edges. Two slightly different node/edge counts appear at different points in the stream; the discrepancy is unresolved and the paper's own figures should be taken as canonical when checked.
3. The published paper has no interactive visualization component (the basis of the user's tool-as-entry-point plan in the early era).

## Project interpretation

**Inference:** the graph carries literature-linked provenance suitable for evidence-rigor work, which is why the July delta (bibliometric rigor weighting) was framed over it. Whether its provenance fields are sufficient for study-type and citation-structure weighting was never checked and is a feasibility question for any such design.

## What this source does NOT establish

- It does not establish the quality or coverage of its provenance annotations for rigor weighting.
- It does not establish anything about rare-disease phenotyping; its domain is supplements and neurodegeneration-adjacent repurposing.

## Methods / data / evaluation relevance

- **Datasets / populations:** literature-derived biomedical entities and relations (details to verify).
- **Reproducibility / code / data availability:** the graph was available to the user for tool-building; formal availability to verify.

## Candidate programs informed

- Family 5 (biomedical KG + LLM reasoning):
  - Supports (as infrastructure).
  - Why: an in-hand, lab-owned substrate for any KG-verification or KG-reasoning candidate, plus the user's demonstrated engineering work on it.

## Research-gap implications

None directly; it is infrastructure and context, not a gap source.

## Advisor / resource implications

Owned by the research mentor's lab; work on it is inherently collaborative with the lab.

## Publication / artifact implications

The user's explorer tool over this graph is an existing artifact; the early era planned it as a citable software contribution, which remains unexecuted as a publication.

## Provenance — where this source is used

- Discussions: `discussion_03/2026-04-11_early-direction-era-and-advisor-search.md`, `discussion_03/2026-07-13_direction-funnel-niches-to-aim1.md`

## Conflicting or complementary sources

- LIT-016: the lab system that validates LLM output against this graph.
- LIT-005: the general-purpose graph LIT-001 verifies against; different graph, different role.

## Open questions prompted by this source

1. Reconcile the node/edge counts against the paper.
2. Assess whether its provenance fields support bibliometric rigor weighting.

## Notes

Registered 2026-08-28 during archival of the stream's earlier threads.
