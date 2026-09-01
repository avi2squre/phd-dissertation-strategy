# Round 3 — Cross-Stream Candidate Normalization Reconciliation

- **Date:** 2026-08-31
- **Base:** canonical Day 1 checkpoint `4deee8eb8425b22e9532f1f3afd74791ef3e422c`
- **Status:** **FROZEN — ROUND 3 NORMALIZATION RECONCILIATION**
- **Scope:** scientific-identity reconciliation only. This artifact does not rank directions, select finalists, average Day 1 verdicts, perform new literature research, or begin adversarial scientific falsification.

## 1. Inputs and reconciliation rule

This reconciliation uses the three Common Analysis Schema v2 Day 1 artifacts, the coordinator Round 1 normalization hypothesis, and the two frozen independent Round 2 normalization reviews. No new external literature search was performed.

Disagreements are resolved by scientific identity rather than majority vote. The governing test is whether proposed members can be represented by **one central scientific object, one falsifiable dissertation thesis, and one coherent set of aims** without turning the dissertation into several attractive projects placed beside one another.

Relationship labels retain their established meanings:

- **SAME DIRECTION:** one scientific object/thesis can encompass the candidates; differences are complementary, competing, or scoped formulations.
- **PARTIAL OVERLAP:** a substantive method, representation, resource, or evaluation layer is shared, but merging would erase an important scientific boundary or create more than one thesis.
- **DISTINCT:** no dissertation-level identity merge is justified.

Normalization is not ranking. Independent convergence is not evidence that a direction is better, and singleton status is not evidence that a direction is weaker.

## 2. Reconciled mapping: 12 original candidates to 8 normalized directions

| Normalized ID | Normalized candidate dissertation direction | Constituent Day 1 candidates | Reconciled relationship |
|---|---|---|---|
| **N1** | Structured Evidence-State Selective Control for Clinical AI | S01-C1; D02-01; S03-C3 | SAME DIRECTION, with competing/complementary formulations |
| **N2** | Diagnostic-State Trajectory Representation and Inference | S01-C2; S03-C2 | SAME DIRECTION, complementary formulations |
| **N3** | Machine-Checkable Causal Data-Fitness for Target-Trial Emulation | S01-C3; D02-03 | SAME DIRECTION, complementary formulations |
| **N4a** | Process-Level Causal Failure Localization for Clinical AI Agents | S01-C4 | DISTINCT direction within the broader assurance/failure-attribution family |
| **N4b** | Versioned Continual Assurance and Change Attribution for Clinical AI | D02-04 | DISTINCT direction within the broader assurance/failure-attribution family |
| **N5** | Probabilistic Clinical Constraint Induction and Proof-Carrying Repair | D02-02 | DISTINCT; partial machinery overlap with N2 |
| **N6** | Adequacy- and Currency-Aware Clinical Claim Verification | S03-C1 | DISTINCT; partial upstream/downstream overlap with N1 |
| **N7** | Measurement-Error-Aware Clinical NLP Evaluation | S03-C4 | DISTINCT; evaluation-instrument interfaces with other directions |

**Result:** 12 nominal Day 1 candidates normalize to **8 candidate dissertation directions across 7 broader research families**. N4a and N4b share a broad assurance/failure-attribution family but are not one dissertation direction.

## 3. Reconciled decisions

### N1 — Structured Evidence-State Selective Control for Clinical AI

**Decision:** retain S01-C1, D02-01, and S03-C3 as one normalized dissertation direction, but explicitly as **competing/complementary formulations**, not as three additive methodological spines.

**Shared scientific object:** a structured representation of why commitment may be unsafe or incomplete, coupled to a clinically cost-sensitive multi-action controller choosing among actions such as answer, retrieve, verify, revise/flag, ask, or defer.

**Preserved variants:**

- S01-C1: typed evidence/uncertainty state.
- D02-01: provenance-linked belief state with separate patient-event and evidence-validity clocks.
- S03-C3: task-structural failure signals, asymmetric risk, workload-normalized evaluation, and distribution-shift testing.

**Reconciliation of Round 2 disagreement:** Stream 02 classified all three as SAME DIRECTION; Stream 03 argued that S03-C3 should be PARTIAL OVERLAP because its structural-signals-under-shift clause can be tested independently. The reconciled judgment retains SAME DIRECTION at the dissertation-identity level because all three ultimately test structured state/signal representations as inputs to the same selective action problem. Stream 03's warning is preserved as a scope constraint: the normalized dissertation must compare or choose among these representations rather than require all of their original task settings and subclaims simultaneously.

**Boundary:** N1 does not absorb the full evidence-appraisal calculus of N6 or lifecycle assurance of N4.

### N2 — Diagnostic-State Trajectory Representation and Inference

**Decision:** merge S01-C2 and S03-C2.

**Shared scientific object:** explicit patient-level diagnostic states and evidence-conditioned transitions over longitudinal clinical records.

**Complementarity:** S01-C2 contributes temporal transition constraints, evidence-horizon justification, and trajectory consistency; S03-C2 contributes resolving events, annotation/adjudication machinery, transition-aware metrics, and cohort-ground-truth validation.

**Boundary:** N2 models diagnostic trajectories; it does not become a general representation-repair dissertation.

### N3 — Machine-Checkable Causal Data-Fitness for Target-Trial Emulation

**Decision:** merge S01-C3 and D02-03.

**Shared scientific object:** an executable representation/checker that maps a target-trial causal question and an EHR data-generating process to supported analysis, restricted/revised estimand, request for additional information, or refusal.

**Normalized emphasis:** the machine-checkable contract/checker is the durable methodological object; agentic translation/orchestration is an interface or implementation variant rather than the sole source of novelty.

### N4a and N4b — split the original N4

**Decision:** SPLIT. The coordinator Round 1 merge is rejected.

#### N4a — Process-Level Causal Failure Localization

**Object:** failure ontology, critical-step localization, counterfactual trajectory replay, and targeted intervention within an agent execution.

**Question:** which step in this execution caused the endpoint failure, and does intervening on that step change the outcome?

#### N4b — Versioned Continual Assurance and Change Attribution

**Object:** versioned failure-surface model, paired component perturbation, regression discovery, change attribution, and budgeted test selection across system releases.

**Question:** which system/component change caused a new regression, and which tests should be run next under a limited assurance budget?

**Reason for split:** the intervention units, causal questions, baselines, metrics, statistical machinery, and decisive experiments differ. Combining them without a genuinely unified attribution formalism would create two methodological spines rather than one thesis.

**Preserved possibility:** a future unified counterfactual-attribution formalism spanning execution steps and system versions may be investigated during later scientific work, but it is a new/redefined hypothesis and is not silently introduced by normalization.

### N5 — Probabilistic Clinical Constraint Induction and Proof-Carrying Repair

**Decision:** retain as DISTINCT.

**Object:** applicability-scoped temporal/ontological constraint induction, violation localization, and minimal auditable representation repair.

**Relationship to N2:** PARTIAL OVERLAP. N5's learned constraints could supply N2's transition rules, but trajectory fidelity and safe representation repair are different theses with different ground truths and falsification tests.

### N6 — Adequacy- and Currency-Aware Clinical Claim Verification

**Decision:** retain as DISTINCT from N1.

**Object:** typed claim-evidence verification over support, methodological adequacy, temporal currency, and patient applicability, with expert ground truth and calibrated verification.

**Relationship to N1:** PARTIAL OVERLAP. N6 verifier outputs can populate an N1 evidence state, and N1's evidence-validity clock shares temporal semantics with N6's currency dimension. Nevertheless N6 has an independent formalism, benchmark, verifier, calibration problem, and falsification test; it can succeed without a general multi-action controller.

### N7 — Measurement-Error-Aware Clinical NLP Evaluation

**Decision:** retain as DISTINCT.

**Object:** measurement-error decomposition of the evaluation instrument, uncertainty-aware system comparison/ranking, and validated corrected evaluation protocols.

**Boundary:** N7 studies error in the ruler used to evaluate systems rather than primarily studying failure of the system itself.

## 4. Preserved partial-overlap interfaces

Partial overlap should guide artifact reuse and coordinated prior-art review, not automatic merging.

| Interface | Relationship to preserve |
|---|---|
| **N5 → N2** | Learned temporal/clinical constraints may supply diagnostic-state transition rules. |
| **N6 → N1** | Adequacy/currency/applicability verification may supply structured evidence-state signals to the selective controller. |
| **N1 ↔ N2** | Longitudinal belief maintenance and diagnostic-state transitions share temporal-state semantics but optimize different outcomes. |
| **N4b ↔ N7** | Continual assurance under noisy adjudication/judge drift contains a measurement-error component, while N7 treats measurement error as the primary phenomenon. |
| **N7 → N2/N4** | Corrected evaluation methodology may improve transition metrics or assurance measurements without becoming those dissertations. |
| **N5 ↔ N6** | Typed temporal/applicability constraints and auditable verification traces share machinery but operate on different scientific objects. |

A broader recurring architecture also appears across N1, N3, and N6: represent validity explicitly in a typed structure and permit selective action/refusal. This is a portfolio-level pattern, **not** a valid umbrella dissertation direction.

## 5. Coherence safeguards

The following merges are explicitly rejected unless future evidence supports a genuinely new unifying thesis:

1. N4a + N4b as currently formulated.
2. N2 + N5.
3. N1 + N6.
4. N4 + N7.
5. N1 + N3 + N6 under a generic "typed validity state plus selective action" umbrella.

The normalized N1 is accepted only under a narrow state-to-action thesis; typed evidence states, dual clocks, and structural failure signals are alternative or complementary representations to test, not three mandatory dissertation projects.

## 6. Normalized set for the next scientific phase

The next adversarial scientific phase should operate on these eight identities:

1. **N1 — Structured Evidence-State Selective Control for Clinical AI**
2. **N2 — Diagnostic-State Trajectory Representation and Inference**
3. **N3 — Machine-Checkable Causal Data-Fitness for Target-Trial Emulation**
4. **N4a — Process-Level Causal Failure Localization for Clinical AI Agents**
5. **N4b — Versioned Continual Assurance and Change Attribution for Clinical AI**
6. **N5 — Probabilistic Clinical Constraint Induction and Proof-Carrying Repair**
7. **N6 — Adequacy- and Currency-Aware Clinical Claim Verification**
8. **N7 — Measurement-Error-Aware Clinical NLP Evaluation**

No Day 1 verdict is averaged or promoted into a normalized verdict by this artifact. Scientific strength, novelty, feasibility, and later strategic utility remain unresolved.

## 7. Strategic-boundary note

The project has an additional private strategic objective concerning long-term technical skill formation: among scientifically strong and feasible directions, prefer work that develops durable, portable capabilities and retains flexibility to absorb future frontier methods. Durable capabilities include representation learning, sequential decision making, uncertainty/risk, optimization, causal/statistical reasoning, rigorous evaluation, scalable experimentation, algorithm implementation, systems thinking, and research problem formulation.

This objective **does not affect the normalization decisions above** and must not rescue a scientifically weak direction during adversarial falsification. It belongs to the later strategic comparison layer, alongside publication propensity, broader career portability, commercialization, and other private criteria. Current tools or fashionable 2026 keywords should not substitute for durable technical depth.

## 8. Freeze boundary

This artifact freezes the reconciled **scientific identity map**, not scientific viability or ranking.

It does not:

- select finalists;
- rank N1–N7/N4a/N4b;
- perform new novelty searches;
- resolve Day 1 scientific uncertainties;
- score publication, career, commercialization, or immigration-related utility;
- modify any Day 1 or Round 2 artifact.

The next scientific operation is adversarial falsification of the eight normalized directions using explicit kill tests and targeted evidence retrieval.

**STATUS: FROZEN — ROUND 3 NORMALIZATION RECONCILIATION.**