# Adversarial Falsification Protocol

- **Version:** 1.0
- **Date adopted:** 2026-09-01
- **Repository base:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Status:** **CANONICAL — ADOPTED THROUGH DEC-009**
- **Scope:** scientific adversarial review of candidate dissertation directions, plus the controlled handoff to later strategic comparison

This document defines the common scientific rules, evidentiary standards, search methodology, decision semantics, citation requirements, and information-flow constraints for adversarial falsification in this repository. It standardizes the analytical instrument used by independent analysis streams without prescribing their conclusions.

The protocol is designed to answer one question:

> Does each candidate dissertation direction survive a serious attempt to defeat its dissertation-level scientific case?

---

# Part I — Authority, purpose, and scope

## 1. Purpose and optimization target

The purpose of adversarial falsification is to expose fatal or material weaknesses before substantial research time is committed. The protocol directs analysis toward evidence that could change the scientific status of a candidate rather than toward ceremonial criticism, supportive-literature accumulation, or advocacy.

The optimization target is:

> Maximize decision-relevant scientific uncertainty reduction per unit of researcher attention, model computation, source-reading effort, annotation effort, implementation effort, and institutional dependency.

This does **not** mean minimizing search depth or computational effort. Expensive work is justified when it materially improves novelty assessment, scientific validity, feasibility judgment, reproducibility, or decision quality. This principle inherits the compute-allocation and stopping rules in [`OPERATING_PROTOCOL.md`](../OPERATING_PROTOCOL.md).

A successful falsification phase may eliminate an attractive candidate, require material revision, or leave it unresolved. Finding that a candidate fails is useful because it prevents larger downstream losses.

## 2. Relationship to existing repository rules

This protocol supplements, and does not replace, the following repository authorities:

1. [`README.md`](../README.md), which defines canonical-state, analytical-independence, source-hierarchy, and public-repository rules.
2. [`OPERATING_PROTOCOL.md`](../OPERATING_PROTOCOL.md), which governs progressive context retrieval, stream independence, source reuse without claim inheritance, computation scaling, stopping rules, human checkpoints, and execution plans.
3. [`COMMON_ANALYSIS_SCHEMA.md`](COMMON_ANALYSIS_SCHEMA.md), which standardizes candidate-analysis structure, evidentiary labeling, advisor-complementarity treatment, and the separation between scientific and private strategic analysis.
4. [`round3_normalization_reconciliation.md`](round3_normalization_reconciliation.md), which freezes the eight normalized candidate dissertation directions entering adversarial falsification.
5. [`decisions/decision_log.md`](../decisions/decision_log.md), which records accepted project decisions and controls material changes to canonical process.

Where this protocol conflicts with a higher-level accepted decision, the accepted decision governs. Where a compressed repository statement conflicts with a primary scientific source, the primary source governs, consistent with `OPERATING_PROTOCOL.md`.

## 3. Scope, non-goals, canonical candidate set, and freeze boundary

### 3.1 Scientific scope

Phases 1 through 5 evaluate whether a candidate direction is scientifically defensible as a dissertation. They assess:

- novelty and prior-art collision;
- thesis coherence;
- ground-truth validity and identifiability;
- necessity beyond simpler baselines;
- feasibility and dependency risk;
- technological and foundation-model resilience;
- dissertation-sized depth;
- generalizability.

### 3.2 Canonical candidate set

The input set is the eight normalized identities frozen in [`round3_normalization_reconciliation.md`](round3_normalization_reconciliation.md):

1. **N1 — Structured Evidence-State Selective Control for Clinical Artificial Intelligence**
2. **N2 — Diagnostic-State Trajectory Representation and Inference**
3. **N3 — Machine-Checkable Causal Data-Fitness for Target-Trial Emulation**
4. **N4a — Process-Level Causal Failure Localization for Clinical Artificial Intelligence Agents**
5. **N4b — Versioned Continual Assurance and Change Attribution for Clinical Artificial Intelligence**
6. **N5 — Probabilistic Clinical Constraint Induction and Proof-Carrying Repair**
7. **N6 — Adequacy- and Currency-Aware Clinical Claim Verification**
8. **N7 — Measurement-Error-Aware Clinical Natural Language Processing Evaluation**

The normalized identities are frozen for the initial falsification pass. A reviewer may recommend narrowing or material revision, but may not silently replace a candidate's central scientific object or thesis.

### 3.3 Candidate Evaluation Packets

Before Phase 1 begins, every normalized direction must have one approved **Candidate Evaluation Packet**. The packet is the common target that all three streams must evaluate. It prevents different reviewers from attacking different variants of the same normalized direction.

Each packet must contain:

1. normalized identifier and title;
2. central scientific object;
3. exact falsifiable thesis being evaluated;
4. included scientific scope;
5. explicitly excluded scientific scope;
6. constituent Day 1 formulations and their relationship;
7. provisional coherent aims;
8. decisive or discriminating experiment;
9. inherited dangerous prior art;
10. known critical uncertainties;
11. source-artifact and Git commit provenance, where the commit is identified by its Secure Hash Algorithm (SHA) value.

All streams must evaluate the same packet. A reviewer may argue that the packet is incoherent, incomplete, or improperly scoped, but may not silently substitute a preferred formulation. Any disagreement about the target must be labeled **CANDIDATE-DEFINITION DISAGREEMENT** and preserved for reconciliation.

The exact packet template belongs in the Phase 1 schema.

### 3.4 Non-goals during scientific phases

Phases 1 through 5 do not evaluate or optimize:

- salary or total compensation;
- desirability to named employers;
- quantitative-finance recruiting value;
- immigration strategy or visa-category evidence;
- commercialization or startup upside;
- personal excitement;
- prestige;
- fashionable terminology.

Those criteria belong to Phase 6, after the scientifically viable set has been frozen. The scientific-versus-private-strategic distinction is already required by [`COMMON_ANALYSIS_SCHEMA.md`](COMMON_ANALYSIS_SCHEMA.md) and preserved by the Round 3 normalization artifact.

### 3.5 Freeze boundary

Earlier frozen artifacts must not be overwritten. New evidence, reconsideration, or reformulation must be recorded in a new phase artifact with explicit provenance. A change that replaces the central scientific object or falsifiable thesis creates a **redefined candidate**, not a routine edit.

---

# Part II — Core scientific semantics

## 4. Definition of adversarial falsification

**Adversarial falsification** is a structured attempt to defeat the current dissertation-level scientific case for a candidate direction. The reviewer actively searches for prior work, simpler explanations, invalid measurement assumptions, incoherent aims, inaccessible dependencies, or technological developments that would make the direction scientifically redundant, untestable, infeasible, insufficiently deep, or obsolete.

In this project, falsification is broader than demonstrating that one empirical hypothesis is false. A candidate may fail as a dissertation direction because:

- the thesis-defining contribution already exists;
- the aims require multiple unrelated theses;
- the proposed outcome cannot be measured validly;
- a simple baseline removes the need for the proposed method;
- the central experiment depends on resources unlikely to become available;
- the contribution disappears under ordinary model or tooling progress.

Therefore:

> A scientifically plausible idea is not automatically a viable dissertation direction.

And:

> A candidate that fails as currently formulated may still contain useful methods, experiments, resources, or narrower research questions.

All failure verdicts should use the phrase **as currently formulated** unless the evidence truly supports a broader statement.

## 5. Core terminology

### 5.1 Scientific case

The complete dissertation-level proposition being evaluated:

`central scientific object + falsifiable thesis + methodological contribution + coherent aims + evaluation strategy + feasibility`

Novelty cannot be assessed from a title, broad theme, or technology label alone.

### 5.2 Kill test

A structured test whose confirmed failure defeats the candidate's scientific case as currently formulated or requires changing its central scientific identity.

### 5.3 Stress test

A structured test that may materially affect scope, execution, or later comparison but does not automatically defeat the central thesis.

### 5.4 Fatal risk

A credible issue which, if confirmed, would require abandoning the candidate or replacing its central scientific object or thesis.

### 5.5 Material revision

A substantive narrowing or methodological change that preserves the candidate's central object and central thesis.

Examples include:

- narrowing a population, task, or validation domain;
- replacing one controller architecture while retaining the selective-control thesis;
- removing an overbroad aim;
- adding a required baseline or validation layer.

A change is not merely a material revision when it replaces the candidate's central object or thesis. That creates a redefined candidate and requires a human checkpoint.

### 5.6 Search non-finding

A documented search that did not identify qualifying evidence or prior work within its stated scope. A search non-finding is not evidence that no such work exists.

### 5.7 Search saturation

The condition in which additional well-designed searching is unlikely to reveal a new thesis-relevant collision class or change the current phase outcome, confidence, unresolved uncertainty, or next scientific action.

### 5.8 Phase 1 minimum adequacy

The minimum search and analysis coverage required to complete an independent fatal-risk scan without claiming deep-search saturation.

### 5.9 Prior-art collision

A prior contribution that overlaps the thesis-defining scientific object, method, hypothesis, or decisive experiment strongly enough to reduce novelty or require reformulation.

### 5.10 Discriminating test

A literature, analytical, empirical, simulation, annotation, implementation, or expert-assessment procedure whose plausible outcomes lead to meaningfully different candidate decisions.

### 5.11 Cheapest discriminating test or experiment

The lowest-burden feasible discriminating test expected to produce substantial decision-relevant information.

### 5.12 Next evidence required

The smallest specific additional evidence package needed to resolve the most decision-relevant remaining uncertainty.

### 5.13 Concrete evidence request

A request is **concrete** only when it specifies:

1. the evidence object;
2. how it will be acquired or produced;
3. the uncertainty it addresses;
4. the decision consequence of alternative outcomes;
5. the completion criterion.

“More research is needed” and “check whether the direction is novel” are not concrete.

### 5.14 Candidate-definition disagreement

A disagreement about the scientific target encoded in the Candidate Evaluation Packet, rather than about the evidence or evaluation of that target. It must be disclosed rather than resolved by silent reinterpretation.

## 6. Governing principles

### 6.1 Attack the thesis, not the vocabulary

The reviewer must test the scientific object, thesis, method, and decisive experiment. Similar terminology, model families, or datasets are weak evidence of collision.

### 6.2 Evaluate the common target

All streams must evaluate the same Candidate Evaluation Packet. A stream may criticize the packet but may not replace it silently with a broader, narrower, or preferred target.

### 6.3 Steelman before rejecting

A candidate should be evaluated in its strongest coherent formulation supported by the approved packet and frozen record. The reviewer may clarify ambiguity but may not invent a superior new candidate and then credit the original with surviving.

### 6.4 One thesis, multiple tests

A valid dissertation architecture requires one central falsifiable thesis. Aims may test different clauses, mechanisms, boundary conditions, or validation domains, but they must not be unrelated projects connected only by healthcare or artificial intelligence.

### 6.5 Search failure is not evidence of nonexistence

Allowed:

> No qualifying collision was identified within the documented search scope.

Not allowed:

> No prior work exists.

### 6.6 Source reuse does not imply interpretation inheritance

A stream may reuse a registered source identifier but must independently inspect and interpret the source when the interpretation is decision-relevant, consistent with [`OPERATING_PROTOCOL.md`](../OPERATING_PROTOCOL.md).

### 6.7 Scientific symmetry does not require equal conclusions

All streams use the same candidate packets, definitions, evidence rules, kill tests, output schema, and transition criteria. They are expected to disagree where their searches or reasoning differ.

### 6.8 Equal candidate status does not require equal computation

Every candidate receives the Phase 1 minimum scan. Additional effort is allocated according to decision consequence and unresolved fatal risk. A confirmed fatal result permits early termination after adequate documentation.

### 6.9 Strategic value cannot rescue scientific weakness

Career, compensation, immigration, commercialization, or prestige considerations are excluded from Phases 1 through 5.

### 6.10 Negative results are useful

A candidate that fails, a method that does not beat a simple baseline, or a benchmark that shows a presumed problem is small can still produce valuable knowledge. The falsification process evaluates dissertation viability, not whether every negative result is unpublishable.

---

# Part III — Evidence, citations, and search methodology

## 7. Evidentiary status, citation requirements, and source-inspection depth

Every decision-relevant claim must record both **evidentiary status** and **source-inspection depth**. These are separate axes.

### 7.1 Evidentiary-status labels

#### DIRECTLY VERIFIED FINDING

The source itself directly reports, proves, or demonstrates the claim, and the reviewer inspected the relevant material.

#### SUPPORTED SYNTHESIS

A cross-source inference grounded in multiple directly verified findings. No individual source necessarily states the synthesis.

#### PROVISIONAL HYPOTHESIS

A reasoned but unestablished proposition requiring additional evidence.

#### SEARCH NON-FINDING

No qualifying evidence or collision was identified within a documented search scope.

#### UNRESOLVED

Sources are inaccessible, contradictory, incomplete, or insufficient for a defensible judgment.

### 7.2 Source-inspection depth

1. **Metadata only:** title, authors, venue, date, and identifier.
2. **Title/abstract screened:** suitable for discovery and preliminary triage.
3. **Relevant sections inspected:** the methods, results, limitations, appendix, or supplementary material needed for the claim were read.
4. **Full text inspected:** the complete paper and relevant supplements were reviewed.
5. **Empirically reproduced or independently validated:** code, data, theorem, metric, or result was tested where feasible.

A paper should not normally cause a confirmed novelty-based failure from metadata or abstract alone. An abstract-level threat must be labeled **potentially fatal pending methods-level verification**.

### 7.3 Citation-integrity dimensions

Each artifact must satisfy:

- **Citation completeness:** claims requiring external support have citations.
- **Citation correctness:** the cited source supports the attributed claim.
- **Citation specificity:** the citation is close enough to identify the supported proposition.
- **Citation provenance:** the source has a stable retrievable identity.
- **Inspection transparency:** the artifact states what portion of the source was actually inspected.

### 7.4 Citation at point of use

Every source-derived factual, empirical, methodological, historical, or numerical claim must be cited sufficiently close to the claim that the source-claim relationship is unambiguous. A bibliography alone is insufficient.

Cross-paper syntheses must cite all load-bearing sources and remain labeled as synthesis. A citation must not be made to appear to prove a research gap or proposed hypothesis that the source itself does not establish. This extends the `claim -> source -> evidentiary status` rule in [`COMMON_ANALYSIS_SCHEMA.md`](COMMON_ANALYSIS_SCHEMA.md).

### 7.5 Stable identifiers and mutable-source provenance

Use stable scholarly identifiers whenever available, in approximately this order:

1. Digital Object Identifier (DOI);
2. official proceedings identifier, such as Association for Computational Linguistics Anthology or Association for Computing Machinery identifiers;
3. PubMed Identifier (PMID) or PubMed Central Identifier;
4. arXiv identifier;
5. stable publisher, repository, or official technical link.

For mutable sources, record the version and access date. Where feasible, preserve an archived snapshot, release identifier, or Git commit. This applies especially to:

- arXiv papers with multiple versions;
- model cards;
- software documentation;
- online benchmarks;
- official system pages;
- living technical reports;
- released code and datasets.

### 7.6 Numerical claims and quotations

Every source-specific numerical result must be cited at the point of use and must preserve the relevant metric, comparison, population, and experimental condition. Direct quotations should include page, section, table, figure, or line information where practical.

### 7.7 Research gaps and hypotheses

A citation may establish an observed result or limitation. It does not automatically establish:

- field-wide absence;
- dissertation novelty;
- the inferred research gap;
- the truth of the proposed hypothesis.

The inferential chain must remain visible:

`source-supported finding -> observed limitation -> reviewer inference -> preliminary gap hypothesis -> proposed research hypothesis`

### 7.8 Search non-findings

Search non-findings must cite or point to the phase search audit rather than to an unrelated scientific paper.

Preferred formulation:

> **SEARCH NON-FINDING:** No qualifying method was identified within the documented databases, query families, synonym sets, and citation chains used in this phase `[search-audit reference]`.

### 7.9 Internal project provenance

Claims about project decisions, candidate identities, freeze states, definitions, or prior analyses must cite the relevant repository artifact and, when decision-relevant, its Git commit identified through the Secure Hash Algorithm (SHA) value.

### 7.10 Existing and provisional source identifiers

Existing registered sources must reuse their permanent `LIT-###` identifier.

A new source discovered during an independent blind phase receives a stream-local provisional identifier:

```text
S01-P1-SRC-001
S02-P1-SRC-001
S03-P1-SRC-001
```

Each artifact must include a local source list with:

- provisional identifier;
- full citation;
- stable identifier or link;
- source type;
- version and access date where applicable;
- inspection depth;
- citation role.

Permanent `LIT-###` identifiers are reconciled only after independent outputs are frozen.

### 7.11 Citation-role vocabulary

Use one or more of the following roles for substantial source uses:

| Citation role | Meaning |
|---|---|
| Problem evidence | Establishes that the scientific problem exists or matters |
| Method precedent | Demonstrates an earlier method or formalism |
| Dangerous prior art | May materially reduce or defeat novelty |
| Baseline | Supplies a comparator the proposed method must beat |
| Limitation evidence | Reports a relevant weakness or failure |
| Ground-truth precedent | Supports labeling, adjudication, simulation truth, or validation design |
| Feasibility evidence | Supports availability of data, tools, compute, or implementation pathways |
| Theoretical foundation | Supplies formal or mathematical machinery |
| Contradictory evidence | Challenges a source, premise, or candidate claim |
| Search lead only | Used to discover primary material but not as decisive evidence |
| Internal provenance | Documents a repository decision or prior project-state claim |

### 7.12 Restricted and private evidence

Public artifacts must not expose protected health information, restricted links, credentials, private correspondence, sensitive institutional identifiers, enclave results, or private strategic material. Where restricted evidence is necessary, use a sanitized identifier such as:

```text
RESTRICTED-EVID-004
```

The public artifact should record the evidence type, scope, provenance class, and limitations without exposing protected content.

## 8. Source-quality and reference-provenance hierarchy

Source quality is evaluated relative to the claim being made.

### Tier 1 — Primary scholarly evidence

- peer-reviewed original research;
- official conference proceedings;
- journal articles;
- formal theoretical work.

Preferred for methodological, empirical, and theoretical claims.

### Tier 2 — Complete technical preprints

Recent preprints with sufficient methodological detail to evaluate the contribution. They can pose real novelty collisions, but publication status, version, and access date must be recorded.

### Tier 3 — Official technical artifacts

- official technical reports;
- released code;
- datasets;
- model cards;
- system documentation;
- standards;
- patents.

These can establish that a system or method exists, but do not necessarily establish scientific validity.

### Tier 4 — Reviews and surveys

Useful for field mapping, terminology, and discovery. Decision-critical claims should be escalated to the underlying primary sources.

### Tier 5 — Informal discovery sources

- blogs;
- news articles;
- marketing pages;
- social-media posts;
- search-result snippets.

These may identify leads but must not independently support a scientific kill decision.

A commercial system may threaten practical or commercial differentiation without defeating academic methodological novelty. Conversely, older theoretical work may defeat methodological novelty even if it has never been applied in healthcare.

## 9. Layered search methodology

Before searching, decompose the Candidate Evaluation Packet into a search concept map.

| Component | Questions to extract |
|---|---|
| Scientific object | What representation, controller, contract, algorithm, or evaluation instrument is proposed? |
| Mechanism | What learning, inference, repair, control, or checking mechanism is central? |
| Target failure | What specific deficiency is the method supposed to correct? |
| Falsifiable thesis | What claim would be shown wrong? |
| Decisive experiment | What comparison most directly tests the thesis? |
| Evaluation | What metrics, ground truth, and baselines define success? |
| Domain | Which clinical, biomedical, or health-data context is integral? |
| Parent disciplines | Which mature methodological fields may contain equivalent work? |

Searches should proceed through the following layers.

### Layer 1 — Exact formulation

Search the normalized title, coined terms, and direct paraphrases.

Purpose: identify obvious direct collisions.

### Layer 2 — Conceptual synonyms

Search the scientific object and problem using alternative terminology rather than the project's chosen labels.

Purpose: avoid false novelty caused by vocabulary mismatch.

### Layer 3 — Method-centric search

Remove healthcare terminology and search the core mechanism, representation, learning objective, or decisive experiment.

Purpose: identify general methods that subsume the proposed healthcare formulation.

### Layer 4 — Adjacent biomedical disciplines

Search medical informatics, biomedical natural language processing, epidemiology, clinical decision support, medical artificial intelligence, real-world evidence, and related fields.

Purpose: identify equivalent methods developed under neighboring application language.

### Layer 5 — Parent methodological disciplines

Search the mature disciplines most likely to contain the underlying contribution, including as applicable:

- machine learning;
- statistics;
- causal inference;
- reinforcement learning;
- database systems and repair;
- formal methods;
- programming languages;
- psychometrics and measurement theory;
- information retrieval;
- software testing and fault localization;
- reliability engineering.

### Layer 6 — Older and foundational literature

Remove foundation-model and contemporary agent terminology. Search the abstract scientific problem historically.

Purpose: identify established methods being rediscovered under new language.

### Citation-chain expansion

For the strongest apparent threats, inspect:

- foundational references they build on;
- later work that cites or extends them;
- related-work clusters;
- benchmark, code, or system successors.

The reviewer must document which layers were applicable and which were omitted, with justification.

## 10. Search audit trail, Phase 1 adequacy, and saturation

### 10.1 Search audit trail

Each candidate must include a search audit table:

| Search layer | Concepts or query families | Sources or databases searched | Hits screened | Sources inspected beyond abstract | New collision class found? | Notes |
|---|---|---|---:|---:|---|---|

The audit need not preserve every literal query string, but must be specific enough for another reviewer to reconstruct the strategy and identify missing methodological neighborhoods.

Search breadth is not measured by raw paper count. A small set of decisive papers in the correct lineage is more valuable than a large collection of topically related papers.

### 10.2 Phase 1 minimum adequacy

For every candidate, the independent fatal-risk scan must include:

1. a completed search concept map;
2. an initial attempt at every applicable search layer;
3. inspection of dangerous prior art inherited from Day 1 and the Candidate Evaluation Packet;
4. screening of newly surfaced direct threats;
5. relevant-sections inspection of at least the most consequential accessible threat where one exists;
6. an assessment of all six kill tests and both stress tests, unless early stopping is justified;
7. explicit `UNRESOLVED` labels where evidence is insufficient;
8. one cheapest discriminating test;
9. one concrete next-evidence request.

Phase 1 establishes broad fatal-risk coverage. It does not need to establish deep-search saturation for every candidate.

### 10.3 Deep-search saturation

Deep-search saturation is normally pursued during Phase 3 for uncertainties capable of changing candidate survival.

A search may be considered saturated for the current deep task only when:

1. all applicable search layers have been attempted;
2. direct synonyms and concept-level synonyms have both been used;
3. the most dangerous apparent collisions have been inspected beyond metadata and, when decision-critical, beyond abstract;
4. parent-discipline searching has been performed where applicable;
5. backward or forward citation chaining has been performed for the strongest threats where accessible;
6. two consecutive meaningful query reformulations or citation expansions produce no new thesis-relevant collision class;
7. unresolved but potentially consequential sources are logged;
8. additional searching is unlikely to change the candidate's phase outcome, confidence, critical uncertainty, or next scientific action.

Failure to reach saturation makes the relevant **search-coverage or collision judgment** unresolved. It makes the entire candidate outcome `UNRESOLVED` only when the unsaturated area could plausibly conceal a fatal result.

## 11. Prior-art collision relevance, overlap assessment, and dispositions

### 11.1 Stage A — Relevance screening

A source advances to collision assessment only if it addresses at least one thesis-defining component:

- central scientific object;
- central scientific problem;
- formal representation;
- method or learning objective;
- falsifiable thesis;
- decisive experiment;
- evaluation methodology.

Similarity based only on the same model family, dataset, domain, or generic words such as “agent,” “evaluation,” or “trustworthy” is insufficient.

The phrase **irrelevant collision** should not be used. A source irrelevant to novelty is an **out-of-scope hit** or **non-colliding related work**.

### 11.2 Dimension-level contribution-overlap scale

The contribution-overlap matrix uses these dimension-level ratings:

#### NONE

No substantive overlap in the dimension being evaluated.

#### PARTIAL

The prior work contains a recognizable component or subproblem, but an independent thesis-defining contribution remains.

#### STRONG

The prior work contains most of the candidate's contribution on that dimension and materially narrows the remaining novelty claim.

#### NEAR-IDENTICAL

The prior work contains substantially the same object, formulation, method, or decisive experiment; remaining differences are primarily implementation, dataset, model, scale, or domain.

These ratings apply to individual dimensions. They are not final collision dispositions and must not be mechanically summed.

### 11.3 Stage B — Contribution-overlap matrix

Every serious collision candidate must be compared using:

| Dimension | None | Partial | Strong | Near-identical | Evidence and citation |
|---|---:|---:|---:|---:|---|
| Falsifiable thesis | | | | | |
| Central scientific object | | | | | |
| Formal representation | | | | | |
| Method or learning objective | | | | | |
| Decision or output behavior | | | | | |
| Decisive experiment | | | | | |
| Evaluation methodology | | | | | |
| Domain or dataset | | | | | |

The dimensions are not equally important. The default priority is:

`falsifiable thesis > scientific object > methodological contribution > decisive experiment > evaluation > domain/dataset/tool similarity`

No automatic numerical sum should determine collision severity.

### 11.4 Collision dispositions

#### OUT-OF-SCOPE HIT

Similarity is superficial or unrelated to the thesis-defining contribution.

#### NON-COLLIDING RELATED WORK

Scientifically relevant background, benchmark, or supporting work that does not materially reduce novelty.

#### PARTIAL COLLISION

Overlaps one or more substantive components and narrows the novelty claim, while leaving an independent central contribution.

#### MAJOR COLLISION

Overlaps enough of the object, method, thesis, or decisive experiment that substantial narrowing or reformulation is required.

#### POTENTIALLY FATAL COLLISION

Available evidence suggests the dissertation contribution may already substantially exist or be a strict subset of prior work. Final classification requires sufficient source inspection.

#### FATAL COLLISION CONFIRMED

Sufficiently inspected prior work contains substantially the same central scientific object and methodological contribution, or a strict superset, and tests substantially the same thesis or decisive experiment. The remaining difference is not independently dissertation-level.

This disposition requires:

1. primary-source inspection beyond metadata and normally beyond abstract;
2. a completed contribution-overlap matrix;
3. examination of material contradictory evidence;
4. an explicit explanation of why narrowing cannot preserve the original candidate identity.

A confirmed fatal collision maps to `KT1 — FATAL CONFIRMED`.

#### UNRESOLVED COLLISION

Available source access or methodological detail is insufficient for reliable classification.

### 11.5 Default fatal-collision condition

A novelty collision is normally fatal when:

1. prior work contains substantially the same central scientific object;
2. it uses substantially the same methodological contribution or a strict superset;
3. it tests substantially the same thesis or decisive experiment;
4. the remaining delta is primarily healthcare application, dataset substitution, model replacement, interface design, or implementation scale.

A fatal collision defeats the candidate **as currently formulated**. It may motivate a narrower or redefined candidate, which must be handled separately.

---

# Part IV — Scientific tests and judgment rubrics

## 12. Six kill tests

Each kill test must record:

`question -> required evidence -> failure condition -> non-failure interpretation -> current status -> severity -> confidence`

### KT1 — Novelty collision

**Question:** Does substantially equivalent prior work already exist?

**Required evidence:** layered search, citation-chain review, and contribution-level comparison of dangerous prior work.

**Failure condition:** the central object, method, or thesis substantially exists and the remaining delta is mainly application or implementation.

**Non-failure means:** no investigated work currently defeats the novelty case at the documented search depth.

**Non-failure does not mean:** global novelty has been proved.

### KT2 — Dissertation coherence

**Question:** Do all proposed aims test one falsifiable dissertation thesis?

**Required evidence:** a thesis-to-aim map:

| Aim | Scientific question | Thesis clause tested | Evidence produced | Dependency on other aims |
|---|---|---|---|---|

**Failure condition:** aims require independent theses or merely share a domain, tool, or fashionable theme.

**Non-failure means:** one coherent dissertation architecture is plausible.

### KT3 — Ground truth and identifiability

**Question:** Can the target state, label, causal attribution, or evaluation criterion be known with sufficient validity?

**Required evidence:** construct definition, annotation protocol, adjudication process, inter-rater reliability, simulation truth, causal assumptions, validation strategy, or partial-identification argument.

**Failure condition:** the primary outcome cannot be distinguished from annotation convention, hindsight, leakage, circular model judging, or an unobservable construct.

**Non-failure means:** a defensible ground-truth, reference-standard, or partial-identification strategy exists.

### KT4 — Simpler-baseline necessity

**Question:** Does the proposed complexity solve something that strong simple rules, checklists, thresholds, standard models, or deterministic methods cannot?

**Required evidence:** conceptual baseline analysis and, where feasible, matched comparison controlling data, model access, action budget, compute, and evaluation.

**Failure condition:** a simple baseline provides practically equivalent thesis-relevant performance while requiring materially less complexity, data, computation, annotation, or operational burden.

Statistical non-significance does not establish equivalence. Practical equivalence must use a candidate-specific, prospectively justified equivalence or non-inferiority criterion. The comparison must consider thesis-relevant dimensions such as:

- average predictive performance;
- calibration;
- robustness and distribution shift;
- clinically weighted error;
- action cost and human workload;
- computation;
- interpretability;
- generalization.

No universal numerical margin is imposed, but the margin and its rationale must be specified before the result is interpreted.

**Non-failure means:** meaningful headroom over strong simpler alternatives remains plausible or demonstrated.

### KT5 — Feasibility and dependency failure

**Question:** Can the central thesis be tested during the PhD using available or realistically obtainable resources?

**Required evidence:** a dependency graph covering data, ground truth, annotation, compute, software infrastructure, expertise, governance, collaborators, and time.

Every dependency must receive two separate classifications.

#### Availability

- **GREEN:** available or under direct control;
- **YELLOW:** realistically obtainable through a credible path;
- **RED:** uncertain, externally controlled, or unlikely.

#### Thesis criticality

- **CORE:** the central thesis cannot be tested validly without it;
- **SUPPORTING:** it materially improves the dissertation, but a valid fallback exists;
- **OPTIONAL:** it is a useful extension but not required for the scientific case.

The dependency table must record:

| Dependency | Availability | Criticality | Owner or gatekeeper | Expected decision point | Fallback | Consequence if unavailable |
|---|---|---|---|---|---|---|

**Failure condition:** the central claim depends on an uncontrolled and unlikely `RED + CORE` resource with no scientifically valid fallback, or on an equivalent dependency configuration that makes the thesis infeasible.

**Non-failure means:** an executable minimum path and fallback architecture exist.

### KT6 — Technological and foundation-model resilience

**Question:** Does the contribution remain meaningful if foundation models and tooling improve substantially during the PhD?

**Required evidence:** explicit separation of structural problem from current capability deficiency, plus analysis of which artifacts or claims survive model replacement.

**Failure condition:** ordinary model progress eliminates the core problem or reduces the dissertation to obsolete prompting, orchestration, or interface engineering.

**Non-failure means:** a durable representation, theory, algorithm, contract, evaluation method, or structural problem remains.

## 13. Two non-kill stress tests

### ST1 — Dissertation-sized depth

**Question:** Does the direction support multiple coherent investigations under one thesis?

This test asks whether multiple scientifically distinct experiments can test different clauses, mechanisms, boundary conditions, or validation domains of one central claim. It does not ask whether three papers can be manufactured.

Allowed outcomes:

- **CLEARLY DISSERTATION-SIZED**
- **PLAUSIBLY DISSERTATION-SIZED**
- **POSSIBLY ONE STRONG PAPER**
- **UNRESOLVED**

A “possibly one strong paper” result is material but not automatically fatal. It becomes fatal when no coherent dissertation-scale expansion exists without changing the scientific identity.

### ST2 — Generalizability

**Question:** Does the contribution extend beyond one disease, dataset, institution, model, or local workflow without losing its identity?

Allowed outcomes:

- **METHODOLOGICALLY GENERAL**
- **GENERALIZABLE WITH EXPLICIT BOUNDARY CONDITIONS**
- **APPLICATION-BOUND**
- **UNRESOLVED**

Application-bound work is not automatically invalid when healthcare-specific structure is itself the scientific contribution. The reviewer must explain what transfers and what remains domain-specific.

## 14. Weakness-severity and confidence rubrics

### 14.1 Weakness severity

#### FATAL

Confirmed evidence defeats the central thesis or requires replacing the candidate's scientific identity.

#### MATERIAL

Requires meaningful narrowing, methodological revision, or dependency mitigation while preserving the central identity.

#### MINOR

Important implementation, reporting, or evaluation issue that does not threaten the central thesis.

#### UNRESOLVED SEVERITY

Evidence is insufficient to determine whether the weakness is fatal, material, or minor.

### 14.2 Confidence

#### HIGH CONFIDENCE

Multiple appropriate sources converge, decisive sources were inspected sufficiently deeply, and little outcome-relevant ambiguity remains.

#### MODERATE CONFIDENCE

Evidence leans clearly one way, but one or more meaningful uncertainties remain.

#### LOW CONFIDENCE

The judgment depends substantially on incomplete source access, abstract-only evidence, narrow search coverage, indirect inference, or unresolved methodological ambiguity.

Confidence measures confidence in the **judgment**, not enthusiasm for the candidate. `FAILS AS CURRENTLY FORMULATED — HIGH CONFIDENCE` and `SURVIVES — LOW CONFIDENCE` are both coherent.

## 15. Candidate-level falsification outcomes

### SURVIVES

No investigated kill test materially defeats the candidate as currently formulated at the completed phase's search depth.

This does not mean globally novel, proven correct, selected as a finalist, or strategically preferred.

### SURVIVES WITH MATERIAL REVISION

The central identity remains scientifically defensible, but explicit narrowing or revision is required.

The artifact must state:

- the required revision;
- why it preserves the identity;
- which kill test triggered it;
- what remains to verify.

### UNRESOLVED

At least one potentially fatal uncertainty remains and available evidence is insufficient for a defensible survival or failure judgment.

The artifact must state the unresolved question and next evidence required.

### FAILS AS CURRENTLY FORMULATED

Confirmed evidence defeats the dissertation-level scientific case or requires replacing the central object or thesis.

Reopening requires materially new evidence or explicit redefinition as a new candidate.

### Kill-test status vocabulary

Each individual kill test should use one of:

- **NO FATAL FAILURE IDENTIFIED**
- **MATERIAL CONCERN**
- **POTENTIALLY FATAL**
- **FATAL CONFIRMED**
- **UNRESOLVED**
- **NOT REACHED DUE TO EARLY STOPPING**

---

# Part V — Decision-enabling evidence

## 16. Cheapest discriminating test or experiment

The **cheapest discriminating test or experiment** is the lowest-burden feasible procedure whose plausible outcomes would substantially update the candidate's scientific status.

It may be:

- full-text contribution comparison;
- small annotation pilot;
- simulation;
- mathematical counterexample;
- implementation of one dangerous baseline;
- ablation;
- expert feasibility assessment;
- data-access verification.

Required fields:

| Field | Required content |
|---|---|
| Decision question | The exact uncertainty being tested |
| Procedure | The steps to perform |
| Inputs | Required papers, data, compute, software, or expertise |
| Strengthening outcome | Result that sustains or strengthens the candidate |
| Weakening/failure outcome | Result that materially weakens or kills it |
| Estimated burden | Time, compute, money, annotation, access, and coordination |
| Why cheapest | Why this test offers high information per unit effort |

“Cheapest” means lowest combined burden, not lowest financial cost alone.

## 17. Next evidence required

**Next evidence required** is the smallest specific evidence package needed to resolve the candidate's most decision-relevant remaining uncertainty.

Every request must specify:

1. **Evidence object:** what document, dataset, experiment, annotation, proof, expert assessment, or implementation result is needed.
2. **Acquisition procedure:** how it will be obtained or produced.
3. **Uncertainty addressed:** which claim or kill test it resolves.
4. **Decision consequence:** how alternative outcomes change the candidate status.
5. **Completion criterion:** what constitutes enough evidence to close the request.

### Inadequate examples

> More research is required.

> Investigate whether the method is novel.

### Concrete literature example

> Inspect the methods and supplementary material of the three closest constraint-induction papers and compare constraint representation, applicability conditions, exception handling, and repair operation. If a prior method contains all four and evaluates semantic repair fidelity, reclassify the collision as major or potentially fatal. The request is complete when each paper has a contribution-overlap matrix and inspection-depth record.

### Concrete empirical example

> Have two qualified reviewers independently annotate a pilot set of longitudinal cases using the proposed diagnostic-state ontology. Estimate agreement for state-at-time and transition labels. If agreement is insufficient for the intended reference-standard use, redesign the construct before corpus expansion. The request is complete when the annotation protocol, adjudicated labels, agreement analysis, and redesign decision are documented.

The protocol does not impose one universal numerical threshold. Any threshold must be justified for the construct, decision, and phase.

## 18. Decision-update and early-stopping rules

### 18.1 Default kill hierarchy

The default triage order is:

`novelty -> coherence -> ground truth -> simpler baseline -> feasibility -> technological resilience`

Rationale:

- if the contribution already exists, later engineering analysis is wasteful;
- if the thesis is incoherent, experiment optimization is premature;
- if the target cannot be measured, sophisticated methods cannot rescue validity;
- if a simple method solves the problem, complexity lacks justification;
- only then is detailed resource planning worthwhile;
- resilience determines whether the surviving direction remains meaningful over the PhD horizon.

The order may be changed when another fatal dependency is cheaper to resolve first. The deviation must be justified.

### 18.2 Early stopping

A confirmed fatal result permits early stopping for the candidate in the current phase when:

1. the decisive evidence is cited and inspected sufficiently deeply;
2. the fatality reasoning is explicit;
3. unresolved contradictory evidence is recorded;
4. later tests are marked `NOT REACHED DUE TO EARLY STOPPING`;
5. a possible material revision or redefinition is distinguished from survival of the original candidate.

### 18.3 No score averaging

Kill-test outcomes, confidence, and source counts must not be averaged into a pseudo-precise numerical score. One high-confidence fatal failure can outweigh several nonfatal strengths.

### 18.4 Evidence update rule

When new evidence arrives, update:

`claim status -> kill-test status -> weakness severity -> confidence -> candidate outcome -> next action`

The artifact must state which link changed and why.

### 18.5 Redefinition rule

If survival requires replacing the central scientific object or thesis, the original candidate is `FAILS AS CURRENTLY FORMULATED`. The proposed replacement must be recorded as a redefined candidate and pass a human checkpoint before entering later analysis.

---

# Part VI — Multi-agent workflow

## 19. Six-phase workflow, transition gates, and role assignment

Phases 1 through 5 constitute adversarial scientific falsification. Phase 6 is the downstream strategic handoff.

### Phase 1 — Independent fatal-risk scan

**Question:** What could kill each of the eight candidates?

All three streams independently evaluate all eight approved Candidate Evaluation Packets using the six kill tests and two stress tests.

Rules:

- external research is allowed;
- each stream uses the same Phase 1 schema;
- each stream evaluates the same packet version for every candidate;
- other streams' Phase 1 outputs are prohibited until all are frozen;
- each candidate receives the Phase 1 minimum-adequacy scan;
- dangerous sources are inspected deeply enough to determine whether a fatal risk is plausible;
- candidate-definition disagreements are disclosed rather than resolved silently;
- one frozen artifact is produced per stream.

**Transition gate:** all three artifacts are frozen, source lists resolve, packet versions match, and no stream has seen another's Phase 1 conclusions.

### Phase 2 — Reconciliation

**Question:** Where do the independent reviews agree or disagree, and what causes the disagreement?

Classify each disagreement as:

- factual disagreement;
- source-coverage disagreement;
- source-inspection-depth disagreement;
- source-interpretation disagreement;
- threshold disagreement;
- candidate-definition disagreement;
- confidence disagreement.

No majority voting. The reconciliation should identify which disagreements require deeper evidence.

**Transition gate:** every disagreement has a type, consequence, and concrete next-evidence request or reason for closure.

### Phase 3 — Targeted deep falsification

**Question:** Can the decision-relevant unresolved questions be resolved?

Possible assignments include:

- full-text novelty audits;
- parent-discipline searches;
- dangerous-baseline implementation;
- annotation or measurement pilots;
- causal or statistical analysis;
- data-access or governance verification;
- expert review.

Not every candidate receives equal additional computation. Deep-search saturation is pursued only where it can materially change candidate status or confidence.

**Transition gate:** targeted tasks reach their stopping condition, update the relevant kill tests, and identify candidates requiring cross-examination.

### Phase 4 — Cross-examination

**Question:** Does the candidate survive the strongest evidence-based rejection case?

Roles:

1. **Prosecutor:** constructs the strongest scientifically defensible rejection case.
2. **Defense reviewer:** answers each allegation and cited source specifically; generic advocacy is insufficient.
3. **Adjudicator:** evaluates both records and the underlying evidence.

No system should act as both prosecutor and adjudicator for the same candidate. Roles should rotate to reduce systematic bias.

**Transition gate:** prosecution, defense, and adjudication artifacts are complete for every candidate assigned to cross-examination.

### Phase 5 — Scientific survivor freeze

**Question:** Which scientifically viable candidates remain?

For each survivor, record:

- exact surviving identity and thesis;
- required material revisions;
- resolved kill tests;
- unresolved but nonfatal risks;
- candidate-level outcome and confidence;
- evidence provenance;
- cheapest next empirical test where relevant.

User approval is required before freezing the scientifically viable set.

### Phase 6 — Strategic optimization

**Question:** Among scientifically viable directions, which best serves the broader objectives?

Only here may the analysis incorporate:

- publication and citation potential;
- advisor configuration;
- durable technical skill formation;
- frontier-artificial-intelligence and quantitative-research portability;
- reusable artifact and adoption potential;
- commercialization;
- specialized-visa-relevant output characteristics;
- broader career goals.

The detailed private strategic layer should not be placed automatically in the public repository.

### Phase-specific schemas

Each phase must use a dedicated schema stored under `analysis/schemas/`. The protocol defines invariant semantics; the schemas define exact headings, tables, required fields, and deterministic checks.

---

# Part VII — Scientific integrity and information flow

## 20. Strategic-contamination firewall

During Phases 1 through 5, the following must not save or kill a scientific direction:

- compensation;
- employer desirability;
- frontier-lab fashion;
- quantitative-finance recruiting;
- immigration planning;
- commercialization;
- startup upside;
- prestige;
- personal excitement;
- fashionable terminology.

Permitted scientific considerations include advisor-method fit, resource feasibility, dissertation depth, data access, methodological transfer, and resilience to technological change.

Every scientific verdict should pass this contamination check:

> Would the scientific verdict change if the direction had no unusual career, immigration, prestige, or commercial value?

If yes, the reviewer must explain why the consideration is genuinely scientific or revise the judgment.

## 21. Stream independence, information flow, privacy, human checkpoints, and artifact integrity

### 21.1 Information flow by phase

- **Phase 1:** blind across streams.
- **Phase 2:** all frozen Phase 1 outputs become readable.
- **Phase 3:** targeted assignments may use the reconciliation artifact.
- **Phase 4:** prosecution precedes defense; adjudication follows both.
- **Phase 5:** all scientific evidence may be synthesized.
- **Phase 6:** scientific survivor records may be combined with private strategic analysis under separate visibility controls.

### 21.2 Independence disclosure

Every artifact must state:

- which other-stream artifacts were read;
- when they were read;
- any accidental exposure;
- whether exposure occurred before or after the stream's independent judgment was frozen;
- whether the exposure changed the analysis.

### 21.3 Human checkpoints

Stop for user approval before:

- redefining a candidate's central object or thesis;
- freezing or materially changing a Candidate Evaluation Packet;
- freezing the scientific survivor set;
- resolving an evidence conflict that materially changes candidate status when provenance remains disputed;
- exposing private or restricted evidence;
- changing this protocol materially;
- proceeding when institutional, legal, privacy, or governance constraints are uncertain.

This extends the checkpoint rules in [`OPERATING_PROTOCOL.md`](../OPERATING_PROTOCOL.md).

### 21.4 Privacy and public-repository safeguards

Do not commit:

- protected health information;
- restricted clinical text or screenshots;
- credentials;
- sensitive institutional identifiers;
- small-cell or enclave results;
- private immigration, wealth, employer, or startup strategy;
- private assessments of named individuals.

Use sanitized evidence identifiers and private records where necessary.

### 21.5 Artifact integrity

- earlier frozen artifacts remain immutable;
- corrections are added as explicit metadata/provenance revisions;
- scientific reconsideration occurs in new artifacts;
- exact candidate-packet version and repository commit must be recorded;
- normalization, falsification, and strategic analysis must not be silently conflated.

---

# Part VIII — Repository and protocol governance

## 22. Repository execution rules, protocol authority, versioning, and amendment control

### 22.1 Execution contract for each substantial task

Before execution, state:

- objective;
- branch and base commit;
- candidate and Candidate Evaluation Packet version;
- files and sources to read;
- files and sources deliberately excluded;
- whether external research is allowed;
- whether parallelism is justified;
- expected artifact;
- stopping condition.

### 22.2 Repository rules

- create an isolated branch from the approved base;
- add only phase-local artifacts;
- do not overwrite frozen records;
- do not modify `decisions/`, shared literature, evidence, candidate definitions, or `main` unless explicitly authorized;
- exclude `.DS_Store` and unrelated files;
- run deterministic changed-file and identifier checks;
- commit locally;
- do not push or merge until user review;
- preserve provider-neutral wording in public artifacts.

### 22.3 Citation audit before freezing

Verify:

1. every source identifier resolves to a source record or local source entry;
2. every source-derived decision-relevant claim is cited at point of use;
3. numerical claims and quotations are cited specifically;
4. cross-paper syntheses cite all load-bearing sources;
5. search non-findings point to the search audit;
6. inspection-depth labels match what was actually read;
7. abstract-only evidence is not treated as a confirmed fatal collision without qualification;
8. mutable sources record version and access date where applicable;
9. no blind stream independently assigns a new permanent `LIT-###` identifier;
10. internal project-state claims cite the relevant artifact or commit;
11. no restricted or private information is exposed.

Deterministic scripts may check malformed DOI, PMID, arXiv, local-source, or internal-path references. Human review remains necessary for citation correctness.

### 22.4 Future citation-usage ledger

A later `citations/` layer may record where and why sources were used without duplicating the canonical bibliography.

Proposed division:

```text
literature/records/   What is this source?
citations/            Where, why, and how was this source used?
```

A future usage ledger may include:

| Field | Purpose |
|---|---|
| Source identifier | Permanent, provisional, restricted, or internal provenance identifier |
| Full citation or source-record link | Human-readable source identity |
| Stable identifier or link | DOI, PMID, proceedings identifier, arXiv, or official URL |
| Source version and access date | Mutable-source provenance |
| Phase and stream | Origin of the citation use |
| Repository artifact | Exact file path |
| Section or claim | Location of use |
| Citation role | Dangerous prior art, baseline, problem evidence, and so forth |
| Why cited | Specific function of the source |
| Evidentiary status | Direct finding, synthesis, hypothesis, non-finding, unresolved |
| Inspection depth | Metadata through reproduction |
| Decision consequence | Kill test, confidence, or candidate decision affected |
| Visibility | Public, sanitized, private, or restricted |
| Last verified | Date and repository commit where useful |

The usage ledger is deferred. This protocol requires enough citation provenance now that it can be generated later without reconstructing the project from memory.

### 22.5 Protocol authority

This document is:

1. linked from `analysis/README.md`;
2. adopted through **DEC-009** in `decisions/decision_log.md`;
3. canonical for Phases 1 through 5 and the Phase 6 handoff;
4. materially changeable only with user approval and a corresponding decision-log update.

### 22.6 Versioning

- **v0.1:** conceptual design covering kill tests, stress tests, phases, and basic evidence rules.
- **v0.2:** corrected eight-part, twenty-two-section architecture; detailed search/collision methodology; citation integrity; source roles; provisional source identifiers; future citation-usage ledger design.
- **v1.0:** first approved canonical version; adds common Candidate Evaluation Packets, operational overlap ratings, confirmed-fatal-collision semantics, Phase 1 minimum adequacy versus deep saturation, baseline-equivalence rules, two-axis dependency assessment, and mutable-source provenance.

Material changes alter definitions, decision thresholds, information flow, scientific outcomes, candidate-packet semantics, or phase gates. Editorial clarifications that preserve meaning may be recorded as metadata-only or wording-only revisions, with explicit provenance.

---

# Compact protocol summary

The adversarial falsification workflow is:

`approved Candidate Evaluation Packet -> layered search -> collision assessment -> six kill tests -> two stress tests -> cheapest discriminating test -> next evidence required -> independent phase outcome -> reconciliation -> deep falsification -> cross-examination -> scientific survivor freeze -> strategic optimization`

The governing rule is:

> Standardize the scientific instrument and target, preserve independent reasoning, cite every decision-relevant source-derived claim, and stop only when additional work is unlikely to change the scientific decision or next action.

**STATUS: CANONICAL — ADOPTED THROUGH DEC-009. Phase 1 may begin only after the Phase 1 schema and all eight Candidate Evaluation Packets are approved.**