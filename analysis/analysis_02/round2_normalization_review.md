# Round 2 — Independent Adversarial Review of Cross-Stream Candidate Normalization

- **Date:** 2026-08-31
- **Analysis stream:** `analysis_02`
- **Branch:** `codex/analysis02-round2-normalization-review`
- **Canonical base SHA:** `4deee8eb8425b22e9532f1f3afd74791ef3e422c`
- **Status:** **FROZEN — ROUND 2 INDEPENDENT NORMALIZATION REVIEW**
- **Question evaluated:** Which of the 12 frozen Day 1 candidates are the same underlying dissertation research direction, which partially overlap, and which are genuinely distinct?
- **Inputs read:** `analysis/analysis_01/day1_candidate_generation_v2.md`; `analysis/analysis_02/day1_candidate_generation_v2.md`; `analysis/analysis_03/day1_candidate_generation_v2.md`; `analysis/COMMON_ANALYSIS_SCHEMA.md`; `analysis/README.md`; `OPERATING_PROTOCOL.md`; and the coordinator's Round 1 hypothesis supplied in the task specification.
- **Deliberately excluded:** historical candidate rankings; non-v2 Day 1 artifacts; historical discussion streams; literature records and original publications; every other Round 2 response or normalization review; candidate quality scores; strategic criteria.
- **External research:** none. No new literature search or source retrieval was performed.
- **Parallelism:** none. One reviewer applied one identity standard to all 66 non-diagonal candidate pairs.
- **Independence disclosure:** no Stream 01 or Stream 03 Round 2 review was read. The coordinator proposal was treated as a hypothesis to attack, not an answer key.
- **Stopping condition:** stop after the symmetric 12 × 12 matrix, N1–N7 audits, three required uncertainty attacks, missed-relationship audit, independent normalized set, disagreement ledger, and merge-coherence audit are complete.

This review concerns candidate identity only. `SAME DIRECTION` does not imply scientific strength, `DISTINCT` does not imply weakness, and convergence count is not evidence of quality.

## 1. Candidate key

| Abbreviation | Frozen Day 1 candidate |
|---|---|
| `1C1` | Stream 01 C1 — Evidence-State Control for Selective Clinical AI Agents |
| `1C2` | Stream 01 C2 — Temporally Constrained Diagnostic-State Reasoning from Longitudinal EHRs |
| `1C3` | Stream 01 C3 — Data-Fitness-Aware Autonomous Target-Trial Emulation |
| `1C4` | Stream 01 C4 — Process-Aware Dynamic Assurance and Failure Localization for Clinical AI Agents |
| `2D1` | Stream 02 D02-01 — Dual-clock Evidence-State Control for Longitudinal Clinical Agents |
| `2D2` | Stream 02 D02-02 — Learned Temporal Clinical Constraints for Auditable Representation Repair |
| `2D3` | Stream 02 D02-03 — Machine-Checkable Causal Data-Fit Contracts for EHR Target-Trial Emulation |
| `2D4` | Stream 02 D02-04 — Change-Attributed Continual Assurance for Clinical Foundation-Model Systems |
| `3C1` | Stream 03 C1 — Adequacy-Aware Verification of Clinical AI Claims |
| `3C2` | Stream 03 C2 — Diagnostic-State Trajectories from Longitudinal Clinical Records |
| `3C3` | Stream 03 C3 — Selective Control for Clinical Language Systems under Asymmetric Risk |
| `3C4` | Stream 03 C4 — Measurement Error in Clinical NLP Evaluation |

## 2. Conceptual relationship matrix

The diagonal is self-identity. Every one of the 66 non-diagonal pairs uses exactly one required relationship label. `PARTIAL OVERLAP` means that a substantive object, aim, or evaluation layer is shared, but one thesis cannot encompass both candidates without either narrowing one or broadening the dissertation artificially. Mere compatibility or reuse of another candidate's artifact is not enough by itself.

| ID | 1C1 | 1C2 | 1C3 | 1C4 | 2D1 | 2D2 | 2D3 | 2D4 | 3C1 | 3C2 | 3C3 | 3C4 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1C1 | — | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | SAME DIRECTION | PARTIAL OVERLAP | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | SAME DIRECTION | DISTINCT |
| 1C2 | PARTIAL OVERLAP | — | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT | SAME DIRECTION | PARTIAL OVERLAP | PARTIAL OVERLAP |
| 1C3 | DISTINCT | DISTINCT | — | DISTINCT | DISTINCT | DISTINCT | SAME DIRECTION | DISTINCT | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT |
| 1C4 | PARTIAL OVERLAP | DISTINCT | DISTINCT | — | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | DISTINCT | DISTINCT | PARTIAL OVERLAP | DISTINCT |
| 2D1 | SAME DIRECTION | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | — | PARTIAL OVERLAP | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | SAME DIRECTION | DISTINCT |
| 2D2 | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | — | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT |
| 2D3 | DISTINCT | DISTINCT | SAME DIRECTION | DISTINCT | DISTINCT | DISTINCT | — | DISTINCT | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT |
| 2D4 | DISTINCT | DISTINCT | DISTINCT | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT | — | DISTINCT | DISTINCT | DISTINCT | PARTIAL OVERLAP |
| 3C1 | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | — | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP |
| 3C2 | PARTIAL OVERLAP | SAME DIRECTION | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT | — | PARTIAL OVERLAP | PARTIAL OVERLAP |
| 3C3 | SAME DIRECTION | PARTIAL OVERLAP | DISTINCT | PARTIAL OVERLAP | SAME DIRECTION | PARTIAL OVERLAP | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | — | DISTINCT |
| 3C4 | DISTINCT | PARTIAL OVERLAP | DISTINCT | DISTINCT | DISTINCT | DISTINCT | DISTINCT | PARTIAL OVERLAP | PARTIAL OVERLAP | PARTIAL OVERLAP | DISTINCT | — |

### Same-direction pair types

- `1C1` ↔ `2D1`: **SAME DIRECTION — strict scoped specialization.** `1C1` is the broader typed-evidence-state/control formulation; `2D1` specializes it to persistent longitudinal belief management with separate patient-event and evidence-validity clocks.
- `1C1` ↔ `3C3`: **SAME DIRECTION — competing and complementary formulations.** Both test whether explicit non-scalar state/signals improve multi-action selective control. They compete on the state variables and task domain; `3C3` contributes asymmetric-cost and risk-control specificity.
- `2D1` ↔ `3C3`: **SAME DIRECTION — complementary formulations.** The dual-clock representation and task-structural failure predictors are alternative structured inputs to the same cost-sensitive action policy, not independent dissertation theses.
- `1C2` ↔ `3C2`: **SAME DIRECTION — complementary formulations.** They share the diagnostic-state trajectory as the scientific object. Temporal transition constraints and resolving-event/annotation/validation machinery are different operationalizations of the same representational thesis.
- `1C3` ↔ `2D3`: **SAME DIRECTION — complementary formulations.** Both ask whether an executable representation of target-trial data fitness can detect unsupported designs and revise, restrict, or refuse them. `2D3` is the more formal contract/compiler formulation; `1C3` is the more agentic workflow formulation.

No other pair preserves both the central scientific object and the falsifiable thesis closely enough for `SAME DIRECTION`.

## 3. Audit of the coordinator's N1–N7 proposal

### N1 — Evidence-State and Selective Control for Clinical AI

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** `1C1`, `2D1`, and `3C3` all contribute a structured, non-scalar representation of why an output may be unsafe or incomplete and a cost-sensitive controller choosing among multiple actions rather than only answer versus abstain.
2. **Scientific distinctions that would be lost by merging:** `1C1` emphasizes a general typed evidence state; `2D1` makes persistent belief revision and the patient-time/evidence-validity-time separation central; `3C3` emphasizes external task-structural predictors, formal risk control, extraction/generation tasks, and asymmetric human-workload costs.
3. **Can one thesis honestly encompass them?** Yes, if the thesis is stated at the state-to-action level: structured external evidence/failure state improves clinically costed multi-action control over scalar confidence and generic self-verification. It should not require every candidate's complete task suite.
4. **Can one coherent set of aims test it?** Yes: define and compare state/signal representations; learn and test the multi-action controller at matched cost; then test transfer under longitudinal and distributional shift. The signal families are competing hypotheses inside Aim 1, not separate projects.
5. **Recommended normalized formulation:** **Structured evidence-state selective control for clinical AI under asymmetric risk.** Preserve dual clocks and structural signals as named alternative formulations, not additive dissertation obligations.
6. **Confidence:** **MODERATE.** The identity is strong, but an overinclusive implementation could still become too broad.

### N2 — Longitudinal Diagnostic-State Trajectory Modeling

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** `1C2` and `3C2` treat patient-level diagnostic state and its evidence-conditioned transitions as the representation and evaluation unit, replacing endpoint diagnosis or per-mention assertion aggregation.
2. **Scientific distinctions that would be lost by merging:** `1C2` foregrounds normative temporal transition constraints and unsupported state changes; `3C2` foregrounds resolving events, disease-agnostic annotation, transition-aware metrics, and fidelity to expert cohort adjudication.
3. **Can one thesis honestly encompass them?** Yes: explicit diagnostic-state trajectory modeling should improve state-at-time and transition fidelity over snapshot or aggregation baselines. Constraints and resolving-event anchors are complementary mechanisms for testing that thesis.
4. **Can one coherent set of aims test it?** Yes: formalize and annotate trajectories; compare explicit trajectory models with snapshot/aggregation baselines; validate state and transition fidelity across conditions and, if available, adjudicated cohorts.
5. **Recommended normalized formulation:** **Diagnostic-state trajectory representation and inference from longitudinal clinical records.** Preserve the constraint-oriented and adjudication-oriented variants.
6. **Confidence:** **HIGH.** The objects, baselines, aims, and falsification conditions align closely.

### N3 — Data-Fitness-Aware Autonomous Target-Trial Emulation

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** `1C3` and `2D3` contribute an executable representation that maps a target-trial question and EHR data-generating process to supported design, restricted/revised estimand, request for information, or refusal.
2. **Scientific distinctions that would be lost by merging:** `1C3` emphasizes autonomous workflow validity and an agentic checker/reviser; `2D3` emphasizes typed contract semantics, a compiler, provenance, diagnostics, and the boundary between testable conditions and untestable causal assumptions.
3. **Can one thesis honestly encompass them?** Yes: explicit machine-checkable data-fitness reasoning should reduce false-supported emulations and estimand mismatch relative to direct automation and checklists.
4. **Can one coherent set of aims test it?** Yes: formalize contract/validity semantics; implement completion/check/restrict/refuse decisions; test end-to-end validity under controlled truth and multiple data environments.
5. **Recommended normalized formulation:** **Machine-checkable causal data-fitness contracts and selective automation for EHR target-trial emulation.** The contract/compiler should be the durable object; agentic translation is an interface or method variant.
6. **Confidence:** **HIGH.** The two candidates are near-isomorphic at the object, thesis, aim, and evaluation levels.

### N4 — Dynamic Continual Assurance and Failure Attribution

**ROUND 1 VERDICT: SPLIT**

1. **Scientific identity shared by the proposed members:** `1C4` and `2D4` both reject endpoint-only evaluation and use structured failure representations, controlled perturbations, and attribution to make clinical-AI assurance actionable.
2. **Scientific distinctions that would be lost by merging:** `1C4` localizes a causal failure step within one stochastic agent trajectory and tests whether repairing that step changes the outcome. `2D4` detects regressions across system releases, attributes them to changed components, and allocates a limited test budget. Their causal units, interventions, comparators, metrics, and time axes differ.
3. **Can one thesis honestly encompass them?** No. A claim that one hierarchical failure model can attribute both within-run step failures and across-release component changes would be a new, broader thesis not present in either frozen candidate.
4. **Can one coherent set of aims test it?** Not without placing process localization, counterfactual trajectory repair, versioned regression detection, sequential test allocation, and prospective monitoring beside one another. That is two methodological spines.
5. **Recommended normalized formulation:** split into **Process-level causal failure localization for clinical AI agents** (`1C4`) and **Versioned continual assurance with change attribution** (`2D4`). Record `PARTIAL OVERLAP`, not identity.
6. **Confidence:** **HIGH.** The discriminating experiments make the split decisive.

### N5 — Learned Temporal Clinical Constraints and Auditable Representation Repair

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** the singleton `2D2` learns applicability-scoped temporal/ontological constraints and uses them to localize violations and produce minimal, proof-carrying repairs.
2. **Scientific distinctions that would be lost by merging:** merging into N2 would lose the general constraint-induction, exception handling, violation localization, and repair-calculus thesis; N2's object is a diagnostic-state trajectory and its fidelity, not representation repair generally.
3. **Can one thesis honestly encompass the proposed member?** Yes, as written. It is a complete independent thesis.
4. **Can one coherent set of aims test that thesis?** Yes: formalize/measure violations; induce constraints and repair; test transfer and downstream effects.
5. **Recommended normalized formulation:** **Probabilistic clinical constraint induction and proof-carrying representation repair.** Keep separate from N2 while recording their overlap at the temporal-constraint layer.
6. **Confidence:** **HIGH.** The partial N2 overlap does not erase the distinct repair object.

### N6 — Adequacy-Aware Clinical Evidence Verification

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** the singleton `3C1` contributes a claim-evidence verification calculus, expert benchmark, and calibrated verifier over support, methodological adequacy, currency, and patient applicability.
2. **Scientific distinctions that would be lost by merging:** an N1 merge would subordinate evidence quality/currency formalization and verifier validity to controller performance. N1 does not require a new evidence-appraisal calculus; N6 does not require a general multi-action controller for its first two aims or core thesis.
3. **Can one thesis honestly encompass the proposed member?** Yes. The prevalence and detectability of adequacy/currency failures, and the verifier's calibrated advantage over entailment checking, form an independent falsifiable thesis.
4. **Can one coherent set of aims test that thesis?** Yes: measure the failure mass; build the verifier; evaluate enforcement. Aim 3 touches N1, but Aims 1–2 remain a defensible dissertation if gating adds little.
5. **Recommended normalized formulation:** **Adequacy- and currency-aware verification of clinical AI claims.** Treat its verifier output as a possible N1 state signal, not as proof that the directions are identical.
6. **Confidence:** **HIGH.** Upstream/downstream composability is not candidate identity.

### N7 — Measurement-Error-Aware Clinical NLP Evaluation

**ROUND 1 VERDICT: ACCEPT**

1. **Scientific identity shared by the proposed members:** the singleton `3C4` models error in the evaluation instrument itself, estimates artifact fractions, propagates measurement uncertainty into system comparisons, and validates corrected protocols.
2. **Scientific distinctions that would be lost by merging:** folding N7 into an assurance, verifier, or trajectory candidate would turn instrument validity into a support function for that system rather than the scientific phenomenon under study.
3. **Can one thesis honestly encompass the proposed member?** Yes. The thesis is that a material, quantifiable portion of reported error is measurement artifact and that correction changes conclusions while better matching expert adjudication.
4. **Can one coherent set of aims test that thesis?** Yes: quantify artifacts; correct and infer; validate the corrected instrument.
5. **Recommended normalized formulation:** **Measurement-error modeling and corrected inference for clinical NLP evaluation.** Keep independent, while exposing interfaces to benchmark-heavy families.
6. **Confidence:** **HIGH.** Its object and falsification test are unlike the systems it could evaluate.

## 4. Direct attacks on the three most uncertain Round 1 decisions

### 4.1 N1: evidence-state representation versus selective risk control

The strongest argument for splitting N1 is that `2D1` makes the dual-clock persistent belief representation itself a contribution, whereas `3C3` could succeed with ontology-consistency and retrieval-agreement features without a persistent evidence state. Conversely, the strongest argument for merging is that none of the three representations is justified independently of the same downstream test: does the representation improve a cost-sensitive choice among answer, retrieve/verify, revise/flag, ask, or defer over scalar confidence and self-verification?

**Judgment: SAME DIRECTION.** The state representation and risk-control policy are two linked parts of one falsifiable state-to-action thesis. They should separate only if later work elevates representation learning to a standalone scientific claim whose success does not depend on action selection. The normalized direction must treat typed evidence state, dual clocks, and task-structural signals as alternative formulations to compare—not require three full representation projects.

### 4.2 N4: process-level failure localization versus change-attributed continual assurance

`1C4` asks, “Which step in this execution caused the endpoint failure, and does repairing that step change the outcome?” `2D4` asks, “Which system change caused a new regression, and which tests should be run next under a budget?” A step intervention within one trajectory does not identify a version/component effect across releases; a version-factor comparison does not identify the critical action within a failed trajectory.

**Judgment: PARTIAL OVERLAP; SPLIT.** Shared failure ontologies and counterfactual designs can be reused, but the causal units and decisive experiments differ. A combined hierarchical attribution framework would be a new candidate direction, which this normalization review is not authorized to invent.

### 4.3 N6: independent verifier or N1 component

N6 can supply N1 with support, adequacy, currency, and applicability signals, and its enforcement aim already gates a generator on verifier output. That makes the interface real rather than cosmetic. But N6's core claim can be confirmed even if no multi-action controller is built: a new benchmark can show a failure mass invisible to entailment checking, and a calibrated verifier can detect it. N1 can likewise succeed using missingness, contradiction, tool reliability, or ontology consistency without solving evidence-quality appraisal.

**Judgment: PARTIAL OVERLAP; keep distinct.** N6 is an upstream verification direction with its own formalism, ground truth, baselines, and two self-sufficient aims. Incorporating all of N6 into N1 would create two central methodological objects rather than one.

## 5. Relationships the coordinator may have under-specified

| Relationship | Matrix judgment | Shared scientific zone | Why this does not justify a merge |
|---|---|---|---|
| N2 ↔ N5 | PARTIAL OVERLAP | Temporal state constraints, violation detection, longitudinal representations | N2 tests a diagnostic-state trajectory representation; N5 tests learned applicability-scoped constraints and proof-carrying repair. The latter can operate on the former but is not the same thesis. |
| N1 ↔ N6 | PARTIAL OVERLAP | Evidence-quality/currency signals, gating, retrieval/verification actions | N6's verifier is one possible N1 signal source; each direction has a self-sufficient object and decisive experiment. |
| N1 ↔ N2 | PARTIAL OVERLAP | Persistent state, evidence-conditioned transitions, unsupported revision | A diagnostic trajectory could be one patient-state substrate for a controller, but trajectory fidelity and action-policy utility are different outcomes. The overlap is strongest for `2D1` and weakest for extraction-centered `3C3`. |
| N1 ↔ N4 | Mixed: PARTIAL OVERLAP with `1C4`; DISTINCT from `2D4` | Runtime failure state and targeted correction for `1C4`; shared safety context only for `2D4` | Process localization can produce controller signals, but evaluation/intervention attribution is not runtime action selection. Versioned regression monitoring operates at a different lifecycle level. |
| N4 ↔ N7 | Mixed: `1C4` DISTINCT; `2D4` PARTIAL OVERLAP | `2D4` explicitly models adjudication uncertainty and judge drift in a repeated evaluation instrument | N7 studies measurement artifact as the phenomenon and ranking inference as the output. `2D4` treats measurement uncertainty as one nuisance inside change detection. |
| N6 ↔ N7 | PARTIAL OVERLAP | Expert benchmarks, verifier-evaluation validity, calibration against adjudication | N6 measures whether claims are adequately supported; N7 measures whether the scoring instrument itself mismeasures system error. N7 can audit N6 without becoming N6. |
| N3 ↔ N6 | PARTIAL OVERLAP | Machine-checkable adequacy judgments, provenance, selective refusal | N3 verifies whether data support a causal estimand; N6 verifies whether evidence supports a clinical claim. The causal semantics, unit of analysis, diagnostics, and validation targets differ. |
| N2 ↔ N7 | PARTIAL OVERLAP | Annotation schemes and transition-aware metrics whose validity must be established | N2 contributes a domain representation plus model; N7 contributes general measurement-error decomposition. Instrument auditing is not trajectory modeling. |
| N5 ↔ N6 | PARTIAL OVERLAP | Typed temporal/applicability rules, verification traces, unresolved outputs | N5 repairs structured clinical representations; N6 appraises claim-evidence relations. Their constraints and ground truths are not interchangeable. |
| N5 ↔ process-localization half of N4 | PARTIAL OVERLAP | Violation localization and targeted repair/intervention | N5 localizes representation inconsistency; `1C4` localizes a causal failure step in agent execution. Similar verbs do not erase different causal objects. |

Two cautions follow. First, `PARTIAL OVERLAP` should trigger interface and duplicate-aim review, not automatic merging. Second, a broad abstraction such as “systems that know when something is wrong” would erase the falsifiable units and is therefore not a valid normalized family.

## 6. Independently recommended normalized candidate set

This review recommends **eight** normalized families. The table is non-ordinal.

| Provisional normalized ID | Normalized title | Constituent original candidates | Central scientific object | Scientific boundary |
|---|---|---|---|---|
| `S02-NF1` | Structured Evidence-State Selective Control for Clinical AI | `1C1`, `2D1`, `3C3` | Structured evidence/failure state plus a clinically cost-sensitive multi-action controller | Includes state-to-action policies under heterogeneous uncertainty; excludes building a full evidence-adequacy verifier or lifecycle assurance system as a second thesis. |
| `S02-NF2` | Diagnostic-State Trajectory Representation and Inference | `1C2`, `3C2` | Patient-level diagnostic states, evidence-conditioned transitions, resolving events, and trajectory-aware models/metrics | Includes explicit longitudinal diagnostic belief trajectories; excludes general representation repair not tied to diagnostic-state fidelity. |
| `S02-NF3` | Machine-Checkable Causal Data-Fitness for Target-Trial Emulation | `1C3`, `2D3` | Executable causal data-fit contract/checker with restrict, revise, request-information, and refuse outcomes | Includes validity-aware selective automation before estimation; excludes generic clinical claim verification and generic causal code generation. |
| `S02-NF4` | Process-Level Causal Failure Localization for Clinical AI Agents | `1C4` | Failure ontology, critical-step localization, counterfactual trajectory replay, and targeted intervention | Includes causal attribution within an agent execution; excludes attribution of regressions to component/version changes across releases. |
| `S02-NF5` | Versioned Continual Assurance and Change Attribution for Clinical AI | `2D4` | Versioned failure-surface model with budgeted regression discovery and component-change localization | Includes repeated assurance across system releases under a testing budget; excludes within-trajectory critical-step attribution as a separate methodological spine. |
| `S02-NF6` | Probabilistic Clinical Constraint Induction and Proof-Carrying Repair | `2D2` | Applicability-scoped temporal/ontological constraints and minimal auditable representation repair | Includes learning, validating, and applying constraints to structured clinical representations; excludes diagnostic-trajectory modeling unless used as one validation domain. |
| `S02-NF7` | Adequacy- and Currency-Aware Clinical Claim Verification | `3C1` | Typed claim-evidence calculus, expert benchmark, and calibrated verifier | Includes support, methodological adequacy, temporal currency, and patient applicability; excludes general multi-action agent control beyond verifier enforcement. |
| `S02-NF8` | Measurement-Error-Aware Clinical NLP Evaluation | `3C4` | Measurement-error decomposition, noise-aware ranking inference, and validated corrected evaluation protocols | Includes error in the evaluation instrument itself; excludes primary modeling of the clinical AI system being evaluated. |

## 7. Disagreement ledger against the coordinator proposal

| Coordinator judgment | Stream 02 judgment | Exact reason | Consequence if adopted |
|---|---|---|---|
| N4: `1C4` and `2D4` are the same direction at the dissertation-family level | **PARTIAL OVERLAP; SPLIT** | Within-run critical-step causation and across-release component-change causation use different units, interventions, aims, baselines, and falsification tests. Combining them requires a new hierarchical thesis absent from both frozen candidates. | Replace N4 with two normalized families; total normalized family count increases from seven to eight. |
| N5 is distinct from N2, though related | **PARTIAL OVERLAP, but remain separate** | `1C2` already makes temporal transition constraints and trajectory consistency part of its method, while `2D2` generalizes constraint induction, violation localization, and proof-carrying repair. The shared constraint layer is substantive, not merely thematic. | Family count is unchanged, but normalization must flag duplicate temporal-constraint aims and preserve the repair-versus-trajectory boundary. |
| N6 is distinct but adjacent to N1 | **PARTIAL OVERLAP, but remain separate** | N6's verifier outputs are explicit N1 evidence-state signals, and N6's enforcement aim gates generation; nevertheless N6 has an independent calculus/benchmark/verifier thesis that survives without N1 control. | Family count is unchanged; record an upstream-verifier/downstream-controller interface and do not collapse the two dissertations. |

**Number of disagreements:** **3** relationship judgments, of which **1** changes the normalized family count.

## 8. “Several fashionable projects” merge-coherence audit

| Proposed merge | Failure mode present? | Judgment |
|---|---|---|
| N1's three members | No, if normalized narrowly | Accept only the shared structured-state-to-multi-action-control thesis. Treat dual clocks and structural signals as competing/complementary representations rather than mandatory parallel projects. |
| N2's two members | No | Their benchmark, representation, constraints, and adjudication tests all bear on one diagnostic-trajectory thesis. |
| N3's two members | No | Contract semantics, selective decisions, and empirical validation test one data-fitness thesis. |
| Coordinator N4 (`1C4` + `2D4`) | **Yes** | Reject. Process localization/counterfactual step repair and versioned regression discovery/test allocation are two methodological spines placed side by side. |
| N2 + N5 | **Yes** unless N5 is narrowed to a method component | Reject as a family merge. A general repair calculus and a diagnostic-trajectory representation are separate theses. |
| N1 + N6 | **Yes** | Reject as a family merge. Claim-evidence adequacy verification and multi-action selective control each require their own formalism, ground truth, and decisive experiment. |
| N4 + N7 | **Yes** | Reject. Assurance of changing systems and measurement-error science about evaluation instruments are coupled but not one thesis. |

The only coordinator merge that triggers the prohibited failure mode is N4. The partial-overlap relationships above would also trigger it if converted into additional merges.

## 9. Final normalization judgment and freeze boundary

The 12 nominal candidates reduce to **eight** independently defensible dissertation-direction identities under the stated test. Five candidate pairs are `SAME DIRECTION`; the remaining relationships are either substantive but non-merging partial overlaps or genuinely distinct.

This review does not rank the eight families, average verdicts, select finalists, assess novelty, or modify any Day 1 conclusion. Further scientific testing belongs to a later task.

**Status: FROZEN — ROUND 2 INDEPENDENT NORMALIZATION REVIEW**
