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
