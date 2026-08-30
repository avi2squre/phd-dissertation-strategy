# Independent Review and the Evidence-State Thesis

- **Historical date:** 2026-07-29
- **Archived:** 2026-08-30
- **Primary provenance:** Stream 02 archival PDF, exchanges 1-2
- **Nature of record:** public, redacted historical reconstruction
- **Canonical effect:** none

## Problem being considered

**User-stated requirement.** The user requested an independent review of an earlier dissertation recommendation rather than a summary or automatic endorsement. The scientific direction needed to be substantive AI/NLP methodology, feasible with available advising and data, and capable of producing independently recognized research contributions, transferable technical skills, external adoption, and strong publication artifacts.

The earlier proposal, as Stream 02 understood it at the time, had moved away from drug-repurposing as the dissertation spine and toward an evaluation-and-assurance program with three components:

- A2: evidence and provenance evaluation;
- A3: failure prediction and abstention;
- A4: federated or multilingual evaluation.

The originating A1-A4 conversation belongs to another provenance stream and is intentionally not imported here. This entry records only Stream 02's contemporaneous understanding and critique.

## Initial position

**Stream 02 strategic judgment.** The earlier pivot toward evaluation science was directionally stronger than the drug-development framing. Drug repurposing could remain an application or collaborative project, but it did not remove experimental, regulatory, capital, and clinical-development bottlenecks and therefore should not control the four-year dissertation.

The first Stream 02 recommendation was narrower than the earlier A2-A4 package:

> Build the dissertation around rigorous evaluation and selective control of evidence-traceable longitudinal clinical agents, with rare-disease phenotyping as the proving ground rather than the entire dissertation.

The provisional title was `Evaluation and Selective Control of Evidence-Traceable Longitudinal Clinical Agents`, with a proposed two-clock subtitle referring to patient time and knowledge time.

## Objection: A2, A3, and A4 did not yet form one thesis

**Stream 02 strategic judgment.** Evidence/provenance evaluation, failure prediction and abstention, and federated/multilingual evaluation were judged to be three research programs. Merely placing them in successive chapters would create a portfolio of related papers rather than one falsifiable scientific thesis.

**Historical source-supported context, not a comprehensive novelty conclusion.** The archive used several sources to argue that the individual ingredients were already active research areas:

- `LIT-024` MedCite and `LIT-025` LINS were cited as evidence that medical citation generation, evidence traceability, timeliness, and retrieval-based credibility were already being studied.
- `LIT-002` HEG-TKG and `LIT-004` ChronoMedKG were cited as evidence that claim-level provenance and temporal biomedical knowledge representations were already active.
- `LIT-026` MedQAbstain was cited as evidence that medical abstention had a dedicated benchmark.
- `LIT-001` KGARevion was treated as a useful generate-review-revise baseline, but not as clinical assurance: its verification concerned knowledge-graph plausibility rather than evidence quality, recency, or patient-record evolution.

**Qualification.** The historical language called parts of these areas “crowded.” That was a Stream 02 inference from a targeted check, not a systematic or comprehensive saturation review. `TIMER` and the unspecified conformal/decision-theoretic abstention work mentioned in the archive remain unresolved source references.

## Revised framing: two clocks and an evidence state

`LIT-004` distinguished publication time, clinical time, and contextual state. Stream 02 inferred that a different research question could be formed around what an agent should do when patient time, evidence time, and context conflict.

**Hypothesis / untested proposal.** The proposed central thesis was:

> A clinical agent is reliable only when it maintains an auditable evidence state across both an evolving patient record and an evolving biomedical evidence base; an action controller using that evidence state can reduce clinically weighted error at a fixed level of coverage better than confidence, self-consistency, retrieval-augmented generation, or knowledge-graph-verification baselines.

The proposed evidence state at time `t` contained observable, auditable information rather than hidden reasoning:

- patient facts, including negation, experiencer, anatomy, temporality, and uncertainty;
- external claims and their sources;
- source quality, validity dates, supersession, and retraction status;
- the agent's current belief or differential;
- contradictions and missing information;
- tool calls, retrieval results, state changes, and the next permitted action.

**Stream 02 recommendation.** Hidden chain-of-thought was explicitly rejected as an audit trail. The trace should consist of observable facts, citations, tool results, state updates, and actions.

## Proposed scientific program

### Aim 1: measurement framework and longitudinal benchmark

**Hypothesis / untested proposal.** Construct a dynamic evaluation framework using public cases, Phenopackets, guidelines, and controlled perturbations before relying on restricted data. Proposed perturbations included late-arriving findings, contradictions, mistaken experiencer, changing negation, ambiguous anatomy, disease-stage inconsistency, superseded guidance, retracted evidence, and evidence that was real but inapplicable to the patient.

Proposed measures included belief-update fidelity, temporal consistency, citation entailment and completeness, evidence quality/currentness, calibration, risk-coverage, unnecessary-abstention cost, action utility, and robustness to model and evidence version changes.

### Aim 2: selective action controller

**Hypothesis / untested proposal.** Build a controller choosing among:

- answer;
- retrieve more evidence;
- ask for missing information;
- preserve the prior belief;
- revise the belief;
- abstain or defer to a clinician.

The proposed methodological core combined decision theory, proper scoring rules, selective prediction or conformal methods, and asymmetric clinical costs. Comparators included direct model answers, ordinary retrieval, knowledge-graph review, structured retrieval, self-consistency, model disagreement, confidence thresholds, and learned deferral.

The key empirical question was whether explicit evidence-state features predict unsafe actions better than confidence or consistency alone.

### Aim 3: applied validation

**Stream 02 recommendation.** Rare-disease phenotyping could test clinical mention detection, negation, experiencer, anatomy, temporality, ontology normalization, and selective deferral. The general question was not whether a multi-component pipeline increased extraction F1, but whether the evidence-state controller could identify unsafe extraction, determine what information was missing, and reduce clinically weighted risk at useful coverage.

Federated or multilingual evaluation was demoted from a required chapter to an optional extension dependent on authorization, data, policy, and collaborators.

## Multi-agent qualification

**Later correction or qualification.** A suggestion to use separate components for context dimensions did not establish that multiple agents were scientifically necessary. Stream 02 recommended using a multi-agent architecture only if controlled comparisons showed improvement over a single model with tools, deterministic pipelines, retrieval, or task-specific models while remaining competitive on cost, latency, reproducibility, and failure rate.

“Agentic” was therefore framed as an experimentally justified control policy, not a branding contribution.

## Historical conclusion and unresolved questions

The July 29 conclusion was that the strongest scientific object was not provenance, abstention, or federated evaluation alone, but an explicit evidence state linked to selective action under two evolving timelines.

Unresolved questions included:

1. Whether the evidence state could be specified with construct validity and reliable annotation.
2. Whether its features added predictive value beyond confidence, consistency, retrieval, and structured-verification baselines.
3. Whether the controller improved clinically weighted outcomes rather than merely abstaining more often.
4. Whether the work was sufficiently distinct after a broader literature review.
5. Whether the rare-disease setting supplied adequate data, annotation, ownership, and generalizability.

No experiment in the archive tested the central thesis.
