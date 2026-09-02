# N5 Candidate Evaluation Packet

- **Candidate identifier:** N5
- **Candidate title:** Probabilistic Clinical Constraint Induction and Proof-Carrying Repair
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifact and section:** `analysis/analysis_02/day1_candidate_generation_v2.md` D02-02
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N5 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **probabilistic, applicability-scoped clinical constraint-induction framework** that learns executable temporal and ontological constraints over structured clinical representations, detects and localizes violations, and produces **minimal proof-carrying repairs** whose rationale and affected facts are machine-checkable.

The object must distinguish clinically meaningful constraints from site-specific regularities, preserve legitimate exceptions and uncertainty, and evaluate semantic correctness rather than rewarding formal consistency alone.

## 2. Exact falsifiable thesis

> A jointly learned probabilistic temporal and ontological constraint model with explicit applicability conditions, coupled to minimal proof-carrying repair, will improve contradiction detection, reduce false correction, and improve downstream longitudinal reasoning under domain shift relative to unconstrained neural extraction, prompt-only self-revision, knowledge-graph lookup, fixed-rule validation, and strong language-model-plus-rule baselines.

The thesis is defeated or materially weakened if:

- learned constraints do not transfer beyond the source site, task, or population;
- constraints capture statistical regularities rather than clinically valid rules;
- repair improves formal validity while harming semantic fidelity;
- fixed expert rules plus a strong model are prospectively equivalent;
- useful exceptions cannot be represented without making constraints vacuous;
- existing program-induction, database-repair, or neuro-symbolic systems already provide substantially the same scoped induction and proof-carrying minimal repair.

## 3. Included scientific scope

The common Phase 1 target includes:

1. Clinical representations derived from text, longitudinal records, concept mapping, event sequences, or knowledge structures.
2. Temporal, ontological, typing, polarity, uncertainty, laterality, episode-boundary, or related constraints whose clinical applicability can be stated.
3. Learning or inducing constraints from data and expert knowledge rather than relying only on a fixed hand-written rule base.
4. Explicit applicability conditions, confidence, exception handling, and uncertainty over learned constraints.
5. Detection and localization of violations in a structured representation.
6. Minimal repair that records which facts changed, which constraints justified the change, and why the proposed repair was selected.
7. Evaluation of false corrections, semantic repair fidelity, formal violation reduction, transfer, and downstream reasoning.
8. Strong comparisons with unconstrained neural models, prompt-only self-correction, fixed rules, and hybrid rule-plus-language-model baselines.
9. Cross-site, cross-domain, or otherwise meaningful distribution-shift testing.

## 4. Explicitly excluded scientific scope

The following are not part of N5's mandatory identity:

- Diagnostic-state trajectory modeling as the primary scientific object; that is N2, although N5 constraints may supply N2 transition rules.
- Generic knowledge-graph verification or generate-then-revise pipelines without learned applicability-scoped constraints.
- Fixed-rule validation alone.
- Formal consistency as a substitute for clinical semantic correctness.
- Silent overwriting of uncertain, contradictory, or exceptional facts.
- A requirement to use one specific logic formalism, differentiable-logic library, or foundation model.
- Generic concept mapping or extraction where no repair/constraint-learning problem is posed.
- Repair of raw text as the sole output; the thesis concerns structured clinical representations and auditable repair semantics.
- A broad claim that neuro-symbolic artificial intelligence is inherently superior.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| D02-02 — Learned Temporal Clinical Constraints for Auditable Representation Repair | Probabilistic constraint induction; applicability conditions; violation localization; minimal proof-carrying repair; transfer and downstream evaluation | Complete scientific source for the normalized singleton | One particular representation type, clinical specialty, or symbolic language |

N5 has partial machinery overlap with N2 but remains distinct: N2 tests diagnostic-trajectory fidelity, whereas N5 tests whether valid constraints can be learned and used for safe repair.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Define and validate constraint targets | Which clinical temporal/ontological constraints are learnable, when do they apply, and how can exceptions and uncertainty be represented? | Constraint language, applicability model, expert/data-derived candidates, and violation benchmark | Clinically valid constraints can be distinguished from accidental correlations | Agreement, stability, exception coverage, and evidence that constraints predict genuine semantic defects |
| Aim 2 — Induce constraints and perform proof-carrying minimal repair | Can a learned hybrid system localize violations and repair them with fewer false corrections than strong neural, fixed-rule, and prompt-only baselines? | Probabilistic induction, minimal-change optimization, proof/trace generation, and ablation | Learned scoped constraints add reliable, auditable repair capability | Better detection and semantic repair fidelity at controlled false-correction rate, with useful traces and component ablations |
| Aim 3 — Test transfer and downstream consequences | Do learned constraints and repairs remain valid under site/domain shift and improve downstream longitudinal reasoning? | Cross-domain adaptation, frozen-constraint tests, downstream task evaluation | The learned rules are not site correlations and formal repair creates real semantic benefit | Preserved validity or explicit applicability boundaries, lower false correction, and downstream gains not explained by violation-count reduction alone |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a structured clinical representation containing controlled or expert-validated violations, legitimate exceptions, and uncertain cases, evaluated both in-domain and under shift.
- **Strongest comparator:** a carefully engineered fixed-rule validator plus a strong language model, alongside unconstrained extraction, prompt-only self-revision, and knowledge-graph lookup.
- **Primary thesis-relevant outcomes:** contradiction/violation detection, semantic repair accuracy, false-correction rate, minimality, trace validity, exception preservation, transfer, and downstream reasoning.
- **Supporting result pattern:** induced applicability-scoped constraints outperform fixed and neural alternatives on semantic repair fidelity and false correction under shift, and repairs yield downstream benefits beyond formal violation reduction.
- **Defeating result pattern:** fixed rules plus a strong model are prospectively equivalent; learned constraints collapse under shift; formal corrections damage meaning; or the same induction-and-repair object already exists in prior work.

## 8. Inherited dangerous prior art

These are inherited Day 1 starting points. Phase 1 must inspect their methods and relevant parent disciplines independently.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| `LIT-028` | Prenosil et al., neuro-symbolic artificial intelligence for auditable information extraction from medical reports, DOI `10.1038/s43856-025-01194-x` | Demonstrates symbolic rules correcting or auditing neural/LLM clinical extraction | SCREENED | Does it learn applicability-scoped constraints and emit minimal proof-carrying repairs, or apply supplied rules? |
| `LIT-029` | Zhang et al., neural-symbolic biomedical concept-mapping agent, DOI `10.1038/s41746-026-02594-6` | Occupies neural-symbolic concept mapping and auditable structured output | SCREENED | Does its verification/revision machinery overlap N5's induction and repair semantics? |
| `LIT-001` | Su et al., *KGARevion*, ICLR 2025, arXiv `2410.04660` | Generate-verify-revise architecture using a knowledge graph | READ in prior repository work | Is proof-carrying repair genuinely different from its verification/revision loop? |
| Unregistered, DOI `10.1609/aaai.v38i14.29460` | Theodorou et al., *ConSequence* | Enforces hard and soft temporal/spatial constraints in synthetic Electronic Health Record generation | Day 1 page/section characterization | Does it already provide the relevant constraint representation and optimization, with learning being an incremental extension? |
| Unregistered | Temporal Cohort Logic | Formal temporal language for clinical cohorts | Day 1 source characterization | Does its rule language or execution semantics subsume N5's temporal constraint component? |
| Unregistered, DOI `10.1038/s41746-025-01965-9` | Cui et al., *TIMER* | Time-aware learning over longitudinal records | Day 1 source characterization | Does time-aware modeling already learn the relevant constraints or merely improve temporal instruction following? |
| Source family | Inductive logic programming, differentiable/probabilistic logic, program synthesis, constraint learning, data validation, database repair, probabilistic databases | Most dangerous parent disciplines for the central induction/repair contribution | Not comprehensively searched on Day 1 | Does established work already learn scoped constraints and perform minimal explainable repair? |
| Source family | Error-correcting structured prediction, ontology repair, knowledge-base completion, neuro-symbolic consistency training | Could provide strong simple or direct methodological precedents | Not comprehensively searched on Day 1 | Is N5 primarily a clinical application of existing repair methods? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether parent-discipline work already provides the same applicability-scoped induction and minimal repair | KT1 | Could fatally preempt the scientific object | Day 1 explicitly deferred the necessary search |
| Whether learned constraints reflect clinically valid rules rather than site correlations | KT3/KT6 | Invalid rules would make repair unsafe and non-transferable | Central unresolved epistemic question |
| Whether semantic repair fidelity improves rather than only formal consistency | KT3/KT4 | Violation reduction alone cannot support the thesis | Proposed evaluation only |
| Whether fixed rules plus a strong language model are practically equivalent | KT4 | Equivalent simpler machinery would remove necessity | Unresolved; decisive baseline not implemented |
| Whether experts can validate constraints, applicability conditions, and repair traces reproducibly | KT3/KT5 | Ground truth and feasibility depend on it | Plausible but uncertain; no commitment inferred |
| Whether the direction supports a dissertation rather than one method paper | ST1/KT2 | Could lack enough coherent depth after novelty narrowing | Day 1 judged depth high but collision risk substantial |
| Whether a representation domain can be selected without making the thesis application-bound | ST2/KT5 | Generality requires more than one narrow schema | Several possible domains exist; final choice unresolved |

## 10. Feasibility assumptions inherited from Day 1

- Structured clinical outputs and synthetic or manually perturbed violations can support an initial benchmark.
- Existing ontologies, temporal resources, and clinical expertise can seed—but should not fully predetermine—the candidate constraint space.
- Limited expert validation is plausibly available for constraint semantics and repair traces; no individual commitment is inferred.
- Public or controlled datasets can support the core method before any restricted-data validation.
- Computation for constraint induction, hybrid inference, ablation, and cross-domain testing is available at research scale.
- At least one external representation/task can be used to test whether learned constraints transfer.

## 11. Packet provenance and change control

### Direct compressions

- The scientific object, thesis, failure conditions, aims, baselines, inherited sources, and critical uncertainty are compressed from D02-02.
- The focus on applicability conditions, exception handling, false correction, and proof-carrying minimal repair is preserved directly.

### Reconciled formulations

- The packet explicitly treats semantic fidelity and downstream benefit as necessary outcomes so that formal consistency alone cannot satisfy the thesis.
- The boundary with N2 is made explicit without removing diagnostic trajectories as a possible validation domain.

### Unresolved candidate-definition tension

Fidelity reviewers should assess whether `proof-carrying repair` is sufficiently defined by the inherited record or whether the packet has made the trace requirement stronger than the original proposal. Any correction must preserve the auditable-repair identity without performing novelty research.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
