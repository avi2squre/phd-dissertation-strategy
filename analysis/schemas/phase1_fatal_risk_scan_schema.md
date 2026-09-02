# Phase 1 Fatal-Risk Scan Schema

- **Version:** Draft 0.2
- **Date:** 2026-09-01
- **Status:** **DRAFT — USER REVIEW REQUIRED**
- **Governing protocol:** [`analysis/ADVERSARIAL_FALSIFICATION_PROTOCOL.md`](../ADVERSARIAL_FALSIFICATION_PROTOCOL.md), version 1.0
- **Purpose:** standardize the common candidate target, minimum search coverage, evidence reporting, decision rules, package structure, and freeze procedure for the three independent Phase 1 fatal-risk scans

This schema defines the exact structure every analysis stream must use during Phase 1. It does not prescribe conclusions. All scientific definitions, source hierarchies, collision semantics, kill tests, stress tests, evidence rules, information-flow rules, and strategic exclusions come from the governing protocol and must not be redefined locally.

Phase 1 asks:

> What could kill each of the eight normalized candidate dissertation directions?

Phase 1 is a broad, independent fatal-risk scan. It is not a final novelty determination, a systematic review, a candidate ranking, a finalist-selection exercise, or a strategic comparison.

---

# Part I - Common Candidate Evaluation Packet set

## 1. Packet-set purpose

Before any stream begins Phase 1, all eight normalized candidates must have one approved **Candidate Evaluation Packet**. Every stream must evaluate the identical packet set and packet version.

The packet set prevents three reviewers from attacking different versions of the same normalized direction. A stream may disagree with a packet, but it may not silently substitute a broader, narrower, or preferred formulation.

Recommended location:

```text
analysis/candidate_packets/
├── README.md
├── N1_candidate_evaluation_packet.md
├── N2_candidate_evaluation_packet.md
├── N3_candidate_evaluation_packet.md
├── N4a_candidate_evaluation_packet.md
├── N4b_candidate_evaluation_packet.md
├── N5_candidate_evaluation_packet.md
├── N6_candidate_evaluation_packet.md
└── N7_candidate_evaluation_packet.md
```

## 2. Packet-set manifest

`analysis/candidate_packets/README.md` is the authoritative packet-set manifest.

It must record:

- **Packet-set version**
- **Status:** `APPROVED - COMMON PHASE 1 TARGET SET`
- **Protocol version**
- **Phase 1 schema version**
- **Source/base repository commit**
- **Source normalization artifact**
- **Approval date**
- **Approval record**
- **Superseded packet-set versions**, if any

It must include:

| Candidate | Packet path | Packet version | Packet status | Packet content fingerprint or Git blob identifier | Constituent source artifacts |
|---|---|---|---|---|---|

### 2.1 Self-reference rule

A packet or Phase 1 artifact must not be required to embed the identifier of the commit that first introduces that exact file. Adding such an identifier changes the file and therefore changes the commit.

Accordingly:

- each packet records its source/base commit, packet-set version, and source provenance;
- the packet-set manifest may record fingerprints or Git blob identifiers for the eight packet files because the manifest is a separate file;
- the manifest does not need to contain its own file digest or the identifier of the commit that introduces the manifest;
- the final integration commit is reported through Git history, the Pull Request record where applicable, and the post-commit completion report;
- output file SHA-256 digests are reported after the files have been committed, not inserted into the files whose digests they describe.

Use precise terminology:

- **commit identifier** for a Git commit object;
- **Git blob identifier** for a file-content object in Git;
- **Secure Hash Algorithm 256-bit (SHA-256) digest** for an independently calculated file digest.

Avoid the redundant phrase `Secure Hash Algorithm hash`.

## 3. Individual Candidate Evaluation Packet template

Each packet must use the following structure.

### Packet metadata

- **Candidate identifier:**
- **Candidate title:**
- **Packet version:**
- **Packet-set version:**
- **Packet status:** `APPROVED - COMMON PHASE 1 TARGET`
- **Date approved:**
- **Source/base repository commit:**
- **Source normalization artifact:** `analysis/round3_normalization_reconciliation.md`
- **Constituent Day 1 artifacts and sections:**
- **Approval record:**
- **Packet fingerprint location:** packet-set manifest

The packet must not claim a commit identifier that did not yet exist when the packet was authored.

### 3.1 Central scientific object

State the principal representation, controller, algorithm, contract, inference framework, evaluation instrument, or other methodological object under evaluation.

This must be specific enough to distinguish the candidate from a broad research family.

### 3.2 Exact falsifiable thesis

State one central dissertation-level claim that can be supported, weakened, or defeated.

The thesis must identify:

- the proposed object or mechanism;
- the meaningful comparator;
- the target outcome;
- the conditions or domain in which the claim is expected to hold.

### 3.3 Included scientific scope

List the claims, mechanisms, task settings, and validation domains that belong to the candidate as evaluated in Phase 1.

### 3.4 Explicitly excluded scientific scope

List nearby ideas that do not belong to the candidate and must not be silently added to make it easier to defend or attack.

For merged Day 1 candidates, distinguish:

- mandatory shared core;
- competing formulations to compare;
- complementary formulations;
- optional validation domains;
- constituent claims deliberately excluded from the common target;
- adjacent theses preserved as separate candidates.

### 3.5 Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|

Use relationship language such as:

- common core;
- competing mechanism;
- complementary mechanism;
- scoped specialization;
- validation instantiation;
- excluded adjacent thesis.

### 3.6 Provisional coherent aims

Normally provide two or three aims.

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|

The aims are provisional targets for coherence testing. A Phase 1 reviewer may identify incoherence but may not silently replace them.

### 3.7 Decisive or discriminating experiment

State the comparison most directly capable of distinguishing the thesis from a serious alternative explanation or simpler baseline.

Include:

- experimental or analytical unit;
- strongest comparator;
- primary thesis-relevant outcome;
- result pattern that supports the thesis;
- result pattern that defeats or materially weakens it.

### 3.8 Inherited dangerous prior art

List the prior work already identified as most likely to collide with the candidate.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|

This is a required starting point, not a closed search universe.

### 3.9 Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|

### 3.10 Feasibility assumptions inherited from Day 1

List only assumptions necessary to understand the candidate target. Phase 1 independently evaluates them under Kill Test 5.

### 3.11 Packet provenance and change control

Record:

- exact source artifacts;
- source/base repository commit;
- which statements are direct compressions;
- which statements are reconciled formulations;
- unresolved candidate-definition tensions;
- user approval date.

A packet may not be materially changed after Phase 1 begins. A material packet change requires:

1. stopping all affected scans;
2. user approval;
3. a new packet and packet-set version;
4. an explicit comparability assessment for any already completed scan;
5. either rerunning affected scans or clearly excluding incomparable results.

## 4. Packet-fidelity approval workflow

Before Phase 1 begins:

1. the coordinator drafts all eight packets from the Round 3 normalization and constituent Day 1 artifacts;
2. the other analysis streams independently audit packet fidelity without performing external scientific research;
3. disagreements are classified as candidate-definition disagreements;
4. the coordinator reconciles disagreements without silently changing candidate identity;
5. the user approves the complete packet set;
6. the packet set is integrated into the canonical repository state;
7. all three Phase 1 streams begin from the same canonical commit and packet-set version.

Packet review asks only:

> Does this packet faithfully encode the normalized candidate we agreed to falsify?

It does not assess novelty, feasibility, ranking, career value, or strategic preference.

---

# Part II - Phase 1 logical artifact package

## 5. One logical artifact, multiple files

Each stream produces one **logical Phase 1 artifact package**, not one monolithic Markdown file.

Recommended structure:

```text
analysis/analysis_01/phase1_fatal_risk_scan/
├── README.md
├── source_registry.md
├── N1.md
├── N2.md
├── N3.md
├── N4a.md
├── N4b.md
├── N5.md
├── N6.md
└── N7.md
```

Use the same structure for `analysis_02` and `analysis_03`.

The package is one frozen analytical artifact distributed across files for retrieval, review, citation tracing, and cross-stream comparison.

### 5.1 Package file responsibilities

`README.md` contains:

- execution contract;
- independence and contamination declarations;
- package file manifest;
- candidate overview dashboard;
- source/search summary;
- cross-candidate Phase 1 synthesis;
- package-level citation and integrity checks;
- freeze declaration.

`source_registry.md` contains:

- one deduplicated stream-level source registry;
- permanent and provisional source identifiers;
- source metadata;
- version/access dates;
- maximum inspection depth;
- citation roles;
- candidates and sections using each source.

Each candidate file contains:

- the approved candidate target;
- packet-fidelity check;
- search concept map and audit;
- decision-relevant claim ledger;
- prior-art screening and collision matrices;
- six kill tests;
- two stress tests;
- rejection and surviving cases;
- discriminating test;
- next evidence;
- candidate outcome;
- citation audit.

### 5.2 Required frozen status

The package `README.md` must end with:

> **STATUS: FROZEN — PHASE 1 INDEPENDENT FATAL-RISK SCAN.**

Earlier files and packet definitions remain unchanged.

## 6. Embedded provenance versus post-commit reporting

### 6.1 Information embedded in the package

Record inside `README.md`:

- date;
- stream identifier;
- branch name;
- base repository commit;
- governing protocol version;
- schema version;
- packet-set version;
- packet paths and versions;
- permitted and excluded inputs;
- external-search scope;
- parallelism;
- stopping condition.

### 6.2 Information reported after commit

The completion report, outside the package files, records:

- output commit identifier;
- branch head;
- changed-file list;
- SHA-256 digest of each package file where available;
- package line counts;
- Git status;
- push/merge status.

Do not create a second content-changing commit merely to insert the first output commit identifier into the artifact.

---

# Part III - Package README structure

# Layer I - Execution contract and executive navigation

## A. Execution contract

Record before substantive execution:

- **Date:**
- **Analysis-stream identifier:**
- **Branch:**
- **Base repository commit:**
- **Governing protocol version:**
- **Phase 1 schema version:**
- **Candidate packet-set version:**
- **Candidate packet-set canonical repository commit:**
- **Candidate packet paths and versions:**
- **Objective:**
- **Repository files permitted:**
- **Repository files deliberately excluded:**
- **Other-stream Phase 1 outputs prohibited:** yes
- **External research:** allowed
- **External source classes permitted:**
- **Parallelism used:** yes/no
- **Accountable synthesizing process:**
- **Parallelism justification:**
- **Subagent or delegated-work disclosure:**
- **Expected artifact package:**
- **Stopping condition:**

The base must contain the approved protocol, schema, manifest, and all eight packet versions.

## B. Parallelism accountability

Parallel processes may assist with:

- separate search layers;
- source retrieval;
- candidate-specific evidence extraction;
- citation-chain tracing;
- deterministic validation.

Every delegated process must receive:

- the same packet-set version;
- the same candidate packet;
- the same protocol and schema versions;
- the same independence restrictions.

No delegated process may read another stream's Phase 1 conclusions.

One accountable reasoning process within the stream must synthesize:

- collision dispositions;
- kill-test statuses;
- severities;
- confidence;
- candidate outcomes.

Final scientific judgments must not be produced by mechanically voting across subagents.

Disclose:

| Delegated unit | Assigned scope | Inputs | Output used | Scientific judgment delegated? | Notes |
|---|---|---|---|---|---|

## C. Independence and contamination declarations

State explicitly:

1. whether any other stream's Phase 1 output was seen;
2. whether any accidental exposure occurred;
3. whether exposure preceded or followed the independent judgment;
4. whether strategic criteria influenced any scientific judgment;
5. whether each scientific outcome would remain unchanged if all candidates had equal career, immigration, commercial, prestige, and personal-interest value;
6. whether another stream's source interpretation was inherited without independent inspection.

## D. Package file manifest

| File | Required? | Present? | Purpose | Frozen status |
|---|---|---|---|---|
| README.md | yes | | package-level contract and synthesis | |
| source_registry.md | yes | | deduplicated source registry | |
| N1.md | yes | | candidate scan | |
| N2.md | yes | | candidate scan | |
| N3.md | yes | | candidate scan | |
| N4a.md | yes | | candidate scan | |
| N4b.md | yes | | candidate scan | |
| N5.md | yes | | candidate scan | |
| N6.md | yes | | candidate scan | |
| N7.md | yes | | candidate scan | |

## E. Candidate overview dashboard

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

A Phase 1 `SURVIVES` outcome means only that no fatal failure was identified at Phase 1 minimum-adequacy depth. It is not a final novelty, finalist, or strategic judgment.

## F. Source and search summary

| Candidate | Search layers 1-6 attempted | Citation-chain expansion | Unique works screened | Unique works inspected at depth 3+ | Potentially fatal collisions | Confirmed fatal collisions | Search-coverage limitation |
|---|---:|---|---:|---:|---:|---:|---|

Counts are descriptive audit information, not quality scores.

### F.1 Counting rules

- **Unique works screened:** distinct scholarly or technical works screened after deduplication across queries for that candidate.
- A source discovered through several queries is counted once for that candidate.
- **Unique works inspected at depth 3+:** distinct works inspected at `relevant sections`, `full text`, or `reproduced/validated` depth.
- Search layers attempted count Layers 1 through 6 only.
- Citation-chain expansion is reported separately as `YES`, `NO`, or `NOT APPLICABLE`.
- When exact counts are unavailable, prefix an estimate with `≈`.
- Package-level source counts may be smaller than the sum of candidate counts because one source may affect several candidates.

### F.2 Most consequential accessible threat

The most consequential threat is the accessible source with the greatest plausible ability to defeat, in order:

1. the exact falsifiable thesis;
2. the central scientific object;
3. the methodological contribution;
4. the decisive experiment.

Do not select it by popularity, recency, venue prestige, or keyword similarity alone.

If the most consequential apparent source is inaccessible:

- record it as an unresolved threat;
- explain why it could be fatal;
- inspect the next most consequential accessible source;
- mark the relevant novelty judgment or candidate outcome unresolved when the inaccessible source could plausibly conceal a fatal collision.

---

# Part IV - Stream-level source registry

## 7. One deduplicated source registry

Use one `source_registry.md` for the complete stream package.

Existing registered sources retain their permanent `LIT-###` identifiers.

New sources discovered during blind Phase 1 receive stream-local provisional identifiers:

```text
S01-P1-SRC-001
S02-P1-SRC-001
S03-P1-SRC-001
```

Identifiers must be unique across all eight candidate files within the stream.

The same source must not receive several provisional identifiers merely because it appears under several candidates.

## 8. Source registry table

| Source ID | Full citation | Stable identifier/link | Source tier | Version/access date | Maximum inspection depth | Citation role(s) | Candidates and sections used | Notes |
|---|---|---|---|---|---|---|---|---|

The source registry records the **maximum** inspection depth reached anywhere in the package.

A candidate's decision-relevant claim ledger records the inspection depth actually supporting each claim. These values may differ.

Mutable sources must record:

- version;
- retrieval/access date;
- archived snapshot, release, commit, or tag where feasible.

Examples include:

- arXiv preprints;
- model cards;
- technical reports;
- software documentation;
- code repositories;
- online benchmarks;
- living standards;
- official system pages.

## 9. Source identity and deduplication

Deduplicate works using stable identifiers where available:

1. Digital Object Identifier;
2. official proceedings identifier;
3. PubMed Identifier or PubMed Central Identifier;
4. arXiv identifier and version;
5. canonical technical-report identifier;
6. official repository plus release/tag/commit;
7. normalized title/authors/year when no stable identifier exists.

Preprint and published versions of the same work should normally share one conceptual source entry with version relationships recorded, unless substantive differences require separate treatment.

---

# Part V - Candidate-file structure

Repeat the following structure in `N1.md`, `N2.md`, `N3.md`, `N4a.md`, `N4b.md`, `N5.md`, `N6.md`, and `N7.md`.

# Candidate [ID] - [Approved packet title]

## 1. Candidate target and packet fidelity

### 1.1 Packet fingerprint

- **Candidate identifier:**
- **Packet path:**
- **Packet version:**
- **Packet-set version:**
- **Packet source/base commit:**
- **Packet fingerprint or Git blob identifier from manifest:**
- **Central scientific object copied from packet:**
- **Exact falsifiable thesis copied from packet:**

### 1.2 Scope fidelity declaration

Choose one:

- `PACKET ACCEPTED AS EVALUATION TARGET`
- `CANDIDATE-DEFINITION DISAGREEMENT`

The reviewer must evaluate the approved packet as written wherever possible.

A packet that appears overly broad, narrow, or incoherent is evidence under Kill Test 2. It is not permission to replace the packet.

Evaluation is **logically impossible** only when the packet:

- contains internally contradictory mandatory clauses;
- fails to identify a coherent scientific object;
- fails to specify a meaningful comparator;
- fails to specify a target outcome;
- cannot be interpreted without choosing among mutually exclusive theses.

If a candidate-definition disagreement exists, record:

- disputed packet clause;
- reviewer's interpretation;
- why it materially affects falsification;
- whether the packet was nevertheless evaluated as written;
- separable kill tests that remain evaluable;
- affected judgments marked `UNRESOLVED`;
- exact packet correction requested for Phase 2.

### 1.3 Steelmanned scientific case

In no more than one substantive paragraph, state the strongest coherent version of the approved packet without adding a new thesis.

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

| Search layer | Query families or concepts | Databases, proceedings, or sources | Unique works screened | Unique works inspected at depth 3+ | New collision class found? | Omitted scope and rationale |
|---|---|---|---:|---:|---|---|
| 1. Exact formulation | | | | | | |
| 2. Conceptual synonyms | | | | | | |
| 3. Method-centric | | | | | | |
| 4. Adjacent biomedical | | | | | | |
| 5. Parent discipline | | | | | | |
| 6. Older/foundational | | | | | | |
| Citation-chain expansion | | | | | | |

Use the counting rules in Package README Section F.

### 3.1 Phase 1 minimum-adequacy checklist

Mark each item `COMPLETE`, `INCOMPLETE`, or `NOT APPLICABLE`, with a brief explanation.

| Requirement | Status | Evidence/location |
|---|---|---|
| Search concept map completed | | |
| Every applicable search layer initially attempted | | |
| Inherited dangerous prior art inspected | | |
| Newly surfaced direct threats screened | | |
| Most consequential accessible threat inspected at relevant-section depth | | |
| Inaccessible potentially fatal threats logged | | |
| Six kill tests assessed or early stop justified | | |
| Two stress tests assessed or early stop justified | | |
| Cheapest discriminating test specified | | |
| Concrete next-evidence request specified | | |
| Decision-relevant claim ledger completed | | |
| Candidate citation audit completed | | |

### 3.2 Saturation statement

Choose one:

- `PHASE 1 ADEQUACY REACHED - DEEP SATURATION NOT CLAIMED`
- `PHASE 1 ADEQUACY NOT REACHED`
- `DEEP SATURATION REACHED FOR A SPECIFIED SUBQUESTION`

State:

- which search areas remain unsaturated;
- which unsaturated areas could plausibly conceal a fatal result;
- whether the limitation affects only one collision judgment, one kill test, or the complete candidate outcome;
- why additional work belongs in Phase 3 rather than the current broad scan.

Failure to reach deep saturation does not automatically make the full candidate `UNRESOLVED`. The candidate becomes `UNRESOLVED` only when the unsaturated area could plausibly conceal a fatal result or prevent application of the outcome hierarchy.

## 4. Decision-relevant claim ledger

A **decision-relevant claim** is any claim that materially supports or changes:

- a relevance decision;
- a collision disposition;
- a kill-test status;
- weakness severity;
- confidence;
- candidate outcome;
- cheapest discriminating test;
- next evidence required.

Use stream-local claim identifiers, for example:

```text
S01-P1-N1-CLM-001
S02-P1-N4a-CLM-003
S03-P1-N7-CLM-012
```

| Claim ID | Decision-relevant claim | Evidentiary status | Source ID(s) | Claim-specific inspection depth | Citation role | Kill test or outcome affected | Point-of-use location |
|---|---|---|---|---|---|---|---|

This ledger supplements, rather than replaces, point-of-use citations.

A source registry may record a full-text maximum depth while a particular claim is supported only by one relevant section. Record the claim-specific depth honestly.

## 5. Prior-art relevance screening

Record significant screened sources, including serious threats and instructive non-collisions.

| Source ID | Thesis-defining component addressed | Relevance decision | Rationale | Advance to overlap matrix? |
|---|---|---|---|---|

Allowed relevance decisions:

- `OUT-OF-SCOPE HIT`
- `NON-COLLIDING RELATED WORK`
- `ADVANCE TO COLLISION ASSESSMENT`
- `UNRESOLVED RELEVANCE`

Do not use the phrase `irrelevant collision`.

## 6. Contribution-overlap assessment

Create a separate matrix for every source classified as a serious collision threat.

### Source [ID] - [Short title]

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

Operational meanings:

- **NONE:** no substantive overlap on the dimension.
- **PARTIAL:** a recognizable component or subproblem overlaps, but an independent thesis-defining contribution remains.
- **STRONG:** the source contains most of the candidate's contribution on that dimension and materially narrows the remaining novelty claim.
- **NEAR-IDENTICAL:** substantially the same object, formulation, method, or experiment; remaining differences are mainly implementation, data, model, scale, or domain.

These are dimension-level ratings, not final collision dispositions. Do not sum them mechanically.

Then record:

- **Collision disposition:**
- **Disposition rationale:**
- **Inspection-depth sufficiency:**
- **Most consequential threat status:** yes/no
- **Remaining contradictory evidence:**
- **Effect on the packet's novelty claim:**
- **Claim-ledger references:**

Allowed dispositions:

- `NON-COLLIDING RELATED WORK`
- `PARTIAL COLLISION`
- `MAJOR COLLISION`
- `POTENTIALLY FATAL COLLISION`
- `FATAL COLLISION CONFIRMED`
- `UNRESOLVED COLLISION`

A confirmed novelty failure requires a `FATAL COLLISION CONFIRMED` assessment satisfying the governing protocol.

## 7. Kill-test dashboard

| Test | Status | Weakness severity | Confidence | One-sentence basis | Key claim/evidence IDs |
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

Canonical weakness severities:

- `FATAL`
- `MATERIAL`
- `MINOR`
- `UNRESOLVED SEVERITY`

Display placeholders:

- `NONE IDENTIFIED`
- `NOT ASSESSED`

The display placeholders are not additional severity categories.

### 7.1 Status-severity compatibility

| Kill-test status | Normally compatible severity |
|---|---|
| `NO FATAL FAILURE IDENTIFIED` | `MINOR` or `NONE IDENTIFIED` |
| `MATERIAL CONCERN` | `MATERIAL` |
| `POTENTIALLY FATAL` | `UNRESOLVED SEVERITY` |
| `FATAL CONFIRMED` | `FATAL` |
| `UNRESOLVED` | `MINOR`, `MATERIAL`, or `UNRESOLVED SEVERITY`, with explanation |
| `NOT REACHED DUE TO EARLY STOPPING` | `NOT ASSESSED` |

Any departure from this table requires an explicit rationale.

## 8. Detailed kill-test analyses

Use the following structure for every test reached.

### KT1 - Novelty collision

- **Protocol question:** Does substantially equivalent prior work already exist?
- **Candidate-specific interpretation:**
- **Evidence examined:**
- **Most consequential threat:**
- **Strongest attack:**
- **Contradictory or preserving evidence:**
- **Failure-condition assessment:**
- **Non-failure interpretation:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT1:**
- **Claim-ledger references:**

A confirmed novelty failure requires a `FATAL COLLISION CONFIRMED` source assessment.

### KT2 - Dissertation coherence

Include:

| Aim | Scientific question | Thesis clause tested | Evidence produced | Dependency on other aims | Coherence judgment |
|---|---|---|---|---|---|

Then state:

- **Strongest incoherence argument:**
- **Can one thesis honestly encompass all aims?**
- **Could material narrowing preserve identity?**
- **Candidate-definition disagreement implicated?**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT2:**

### KT3 - Ground truth and identifiability

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
- **Claim-ledger references:**

### KT4 - Simpler-baseline necessity

| Baseline | Why scientifically serious | What it controls | Thesis-relevant outcomes | Prospectively justified equivalence/non-inferiority criterion |
|---|---|---|---|---|

Then state:

- **Why proposed complexity may be necessary:**
- **Strongest simple-baseline domination case:**
- **Practical-equivalence margin or rule:**
- **When and why the rule was specified:**
- **Thesis-relevant dimensions included:** performance, calibration, robustness, clinically weighted error, action cost, human workload, compute, interpretability, generalization, or other
- **Why statistical non-significance alone is insufficient:**
- **Status:**
- **Severity:**
- **Confidence:**
- **Next evidence specific to KT4:**
- **Claim-ledger references:**

If no empirical result exists, report whether headroom is plausible, not established.

### KT5 - Feasibility and dependency failure

| Dependency | Availability | Criticality | Owner/gatekeeper | Expected decision point | Fallback | Consequence if unavailable | Evidence/claim IDs |
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
- **Claim-ledger references:**

### KT6 - Technological and foundation-model resilience

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
- **Claim-ledger references:**

## 9. Non-kill stress tests

### ST1 - Dissertation-sized depth

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
- confidence;
- claim/evidence references where source-derived.

### ST2 - Generalizability

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
- confidence;
- claim/evidence references where source-derived.

## 10. Strongest rejection case

Present the strongest evidence-based argument for rejecting the candidate as currently formulated.

Requirements:

- steelman the rejection;
- cite every source-derived premise;
- identify the exact kill test implicated;
- distinguish directly verified findings from synthesis and hypothesis;
- state whether the attack is fatal, material, minor, or unresolved;
- cite relevant claim-ledger entries.

Avoid ceremonial objections that do not threaten the central thesis.

## 11. Strongest surviving scientific case

Only after completing the attacks, state what scientific case remains.

Requirements:

- do not introduce a new thesis absent from the packet;
- answer the strongest rejection case rather than merely summarize benefits;
- state which thesis clauses remain defensible;
- identify what remains unresolved;
- exclude career, commercial, immigration, prestige, and personal-interest arguments;
- cite relevant claim-ledger entries.

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
| Kill test updated | |
| Completion criterion | |

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
| Responsible role or expertise | |
| Dependency or access requirement | |

Do not write only `more literature`, `expert review`, `run a pilot`, or `verify novelty`.

## 14. Candidate-outcome decision hierarchy

Apply this default hierarchy in order:

1. **Any `FATAL CONFIRMED` kill test**
   - Outcome: `FAILS AS CURRENTLY FORMULATED`.

2. **No confirmed fatal failure, but at least one unresolved potentially fatal issue**
   - Outcome: `UNRESOLVED`.

3. **No unresolved potentially fatal issue, but one or more material revisions are required**
   - Outcome: `SURVIVES WITH MATERIAL REVISION`.

4. **Phase 1 minimum adequacy reached, no fatal failure, no unresolved potentially fatal issue, and no required material revision**
   - Outcome: `SURVIVES`.

5. **Phase 1 minimum adequacy not reached**
   - Outcome: `UNRESOLVED`, unless sufficiently verified fatal evidence already requires `FAILS AS CURRENTLY FORMULATED`.

Any departure must state:

- the default outcome;
- the chosen outcome;
- the exact reason;
- the evidence supporting the exception.

Stress-test findings affect the candidate outcome only through a stated scientific consequence. For example, `POSSIBLY ONE STRONG PAPER` becomes fatal only when no coherent dissertation-scale expansion exists without replacing the candidate identity.

## 15. Phase 1 candidate outcome

- **Outcome:**
- **Outcome confidence:**
- **Default hierarchy applied:** yes/no
- **If no, exception rationale:**
- **Most severe weakness:**
- **Weakness severity:**
- **Most decision-relevant unresolved question:**
- **Required material revision, if any:**
- **Why the revision preserves or changes candidate identity:**
- **Tests not reached due to early stopping:**
- **One-paragraph outcome rationale:**
- **Claim-ledger references:**

Outcome reminders:

- `SURVIVES`: no fatal failure identified at Phase 1 minimum-adequacy depth.
- `SURVIVES WITH MATERIAL REVISION`: the central identity survives, but explicit narrowing or revision is required.
- `UNRESOLVED`: a potentially fatal uncertainty remains or minimum adequacy was not reached.
- `FAILS AS CURRENTLY FORMULATED`: confirmed evidence defeats the dissertation-level case or requires replacement of its central object or thesis.

## 16. Candidate citation audit

Mark each `PASS`, `FAIL`, or `NOT APPLICABLE`.

| Check | Result | Notes |
|---|---|---|
| Every decision-relevant source-derived claim appears in the claim ledger | | |
| Every such claim is cited at point of use | | |
| Numerical claims and quotations are specifically cited | | |
| Supported syntheses cite all load-bearing sources | | |
| Search non-findings point to the search audit | | |
| Source-inspection depth is accurately recorded | | |
| Mutable sources include version/access date | | |
| Every provisional source ID resolves to the package registry | | |
| No abstract-only source is treated as confirmed fatal without qualification | | |
| No private or restricted information is exposed | | |
| No permanent source ID was assigned independently | | |

---

# Part VI - Cross-candidate package summary

The following sections belong in the package `README.md`. They summarize one stream's own eight scans and do not rank candidates.

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

Use only standardized kill-test statuses.

## C. Decision-impact and downstream-evidence map

| Candidate | Unresolved question | Why it may change the outcome | Evidence class needed | Provisional Phase 3 task if unresolved after Phase 2 |
|---|---|---|---|---|

This table does not predict how another stream will disagree. It identifies questions with high expected decision impact.

## D. Shared sources and cross-candidate collisions

| Source or method | Candidates affected | Different citation roles | Risk of inconsistent interpretation | Registry ID |
|---|---|---|---|---|

Do not merge candidate identities merely because they share a source or method.

## E. Candidate-definition disagreements

| Candidate | Disputed packet clause | Why evaluation was affected | Can results still be compared? | Exact Phase 2 action required |
|---|---|---|---|---|

## F. Search-coverage limitations

State:

- methodological fields not searched adequately;
- inaccessible decisive sources;
- candidates for which Phase 1 adequacy was not reached;
- areas where unsaturated search could conceal a fatal collision;
- whether the limitation affects one judgment or the full candidate outcome;
- why further work belongs in Phase 3.

## G. Strategic-contamination audit

For every candidate, confirm:

> The outcome would be unchanged if the candidate had no unusual career, immigration, commercial, prestige, or personal-interest value.

List and correct any exception.

## H. Parallelism and synthesis audit

State:

- delegated searches or evidence tasks;
- whether every delegated unit received the same packet and protocol;
- whether any delegated unit saw another stream's conclusions;
- who or what process made the final scientific judgments;
- confirmation that no mechanical vote produced the candidate outcomes.

## I. Stream-level stopping-condition statement

Explain why additional work in this independent Phase 1 pass is unlikely to change the current candidate outcomes, confidence assignments, unresolved questions, or next-evidence requests without entering Phase 3 depth.

---

# Part VII - Artifact integrity and freeze report

## 17. Package-level citation audit

Confirm:

1. every provisional source identifier is unique across the package;
2. every provisional or permanent identifier resolves in `source_registry.md`;
3. source registry maximum inspection depths are consistent with candidate claim ledgers;
4. cross-candidate source uses retain candidate-specific citation roles;
5. mutable-source versions/access dates are present;
6. search non-findings reference candidate search audits;
7. restricted/private evidence is not exposed.

## 18. Deterministic repository checks

Confirm:

1. the branch began from the approved canonical base;
2. the protocol, schema, packet-set version, manifest, and eight packets match the execution contract;
3. no Day 1 artifact, normalization artifact, packet, decision, literature record, evidence record, protocol, schema, or other stream artifact changed;
4. only the Phase 1 stream-local package files were added;
5. the package contains exactly `README.md`, `source_registry.md`, and eight candidate files unless an exception was approved;
6. no `.DS_Store` or unrelated file was staged or committed;
7. no permanent `LIT-###` identifier was assigned to a newly discovered source;
8. all provisional source and claim identifiers are unique within the package;
9. internal links and source identifiers resolve where mechanically checkable;
10. file names and candidate ordering match the schema.

## 19. Embedded package freeze report

Record inside `README.md`:

- branch;
- base repository commit;
- protocol version;
- schema version;
- packet-set version;
- changed-file expectation;
- candidate outcome distribution;
- number of candidate-definition disagreements;
- number of potentially fatal collisions;
- number of confirmed fatal collisions;
- candidates stopped early;
- unresolved source entries;
- confirmation that no other stream's Phase 1 output was used;
- confirmation that no push or merge occurred before user review.

Do not embed the output commit identifier or file digests that would require a self-referential edit.

## 20. Post-commit completion report

After committing, report outside the artifact:

- branch;
- base repository commit;
- output commit identifier;
- branch head;
- complete changed-file list;
- line count for each package file;
- SHA-256 digest for each package file where available;
- packet-set version evaluated;
- candidate outcome distribution;
- candidate-definition disagreement count;
- potentially fatal collision count;
- confirmed fatal collision count;
- candidates stopped early;
- unresolved source entries;
- `git status` summary;
- confirmation no `.DS_Store` or unrelated file was committed;
- confirmation nothing was pushed or merged.

## 21. Freeze declaration

End the package `README.md` with:

> **STATUS: FROZEN — PHASE 1 INDEPENDENT FATAL-RISK SCAN.**
>
> This package records one stream's independent Phase 1 judgments. It does not rank candidates, select finalists, establish global novelty, begin Phase 2 reconciliation, or incorporate another stream's Phase 1 conclusions.

---

# Part VIII - Phase 1 prohibitions and readiness gate

## 22. Phase 1 execution prohibitions

During Phase 1, do not:

- read another stream's Phase 1 output;
- rank the eight candidates;
- select finalists;
- average Day 1 verdicts;
- use cross-stream convergence count as evidence of quality;
- modify a Candidate Evaluation Packet or packet manifest;
- silently redefine a candidate;
- assign permanent identifiers to newly discovered sources;
- modify shared literature, evidence, candidate, decision, protocol, or schema files;
- use career, compensation, employer, immigration, commercialization, prestige, or personal-preference criteria;
- claim global novelty from a search non-finding;
- treat statistical non-significance as equivalence;
- treat source counts as evidence quality;
- produce candidate outcomes by subagent voting;
- begin Phase 2 reconciliation or Phase 3 deep falsification.

## 23. Schema readiness gate

This draft becomes operational only after:

1. user approval;
2. canonical integration into `main`;
3. an `analysis/README.md` pointer where appropriate;
4. creation and approval of the packet-set manifest;
5. creation and approval of all eight Candidate Evaluation Packets;
6. completion of independent packet-fidelity audits;
7. confirmation that all three streams can access the same canonical commit and packet set.

**STATUS: DRAFT — USER REVIEW REQUIRED. NO PHASE 1 SCAN IS AUTHORIZED SOLELY BY THIS DRAFT.**
