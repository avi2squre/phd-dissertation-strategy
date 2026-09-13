# PhD Dissertation Strategy Project

> **Start here:** [`CURRENT_STATE.md`](CURRENT_STATE.md) records the active workflow, current candidate status, and next decisions. The tool-owned folders are [`analysis/ChatGPT_disst/`](analysis/ChatGPT_disst/), [`analysis/Codex_disst/`](analysis/Codex_disst/), and [`analysis/Fable_disst/`](analysis/Fable_disst/). Older numbered paths are mapped in [`analysis/PATH_MAP.md`](analysis/PATH_MAP.md). DEC-010 and DEC-011 govern the current naming and decision-oriented workflow where they amend older instructions.

## Purpose

This repository is the canonical shared workspace for evaluating and developing dissertation research directions for a PhD in Health Informatics.

Multiple independent analysis streams may contribute to the same evidence base and project state.

The project uses two distinct evaluation layers.

### Layer 1 — Internal strategic evaluation

Internal dissertation selection may consider the full set of scientific, professional, and practical objectives, including:

- scientific importance and novelty
- publication feasibility
- publication decomposition and velocity
- citation and artifact-adoption potential
- career resilience as AI capabilities improve
- transferable technical skills
- US labor-market relevance
- commercialization and startup potential
- specialized-visa research portfolio value
- advisor fit at the University of Minnesota
- complementarity with Dr. Rui Zhang
- feasibility given available data, compute, infrastructure, and time

These criteria are used to decide which research directions are strategically worth pursuing and comparing. Listing an internal criterion in this public repository does not make detailed personal strategy appropriate for publication; repository visibility and private-workspace separation are separate access-control decisions.

### Layer 2 — Faculty-facing scientific evaluation

Materials prepared for research discussions with faculty should focus on the scientific research direction rather than the user's private career-optimization criteria. Faculty-facing materials should emphasize:

- scientific significance
- novelty and unresolved research gaps
- methodological depth
- research questions and potential contributions
- feasibility and tractability
- available data, compute, infrastructure, and collaborators
- rigorous evaluation strategies and failure modes
- generalizability beyond a narrow application
- coherence as a multi-study dissertation
- advisor, lab, and institutional expertise/resources
- major scientific uncertainties

Publication venues may be included when scientifically useful. Publication velocity, citation optimization, specialized-visa strategy, labor-market optimization, AI-proofing, and startup potential should remain internal unless they arise naturally as relevant scholarly or translational considerations.

## Canonical-state rule

Accepted, versioned decisions on GitHub define the shared project state. Archived agent statements do not become scientific truth merely by being stored here. Current operative instructions are summarized in `CURRENT_STATE.md`; historical rankings and frozen drafts must not be mistaken for current approvals.

No individual analysis stream should treat its own prior discussion history as authoritative when it conflicts with the current accepted project state.

## Operating protocol for analysis systems

`OPERATING_PROTOCOL.md` defines progressive context retrieval, no routine rereading of raw exports or the full repository, stream independence, compute scaled to decision consequence, and human checkpoints. Read it at onboarding alongside `CURRENT_STATE.md`. The current decision-oriented workflow and persistent-worktree rules are adopted through DEC-010 and DEC-011; detailed historical phase templates are reference tools, not prerequisites for every exploratory discussion.

## Analytical independence

Independent analyses should evaluate the evidence on their own merits.

Do not automatically converge simply because another analysis reached a particular conclusion.

Explicitly identify agreements, disagreements, different assumptions, uncertainty, and missing evidence. Disagreement is useful and should be preserved until resolved. Independent model reviews are not independent empirical replications.

## Decision-change rule

Before changing an accepted decision:

1. Identify the existing decision.
2. Explain what new evidence or reasoning challenges it.
3. State the proposed replacement.
4. Record the change in `decisions/decision_log.md`.

Do not silently rewrite previous decisions.

## Source hierarchy

Prefer evidence roughly in this order:

1. Peer-reviewed research and primary scientific literature
2. Official university/faculty/program information
3. Government and official statistical sources
4. High-quality industry evidence
5. Commentary and opinion

Industry evidence may establish market demand or operational pain points, but it does not by itself establish scientific novelty.

## Literature archive and evidence provenance

Scientific and scholarly literature used during brainstorming and candidate development should be cataloged in `literature/`.

Preserve the provenance chain where practical:

`source -> extracted claim -> discussion/analysis -> candidate direction -> decision`

Use:

- `literature/index.md` as the master scholarly-literature registry
- `literature/records/` for structured notes on substantively used papers and articles
- `evidence/` for distilled claims used in comparisons
- `discussions/` for the reasoning history
- `analysis/` for independent synthesis and critique
- `decisions/` for accepted project state

A paper being mentioned does not automatically make it accepted evidence. Sources used for substantive claims should be checked at an appropriate depth, and novelty or field-saturation claims should not be inferred from a single paper.

Do not store copyrighted full-text PDFs unless storage/redistribution is clearly permitted. Prefer stable identifiers, official or open-access links, and structured source notes.

## Candidate-definition rule

Do not change a candidate's definition silently while comparing it. Preserve the earlier version and explicitly record a materially revised formulation. A negative hypothesis result does not automatically eliminate a broader research direction; report those judgments separately.

## Open research portfolio

The eight directions in `analysis/round3_normalization_reconciliation.md` remain the incumbent portfolio. They are not an exhaustive list, a final ranking, or a commitment to a particular disease or method.

Additional avenues may be discovered independently from the user's requirements, current research, clinical or biological bottlenecks, emerging resources, and credible translational signals. Evaluate newcomers and incumbents on comparable evidence rather than document polish, novelty of terminology, or sunk preparation effort. Do not promote a horizon-scan lead to an approved candidate merely because it was discussed.
