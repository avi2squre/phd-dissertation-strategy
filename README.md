# PhD Dissertation Strategy Project

## Purpose

This repository is the canonical shared workspace for evaluating and developing dissertation research programs for a PhD in Health Informatics.

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

These criteria are used to decide which research directions are strategically worth pursuing and comparing.

### Layer 2 — Faculty-facing scientific evaluation

Materials prepared for research discussions with faculty should focus on the scientific research program rather than the user's private career-optimization criteria. Faculty-facing materials should emphasize:

- scientific significance
- novelty and unresolved research gaps
- methodological depth
- research questions and potential contributions
- feasibility and tractability
- available data, compute, infrastructure, and collaborators
- rigorous evaluation strategies and failure modes
- generalizability beyond a narrow application
- coherence as a multi-study dissertation program
- advisor, lab, and institutional expertise/resources
- major scientific uncertainties

Publication venues may be included when scientifically useful. Publication velocity, citation optimization, specialized-visa strategy, labor-market optimization, AI-proofing, and startup potential should remain internal unless they arise naturally as relevant scholarly or translational considerations.

## Canonical-state rule

GitHub is the source of truth.

No individual analysis stream should treat its own prior discussion history as authoritative when it conflicts with the current repository.

## Operating protocol for analysis systems

`OPERATING_PROTOCOL.md` defines how any AI analysis system should allocate its computation here: progressive context retrieval, no routine rereading of raw exports or the full repository, stream independence during first-pass analysis, compute scaled to decision consequence, and human checkpoints. Read it once at onboarding. It governs process only and changes no scientific decision, ranking, or provenance record.

## Analytical independence

Independent analyses should evaluate the evidence on their own merits.

Do not automatically converge simply because another analysis reached a particular conclusion.

Explicitly identify:

- agreements
- disagreements
- different assumptions
- uncertainty
- missing evidence

Disagreement is useful and should be preserved until resolved.

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

The project should preserve the following provenance chain whenever practical:

`source -> extracted claim -> discussion/analysis -> candidate program -> decision`

Use:

- `literature/index.md` as the master scholarly-literature registry
- `literature/records/` for structured notes on substantively used papers and articles
- `evidence/` for distilled claims used in comparisons
- `discussions/` for the reasoning history
- `analysis/` for independent synthesis and critique
- `decisions/` for accepted project state

A paper being mentioned does not automatically make it accepted evidence. Sources used for substantive claims should be checked at an appropriate depth, and novelty or field-saturation claims should not be inferred from a single paper.

Do not store copyrighted full-text PDFs in the repository unless storage/redistribution is clearly permitted. Prefer stable identifiers, official or open-access links, and structured source notes.

## Candidate-definition rule

Do not change the definition of a candidate dissertation program while ranking it.

If a materially different program is proposed, create a new candidate.

## Current research themes under investigation

- Trustworthy agentic AI
- Neuro-symbolic AI
- Artificial metacognition
- Causal agentic AI / automated real-world evidence
- AI evaluation, verification, and safety
- Biomedical knowledge graphs and LLM reasoning

These are provisional and may be added, merged, or eliminated through the decision process.
