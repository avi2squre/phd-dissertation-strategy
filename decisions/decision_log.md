# Decision Log

This file records important accepted decisions and unresolved disagreements.

---

## DEC-001 — GitHub is the canonical shared project state

**Status:** ACCEPTED

**Decision:** GitHub, rather than any individual discussion or analysis history, is the canonical source of truth for the dissertation-strategy project.

**Rationale:** Independent analysis streams may have different contexts and may otherwise diverge.

---

## DEC-002 — Advisor availability primarily functions as a feasibility filter

**Status:** ACCEPTED

**Decision:** If a candidate dissertation program has at least one strong potential IHI primary advisor and meaningful complementarity with Rui Zhang, advisor-team advantage should normally have modest ranking weight.

**Rationale:** Advisor availability is essential to feasibility, but small differences in advisor fit should not outweigh large differences in scientific, publication, career, or commercialization value.

---

## DEC-003 — Industry evidence does not establish scientific novelty

**Status:** ACCEPTED

**Decision:** Industry reports may be used to estimate market demand, workflow pain points, deployment barriers, labor-market relevance, and commercialization potential. Scientific novelty and research gaps must be established primarily from scientific literature.

---

## DEC-004 — Publication feasibility is a first-class design constraint

**Status:** ACCEPTED

**Decision:** Dissertation selection should explicitly consider publication probability, time to first paper, decomposition into multiple publishable units, citation/adoption potential, and venue fit rather than optimizing for theoretical novelty alone.

---

## DEC-005 — Preserve independent disagreement rather than forcing consensus

**Status:** ACCEPTED

**Decision:** Independent analyses should be conducted separately. Significant disagreements should be documented and investigated rather than averaged away.

---

## DEC-006 — Separate internal strategic selection from faculty-facing scientific discussion

**Status:** ACCEPTED

**Decision:** The project will maintain two evaluation layers. Internal dissertation selection may use the full strategic framework, including publication strategy, citation/adoption potential, career resilience, transferable skills, labor-market relevance, commercialization, specialized-visa portfolio value, advisor fit, and execution feasibility. Faculty-facing materials will focus on scientific significance, novelty, methodological depth, research-program coherence, feasibility, rigorous evaluation, generalizability, local expertise/resources, and unresolved scientific uncertainties.

**Rationale:** The broader strategic criteria are legitimate inputs to the user's personal dissertation decision, but they are not all useful or appropriate for an exploratory scientific discussion with research faculty. Keeping the layers separate allows faculty expertise to be used where it is most informative while preserving the broader decision objectives internally.

---

## DEC-007 — Maintain a structured literature archive with reasoning provenance

**Status:** ACCEPTED

**Decision:** Scholarly literature that materially informs dissertation brainstorming, candidate definitions, novelty claims, methodological recommendations, comparisons, or faculty-facing statements should be cataloged in `literature/`. Substantively used sources should be traceable through a provenance chain from source to extracted claim to discussion/analysis to candidate program and, when applicable, to accepted decision.

**Rationale:** The project should preserve not only conclusions and discussion history but also the scientific sources underlying those arguments. A structured literature archive makes cross-analysis more reproducible, reduces citation drift, helps distinguish source-supported findings from project inference, and allows future reviewers to reassess the evidence behind a recommendation.

**Implementation:** Use `literature/index.md` as the master registry and `literature/records/` for structured source notes. Avoid storing copyrighted full-text PDFs unless storage and redistribution are clearly permitted; normally preserve citations, stable identifiers/links, structured notes, and project-relevant claims instead.

---

## DEC-008 — Adopt OPERATING_PROTOCOL.md as the canonical process protocol

**Status:** ACCEPTED

**Decision:** `OPERATING_PROTOCOL.md` is the canonical, provider-neutral protocol governing how analysis systems allocate computation in this repository. It governs process only: it changes no scientific decision, ranking, candidate definition, scoring criterion, evidence item, literature interpretation, or provenance record. Material changes to the protocol require user approval and an explicit decision-log update.

**Rationale:** Frontier-model computation should be spent on scientific reasoning rather than on reconstructing historical context, rereading already-processed exports, or redundant orchestration. A single canonical protocol prevents each new analysis session from re-deriving working rules, while DEC-005 and the protocol's own independence rules preserve genuinely independent reasoning for consequential decisions.

---

## DEC-009 — Adopt ADVERSARIAL_FALSIFICATION_PROTOCOL.md as the canonical scientific falsification protocol

**Status:** ACCEPTED

**Decision:** `analysis/ADVERSARIAL_FALSIFICATION_PROTOCOL.md` is the canonical, provider-neutral protocol for adversarial scientific review of normalized candidate dissertation directions. It governs Candidate Evaluation Packets, evidence and citation semantics, layered search, prior-art collision classification, six kill tests, two non-kill stress tests, candidate-level falsification outcomes, multi-stream information flow, and the controlled handoff from scientific survivor selection to later strategic optimization.

Phase 1 may begin only after a common Phase 1 schema and all eight Candidate Evaluation Packets have been approved. All participating streams must evaluate the same packet version for each candidate. Strategic criteria such as compensation, employer desirability, immigration strategy, commercialization, and personal preference remain excluded from Phases 1 through 5.

**Rationale:** Independent falsification is only comparable when all streams attack the same scientific target using shared definitions, evidence rules, collision rubrics, decision thresholds, and output semantics. The protocol preserves independent reasoning while preventing differences in task interpretation, search depth, citation practice, or candidate formulation from masquerading as scientific disagreement.

**Change control:** Material changes to the protocol, Candidate Evaluation Packet semantics, phase gates, decision rules, or information-flow rules require user approval and an explicit decision-log update. Editorial clarifications that preserve meaning must remain traceable through ordinary repository history.

---

## DEC-010 — Recognizable tool-owned folders and durable workspaces

**Status:** ACCEPTED, 2026-09-12, by the user in the project conversation.

**Decision:** Rename the active analysis directories `analysis/analysis_01/`, `analysis/analysis_02/`, and `analysis/analysis_03/` to `analysis/ChatGPT_disst/`, `analysis/Codex_disst/`, and `analysis/Fable_disst/`. Keep historical stream IDs and frozen artifact contents unchanged. The exact path/content map and recovered-review source commits are recorded in `analysis/PATH_MAP.md`. Three recovered, already-public Fable reviews may be imported unchanged as archival evidence, not as accepted scientific conclusions.

For concurrent local tasks, use separate persistent worktrees derived from a verified persistent repository, with names `<Tool>_disst_<task>`. Confirm runtime and filesystem access first. Durable preservation is a completion requirement; publishing sensitive material or merging a branch requires its own authorization. Never rely solely on a session scratch directory or remembered workspace rules.

**Rationale:** The user reported an almost-incorrect cross-tool file transfer and repeated loss of temporary workspaces. Recognizable ownership and durable storage address those concrete failures.

**Amendment scope:** This supersedes numbered/provider-neutral directory-name examples and blanket local-only completion practices where they conflict with this decision. Scientific rubrics remain tool-neutral. Frozen files, source commits, old branches, historical discussion directories, and model-version attribution are not rewritten. Local Finder changes require separate execution on the user's Mac; a remote migration alone does not perform them.

---

## DEC-011 — Decision-oriented research workflow with open-ended discovery

**Status:** ACCEPTED, 2026-09-12, by the user in the project conversation following the process audit and landscape-expansion discussion.

**Decision:** Use `CURRENT_STATE.md` as the current-state entry point. Preserve the eight normalized directions while permitting additional avenues discovered independently from the user's requirements and current evidence. Do not restrict discovery to topics previously named by the user or the three tools. New avenues remain provisional until evaluated; no incumbent is removed, no newcomer is selected, and no disease or method is predetermined by this decision.

Match effort to the next decision: faculty discussion, bounded pilot, or dissertation commitment. Use compact evidence briefs, early faculty/resource input, and informative experiments. Independent first-pass judgment and evidence-based reconciliation remain; recursive procedural audits do not occur by default. Hypothesis results, research-direction viability, historical fidelity, and scientific validity must be distinguished. Scientific revisions must be explicitly versioned, not silently substituted into frozen artifacts. Training and execution fit may shape project choice but cannot alter factual or novelty findings.

**Rationale:** The earlier workflow concentrated on validating a narrow initial search space and imposed dissertation-level process on reversible meeting-preparation decisions. The user requested a broader opportunity search without discarding the work already completed.

**Relationship to DEC-008/009:** Their evidence, citation, independence, and provenance safeguards remain reference standards. DEC-011 authorizes exploratory horizon scanning and decision-oriented briefs without first completing formal Phase 1. It does not relabel those briefs as Phase 1 scans, waive formal packet approval if that mode is invoked, promote the draft packet set, alter frozen N7 or other hypotheses, or change repository visibility. Specific scientific amendments and sensitive-access decisions remain explicit later checkpoints.
