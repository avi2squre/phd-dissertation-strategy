# Phase 1 Fatal-Risk Scan Schema

- **Version:** Draft 0.1
- **Date:** 2026-09-01
- **Status:** **DRAFT — USER REVIEW REQUIRED**
- **Governing protocol:** [`analysis/ADVERSARIAL_FALSIFICATION_PROTOCOL.md`](../ADVERSARIAL_FALSIFICATION_PROTOCOL.md)
- **Purpose:** standardize the common target, minimum search coverage, evidence reporting, and output structure for the three independent Phase 1 fatal-risk scans

This schema defines the exact structure every analysis stream must use during Phase 1. It does not prescribe conclusions. All definitions, decision rules, source hierarchies, collision semantics, kill tests, stress tests, and information-flow rules come from the governing protocol and must not be redefined locally.

Phase 1 asks:

> What could kill each of the eight normalized candidate dissertation directions?

Phase 1 is a broad, independent fatal-risk scan. It is not a final novelty determination, deep systematic review, candidate ranking, or strategic comparison.

---

# Part I — Common Candidate Evaluation Packet template

Before any stream begins Phase 1, all eight candidates must have one approved Candidate Evaluation Packet. Every stream must evaluate the identical packet version.

Recommended location:

```text
analysis/candidate_packets/
    N1_candidate_evaluation_packet.md
    N2_candidate_evaluation_packet.md
    N3_candidate_evaluation_packet.md
    N4a_candidate_evaluation_packet.md
    N4b_candidate_evaluation_packet.md
    N5_candidate_evaluation_packet.md
    N6_candidate_evaluation_packet.md
    N7_candidate_evaluation_packet.md
```

Each packet must use the following structure.

## Packet metadata

- **Candidate identifier:**
- **Candidate title:**
- **Packet version:**
- **Packet status:** `APPROVED — COMMON PHASE 1 TARGET`
- **Repository commit:**
- **Date approved:**
- **Source normalization artifact:** `analysis/round3_normalization_reconciliation.md`
- **Constituent Day 1 artifacts and sections:**
- **Approval record:**

## 1. Central scientific object

State the principal representation, controller, algorithm, contract, inference framework, evaluation instrument, or other methodological object under evaluation.

This must be specific enough that a reviewer can distinguish the candidate from a broad research family.

## 2. Exact falsifiable thesis

State one central dissertation-level claim that can be supported, weakened, or defeated.

The thesis must identify:

- the proposed object or mechanism;
- the meaningful comparator;
- the target outcome;
- the conditions or domain in which the claim is expected to hold.

## 3. Included scientific scope

List the claims, mechanisms, task settings, and validation domains that belong to the candidate as evaluated in Phase 1.

## 4. Explicitly excluded scientific scope

List nearby ideas that do not belong to the candidate and must not be silently added to make it easier to defend or attack.

For merged Day 1 candidates, distinguish:

- mandatory shared core;
- competing formulations to compare;
- optional validation domains;
- constituent claims deliberately excluded from the common target.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|

Use relationship language such as:

- common core;
- competing mechanism;
- complementary mechanism;
- scoped specialization;
- validation instantiation;
- excluded adjacent thesis.

## 6. Provisional coherent aims

Normally provide two or three aims.

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|

The aims are provisional targets for coherence testing. A Phase 1 reviewer may identify incoherence but may not silently replace them.

## 7. Decisive or discriminating experiment

State the comparison most directly capable of distinguishing the thesis from a serious alternative explanation or simpler baseline.

Include:

- experimental or analytical unit;
- strongest comparator;
- primary thesis-relevant outcome;
- result pattern that supports the thesis;
- result pattern that defeats or materially weakens it.

## 8. Inherited dangerous prior art

List the prior work already identified as most likely to collide with the candidate.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|

This list is a required starting point, not a closed search universe.

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|

## 10. Feasibility assumptions inherited from Day 1

List only assumptions necessary to understand the candidate target. Phase 1 independently evaluates them under Kill Test 5.

## 11. Packet provenance and change control

Record:

- exact source artifacts;
- repository commit identifiers;
- which statements are direct compressions versus reconciled formulations;
- unresolved candidate-definition tensions;
- user approval date.

A packet may not be materially changed after Phase 1 begins. A material packet change requires:

1. stopping all affected scans;
2. user approval;
3. a new packet version;
4. explicit assessment of whether completed scans remain comparable.

---

# Part II — Required Phase 1 artifact structure

Each analysis stream creates exactly one Phase 1 artifact containing all eight candidate scans.

Recommended paths:

```text
analysis/analysis_01/phase1_fatal_risk_scan.md
analysis/analysis_02/phase1_fatal_risk_scan.md
analysis/analysis_03/phase1_fatal_risk_scan.md
```

Required frozen status:

**FROZEN — PHASE 1 INDEPENDENT FATAL-RISK SCAN**

---

# Layer I — Execution contract and executive navigation

## A. Execution contract

Record before substantive execution:

- **Date:**
- **Analysis-stream identifier:**
- **Branch:**
- **Base repository commit:**
- **Governing protocol version:**
- **Phase 1 schema version:**
- **Candidate Evaluation Packet versions:**
- **Objective:**
- **Repository files permitted:**
- **Repository files deliberately excluded:**
- **Other-stream Phase 1 outputs prohibited:** yes
- **External research:** allowed
- **External source classes permitted:**
- **Parallelism used:** yes/no
- **Parallelism justification:**
- **Expected artifact:**
- **Stopping condition:**

The base must contain the approved protocol, schema, and packets.

## B. Independence and contamination declarations

State explicitly:

1. whether any other stream's Phase 1 output was seen;
2. whether any accidental exposure occurred;
3. whether exposure preceded or followed the independent judgment;
4. whether strategic criteria influenced any scientific judgment;
5. whether the scientific verdict would change if every candidate had equal career, immigration, commercial, and prestige value.

## C. Candidate overview dashboard

This table is a navigation surface, not a ranking.

| Candidate | Packet version | Phase 1 outcome | Outcome confidence | Most severe weakness | Severity | Most decision-relevant unresolved question | Early stop? |
|---|---|---|---|---|---|---|---|
| N1 | | | | | | | |
| N2 | | | | | | | |
| N3 | | | | | | | |
| N4a | | | | | | | |
| N4b | | | | | | | |
| N5 | | | | | | | |
| N6 | | | | | | | |
| N7 | | | | | | | |

Allowed candidate outcomes:

- `SURVIVES`
- `SURVIVES WITH MATERIAL REVISION`
- `UNRESOLVED`
- `FAILS AS CURRENTLY FORMULATED`

A Phase 1 `SURVIVES` outcome means only that no fatal failure was identified at Phase 1 minimum-adequacy depth. It is not a final novelty or finalist judgment.

## D. Source and search summary

| Candidate | Search layers attempted | Hits screened | Sources inspected beyond abstract | Potentially fatal collisions | Confirmed fatal collisions | Search-coverage limitation |
|---|---:|---:|---:|---:|---:|---|

Counts are descriptive audit information, not quality scores.

---

# Layer II — Candidate-by-candidate fatal-risk scans

Repeat the following complete structure for N1, N2, N3, N4a, N4b, N5, N6, and N7 in that order.

# Candidate [ID] — [Approved packet title]

## 1. Candidate target and packet fidelity

### 1.1 Packet fingerprint

- **Candidate identifier:**
- **Packet path:**
- **Packet version:**
- **Packet repository commit:**
- **Central scientific object copied from packet:**
- **Exact falsifiable thesis copied from packet:**

### 1.2 Scope fidelity declaration

State whether the reviewer evaluated the packet without silently broadening or narrowing it.

Choose one:

- `PACKET ACCEPTED AS EVALUATION TARGET`
- `CANDIDATE-DEFINITION DISAGREEMENT`

If disagreement exists, state:

- disputed packet clause;
- reviewer's interpretation;
- why it materially affects falsification;
- whether the packet was nevertheless evaluated as written;
- next action required in Phase 2.

The reviewer must still evaluate the approved packet unless doing so is logically impossible.

### 1.3 Steelmanned scientific case

In no more than one substantive paragraph, state the strongest coherent version of the packet's scientific case without adding a new thesis.

## 2. Search concept map

| Component | Packet-derived concept | Synonyms or alternate terminology | Likely parent disciplines | Search risk if omitted |
|---|---|---|---|---|
| Scientific object | | | | |
| Mechanism | | | | |
| Target failure | | | | |
| Falsifiable thesis | | | | |
| Decisive experiment | | | | |
| Evaluation | | | | |
| Domain-specific structure | | | | |

## 3. Search audit trail

Complete one row for every applicable search layer.

| Search layer | Query families or concepts | Databases, proceedings, or sources | Hits screened | Sources inspected beyond abstract | New collision class found? | Omitted scope and rationale |
|---|---|---|---:|---:|---|---|
| 1. Exact formulation | | | | | | |
| 2. Conceptual synonyms | | | | | | |
| 3. Method-centric | | | | | | |
| 4. Adjacent biomedical | | | | | | |
| 5. Parent discipline | | | | | | |
| 6. Older/foundational | | | | | | |
| Citation-chain expansion | | | | | | |

### 3.1 Phase 1 minimum-adequacy checklist

Mark each item `COMPLETE`, `INCOMPLETE`, or `NOT APPLICABLE`, with a brief explanation.

| Requirement | Status | Evidence/location |
|---|---|---|
| Search concept map completed | | |
| Every applicable search layer attempted | | |
| Inherited dangerous prior art inspected | | |
| Newly surfaced direct threats screened | | |
| Most consequential accessible threat inspected at relevant-section depth | | |
| Six kill tests assessed or early stop justified | | |
| Two stress tests assessed or early stop justified | | |
| Cheapest discriminating test specified | | |
| Concrete next-evidence request specified | | |

### 3.2 Saturation statement

Choose one:

- `PHASE 1 ADEQUACY REACHED — DEEP SATURATION NOT CLAIMED`
- `PHASE 1 ADEQUACY NOT REACHED`
- `DEEP SATURATION REACHED FOR A SPECIFIED SUBQUESTION`

State which unsaturated search areas could plausibly conceal a fatal result. Do not make a field-wide absence claim.

## 4. Local source registry

Use existing permanent `LIT-###` identifiers where available. Assign newly discovered sources stream-local provisional identifiers using the required pattern.

| Source ID | Full citation | Stable identifier/link | Source tier | Version/access date | Inspection depth | Citation role(s) | Candidate sections used |
|---|---|---|---|---|---|---|---|

Inspection-depth values:

1. metadata only;
2. title/abstract screened;
3. relevant sections inspected;
4. full text inspected;
5. reproduced or independently validated.

## 5. Prior-art relevance screening

Record significant screened sources, including serious threats and instructive non-collisions.

| Source ID | Thesis-defining component addressed | Relevance decision | Rationale | Advance to overlap matrix? |
|---|---|---|---|---|

Allowed relevance decisions:

- `OUT-OF-SCOPE HIT`
- `NON-COLLIDING RELATED WORK`
- `ADVANCE TO COLLISION ASSESSMENT`
- `UNRESOLVED RELEVANCE`

Do not use the phrase “irrelevant collision.”

## 6. Contribution-overlap assessment

Create a separate matrix for every source classified as a serious collision threat.

### Source [ID] — [Short title]

| Dimension | None | Partial | Strong | Near-identical | Evidence and point-of-use citation |
|---|---:|---:|---:|---:|---|
| Falsifiable thesis | | | | | |
| Central scientific object | | | | | |
| Formal representation | | | | | |
| Method or learning objective | | | | | |
| Decision or output behavior | | | | | |
| Decisive experiment | | | | | |
| Evaluation methodology | | | | | |
| Domain or dataset | | | | | |

Then record:

- **Collision disposition:**
- **Disposition rationale:**
- **Inspection-depth sufficiency:**
- **Remaining contradictory evidence:**
- **Effect on the packet's novelty claim:**

Allowed dispositions:

- `NON-COLLIDING RELATED WORK`
- `PARTIAL COLLISION`
- `MAJOR COLLISION`
- `POTENTIALLY FATAL COLLISION`
- `FATAL COLLISION CONFIRMED`
- `UNRESOLVED COLLISION`

Dimension-level ratings must not be mechanically summed.

## 7. Kill-test dashboard

| Test | Status | Weakness severity | Confidence | One-sentence basis | Key evidence IDs |
|---|---|---|---|---|---|
| KT1 Novelty collision | | | | | |
| KT2 Dissertation coherence | | | | | |
| KT3 Ground truth/identifiability | | | | | |
| KT4 Simpler-baseline necessity | | | | | |
| KT5 Feasibility/dependencies | | | | | |
| KT6 Technological resilience | | | | | |

Allowed kill-test statuses:

- `NO FATAL FAILURE IDENTIFIED`
- `MATERIAL CONCERN`
- `POTENTIALLY FATAL`
- `FATAL CONFIRMED`
- `UNRESOLVED`
- `NOT REACHED DUE TO EARLY STOPPING`

Allowed severity values:

- `FATAL`
- `MATERIAL`
- `MINOR`
- `UNRESOLVED SEVERITY`
- `NO MATERIAL WEAKNESS IDENTIFIED`

Allowed confidence values:

- `HIGH`
- `MODERATE`
- `LOW`

## 8. Detailed kill-test analyses

Use the following structure for every test that is reached.

### KT1 — Novelty collision

- **Protocol question:** Does substantially equivalent prior work already exist?
- **Candidate-specific interpretation:**
- **Evidence examined:**
- **Strongest attack:**
- **Contradictory or preserving evidence:**
- **Failure-condition assessment:**
- **Non-failure interpretation:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT1:**

A confirmed novelty failure requires a `FATAL COLLISION CONFIRMED` source assessment under the protocol.

### KT2 — Dissertation coherence

Include the thesis-to-aim map:

| Aim | Scientific question | Thesis clause tested | Evidence produced | Dependency on other aims | Coherence judgment |
|---|---|---|---|---|---|

Then state:

- **Strongest incoherence argument:**
- **Can one thesis honestly encompass all aims?**
- **Could material narrowing preserve identity?**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT2:**

### KT3 — Ground truth and identifiability

- **Target construct or causal quantity:**
- **Proposed reference standard:**
- **Why the target can or cannot be known:**
- **Threats:** annotation convention, hindsight, leakage, circular judging, unobservability, site specificity, or other
- **Validation or partial-identification strategy:**
- **Strongest ground-truth failure case:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT3:**

### KT4 — Simpler-baseline necessity

| Baseline | Why scientifically serious | What it controls | Thesis-relevant outcomes | Required equivalence/non-inferiority criterion |
|---|---|---|---|---|

Then state:

- **Why proposed complexity may be necessary:**
- **Strongest simple-baseline domination case:**
- **Prospectively justified practical-equivalence margin or rule:**
- **Why statistical non-significance alone is insufficient:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT4:**

If no empirical result exists, report whether headroom is plausible, not established.

### KT5 — Feasibility and dependency failure

| Dependency | Availability | Criticality | Owner/gatekeeper | Expected decision point | Fallback | Consequence if unavailable | Evidence |
|---|---|---|---|---|---|---|---|

Availability:

- `GREEN`
- `YELLOW`
- `RED`

Criticality:

- `CORE`
- `SUPPORTING`
- `OPTIONAL`

Then state:

- **Minimum executable path:**
- **Fallback architecture:**
- **Any RED + CORE dependency without valid fallback:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT5:**

### KT6 — Technological and foundation-model resilience

- **Current capability deficiency:**
- **Underlying structural problem:**
- **What survives substantially stronger models:**
- **What would be commoditized or obsolete:**
- **Model-replacement test:**
- **Strongest obsolescence case:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT6:**

## 9. Non-kill stress tests

### ST1 — Dissertation-sized depth

Choose one:

- `CLEARLY DISSERTATION-SIZED`
- `PLAUSIBLY DISSERTATION-SIZED`
- `POSSIBLY ONE STRONG PAPER`
- `UNRESOLVED`

Provide:

- one-thesis publication/experiment decomposition;
- why each unit tests the same thesis;
- strongest scope-deflation argument;
- whether scope concern becomes fatal without changing identity;
- confidence.

### ST2 — Generalizability

Choose one:

- `METHODOLOGICALLY GENERAL`
- `GENERALIZABLE WITH EXPLICIT BOUNDARY CONDITIONS`
- `APPLICATION-BOUND`
- `UNRESOLVED`

Provide:

- healthcare-specific structure integral to the method;
- transferable methodological component;
- minimum external validation needed;
- strongest application-bound argument;
- confidence.

## 10. Strongest rejection case

Present the strongest evidence-based argument for rejecting the candidate as currently formulated.

Requirements:

- steelman the rejection;
- cite every source-derived premise;
- identify the exact kill test implicated;
- distinguish confirmed evidence from inference;
- state whether the attack is fatal, material, minor, or unresolved.

Avoid ceremonial objections that do not threaten the central thesis.

## 11. Strongest surviving scientific case

Only after completing the attacks, state what scientific case remains.

Requirements:

- do not introduce new claims absent from the packet;
- respond to the strongest rejection case rather than summarize benefits;
- state which thesis clauses remain defensible;
- identify what is merely unresolved;
- avoid career, commercial, immigration, prestige, or personal-interest arguments.

## 12. Cheapest discriminating test or experiment

| Field | Required candidate-specific answer |
|---|---|
| Decision question | |
| Procedure | |
| Inputs | |
| Strengthening outcome | |
| Weakening/failure outcome | |
| Estimated burden | |
| Why cheapest | |

The test must be executable enough that another researcher could perform it without first redefining the question.

## 13. Next evidence required

Specify one primary evidence package. Add secondary packages only when they resolve genuinely independent potentially fatal uncertainties.

| Required component | Candidate-specific answer |
|---|---|
| Evidence object | |
| Acquisition procedure | |
| Uncertainty addressed | |
| Decision consequence | |
| Completion criterion | |

Do not write only “more literature,” “expert review,” “run a pilot,” or “verify novelty.”

## 14. Phase 1 candidate outcome

- **Outcome:**
- **Outcome confidence:**
- **Most severe weakness:**
- **Weakness severity:**
- **Most decision-relevant unresolved question:**
- **Required material revision, if any:**
- **Why the revision preserves or changes candidate identity:**
- **Tests not reached due to early stopping:**
- **One-paragraph outcome rationale:**

### Outcome semantics reminder

- `SURVIVES`: no fatal failure identified at Phase 1 minimum-adequacy depth.
- `SURVIVES WITH MATERIAL REVISION`: the central identity survives, but explicit narrowing or revision is required.
- `UNRESOLVED`: a potentially fatal uncertainty remains without enough evidence for a survival/failure decision.
- `FAILS AS CURRENTLY FORMULATED`: confirmed evidence defeats the dissertation-level case or requires replacement of its central object or thesis.

## 15. Candidate citation audit

Mark each `PASS`, `FAIL`, or `NOT APPLICABLE`.

| Check | Result | Notes |
|---|---|---|
| Every decision-relevant source-derived claim cited at point of use | | |
| Numerical claims and quotations specifically cited | | |
| Supported syntheses cite all load-bearing sources | | |
| Search non-findings point to the search audit | | |
| Source-inspection depth accurately recorded | | |
| Mutable sources include version/access date | | |
| Every provisional source ID resolves to the local registry | | |
| No abstract-only source treated as confirmed fatal without qualification | | |
| No private or restricted information exposed | | |

---

# Layer III — Cross-candidate Phase 1 summary

This layer summarizes the stream's own eight scans. It does not rank candidates.

## A. Outcome distribution

| Outcome | Candidates | Count |
|---|---|---:|
| SURVIVES | | |
| SURVIVES WITH MATERIAL REVISION | | |
| UNRESOLVED | | |
| FAILS AS CURRENTLY FORMULATED | | |

Counts are descriptive and must not be treated as scores.

## B. Fatal-risk map

| Candidate | Novelty | Coherence | Ground truth | Simpler baseline | Feasibility | Resilience | Highest-severity risk |
|---|---|---|---|---|---|---|---|

Use only the standardized kill-test statuses.

## C. Deep-work priority map for Phase 2 reconciliation

| Candidate | Unresolved question | Disagreement anticipated? | Why additional evidence could change status | Proposed Phase 3 task type |
|---|---|---|---|---|

Do not rank by personal preference. Priority here means expected decision impact.

## D. Shared sources and cross-candidate collisions

List sources or methods that materially affect more than one candidate.

| Source/method | Candidates affected | Different citation roles | Risk of inconsistent interpretation |
|---|---|---|---|

Do not merge candidate identities merely because they share a source or method.

## E. Candidate-definition disagreements

| Candidate | Disputed packet clause | Consequence | Can Phase 1 conclusions still be compared? | Required Phase 2 action |
|---|---|---|---|---|

## F. Search-coverage limitations

State:

- methodological fields not searched adequately;
- inaccessible decisive sources;
- candidates for which Phase 1 adequacy was not reached;
- areas where unsaturated search could conceal a fatal collision;
- whether any overall outcome must therefore remain unresolved.

## G. Strategic-contamination audit

For each candidate, confirm:

> The outcome would be unchanged if the candidate had no unusual career, immigration, commercial, prestige, or personal-interest value.

List and correct any exception.

## H. Stream-level stopping-condition statement

Explain why additional work in this independent Phase 1 pass is unlikely to change the current candidate outcomes, confidence assignments, unresolved questions, or next-evidence requests without entering Phase 3 depth.

---

# Layer IV — Artifact integrity and freeze report

## A. Deterministic repository checks

Confirm:

1. the branch began from the approved canonical base;
2. the protocol, schema, and all eight packet versions match the execution contract;
3. no Day 1 artifact, normalization artifact, packet, decision, literature record, evidence record, or other stream artifact changed;
4. only the Phase 1 stream-local artifact was added;
5. no `.DS_Store` or unrelated file was staged or committed;
6. no permanent `LIT-###` identifier was assigned to a newly discovered source;
7. all provisional source identifiers are unique within the artifact;
8. internal links and source identifiers resolve where mechanically checkable.

## B. Final report

Report:

- branch;
- base repository commit;
- commit identifier;
- changed-file list;
- artifact line count;
- artifact Secure Hash Algorithm hash where available;
- packet versions evaluated;
- candidate outcome distribution;
- number of candidate-definition disagreements;
- number of potentially fatal collisions;
- number of confirmed fatal collisions;
- candidates stopped early;
- unresolved citation/source entries;
- confirmation nothing was pushed or merged.

## C. Freeze declaration

End with:

> **STATUS: FROZEN — PHASE 1 INDEPENDENT FATAL-RISK SCAN.**
>
> This artifact records one stream's independent Phase 1 judgments. It does not rank candidates, select finalists, establish global novelty, begin Phase 2 reconciliation, or incorporate another stream's Phase 1 conclusions.

---

# Phase 1 execution prohibitions

During Phase 1, do not:

- read another stream's Phase 1 output;
- rank the eight candidates;
- select finalists;
- average Day 1 verdicts;
- use cross-stream convergence count as evidence of scientific quality;
- modify a Candidate Evaluation Packet;
- redefine a candidate silently;
- assign permanent identifiers to newly discovered sources;
- modify shared literature, evidence, candidate, decision, or protocol files;
- use career, compensation, employer, immigration, commercialization, prestige, or personal-preference criteria;
- claim global novelty from a search non-finding;
- treat statistical non-significance as equivalence;
- treat source counts as evidence quality;
- begin Phase 2 reconciliation or Phase 3 deep falsification.

---

# Schema readiness gate

This draft becomes operational only after:

1. user approval;
2. canonical integration into `main`;
3. an `analysis/README.md` pointer where appropriate;
4. creation and approval of all eight Candidate Evaluation Packets;
5. confirmation that all three streams can access the same canonical commit.

**STATUS: DRAFT — USER REVIEW REQUIRED. NO PHASE 1 SCAN IS AUTHORIZED SOLELY BY THIS DRAFT.**
