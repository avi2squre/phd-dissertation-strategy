# N2 Candidate Evaluation Packet

- **Candidate identifier:** N2
- **Candidate title:** Diagnostic-State Trajectory Representation and Inference
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifacts and sections:** `analysis/analysis_01/day1_candidate_generation_v2.md` C2; `analysis/analysis_03/day1_candidate_generation_v2.md` C2
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N2 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **patient-level diagnostic-state trajectory representation** with explicit states, evidence-conditioned transitions, resolving events, temporal-transition constraints, trajectory-aware inference, and transition-level evaluation.

The object is not merely a timeline of mentions. It represents what the longitudinal record supports about a diagnosis at each evidence horizon, including states such as suspected, provisional or working, confirmed, excluded or ruled out, and historical, together with the evidence that justifies transitions.

## 2. Exact falsifiable thesis

> Explicit patient-level diagnostic-state trajectories, including evidence-conditioned transitions and resolving events, can be recovered from longitudinal clinical records more faithfully than per-mention assertion classification plus simple aggregation or unconstrained long-context generation; trajectory-aware representations and inference will improve state-at-time and transition fidelity, particularly as record length and diagnostic complexity increase, and will provide clinically useful agreement with an independent reference standard where such a standard is available.

The thesis is defeated or materially weakened if:

- per-mention assertion plus simple aggregation is prospectively equivalent to trajectory-aware modeling;
- long-context generation matches trajectory fidelity without an explicit representation;
- diagnostic states or transitions cannot be annotated or otherwise identified reliably;
- apparent gains depend on hindsight leakage from later resolving events;
- an existing general multi-disease trajectory formalism and benchmark already provide the proposed object and evaluation;
- neither trajectory-aware nor simpler methods approach the fidelity needed for the intended downstream use.

## 3. Included scientific scope

The common Phase 1 target includes:

1. A disease-agnostic or multi-condition ontology of patient-level diagnostic states.
2. Evidence-horizon labeling: what was supportable at a given time, not merely what became known later.
3. Explicit transitions, transition triggers, and resolving events such as definitive tests, specialist adjudication, pathology, or genetic confirmation where appropriate.
4. An annotation or reference-standard methodology with agreement and adjudication procedures.
5. Comparison of explicit trajectory inference against per-mention assertion classification plus aggregation, whole-chart prompting, and other strong longitudinal baselines.
6. Transition-aware evaluation, including state-at-time fidelity, transition detection, resolution-event detection, and timing error.
7. Temporal constraints or trajectory-consistency mechanisms as candidate methods, not assumed requirements.
8. Validation on more than one condition, record type, or setting where feasible.
9. A clinically meaningful downstream validation, such as cohort-status adjudication, provided it can be performed without making one restricted dataset the sole scientific contribution.

## 4. Explicitly excluded scientific scope

The following do not belong to N2's mandatory scientific identity:

- General temporal relation extraction without patient-level diagnostic-state semantics.
- Generic event-timeline generation where the target is treatment or event ordering rather than diagnostic belief/status.
- General representation repair or proof-carrying correction across arbitrary clinical structures; that is N5.
- A controller choosing answer, retrieve, ask, or defer; that is N1.
- A requirement that one rare-disease cohort, one genetic condition, or one institution define the dissertation.
- A claim that every diagnosis has a single objectively correct state at every time.
- Hindsight labeling that uses future evidence without explicitly distinguishing retrospective truth from contemporaneously supportable state.
- Simple phenotyping or code-based cohort construction without the trajectory representation.
- A requirement that symbolic constraints outperform all neural or long-context methods; constraint-guided and state-carrying models are competing mechanisms under the shared thesis.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S01-C2 — Temporally Constrained Diagnostic-State Reasoning from Longitudinal Electronic Health Records | Diagnostic-state ontology; temporally grounded transition constraints; trajectory-consistency objective; evidence-horizon fidelity | Constraint-oriented methodological formulation | A specifically neuro-symbolic solution or symbolic constraints as the only valid model |
| S03-C2 — Diagnostic-State Trajectories from Longitudinal Clinical Records | States, transitions, resolving events; annotation scheme; transition-aware metrics; cohort-ground-truth validation | Representation, measurement, and clinically grounded validation formulation | One rare-disease cohort as the mandatory dataset; replacement of clinician adjudication as the only success criterion |

The two formulations are **same direction with complementary mechanisms and validation emphases**.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Formalize and measure diagnostic trajectories | Can patient-level diagnostic states, evidence horizons, transitions, and resolving events be defined and labeled with sufficient validity? | Develop ontology, annotation protocol, benchmark, and transition-aware metrics | The proposed trajectory is a measurable scientific object rather than an annotation convention | Agreement, adjudication analysis, prevalence of snapshot/aggregation failure, and construct-validity evidence |
| Aim 2 — Infer trajectories and test representational value | Do explicit state-carrying or constraint-guided methods outperform assertion-plus-aggregation, whole-chart prompting, and unconstrained sequence models? | Develop and compare trajectory-aware inference mechanisms with ablations | Explicit trajectory structure improves state-at-time and transition fidelity | Practically meaningful improvement on preregistered trajectory metrics, especially for longer and more complex records |
| Aim 3 — Validate transfer and downstream fidelity | Does the representation generalize across conditions/settings and support a meaningful downstream task against independent ground truth? | Cross-condition transfer and limited adjudicated validation | The method is not a one-dataset formalism and has clinically meaningful validity | Reproducible cross-condition performance and agreement with an independent reference standard, or clear boundary conditions |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a longitudinal patient record partitioned into evidence horizons with independently defined diagnostic states and transitions.
- **Strongest comparator:** high-quality per-mention assertion extraction followed by prospectively specified aggregation rules, plus a strong long-context or retrieval-augmented whole-chart model.
- **Primary thesis-relevant outcomes:** state-at-time fidelity, transition/resolution-event accuracy with temporal tolerance, unsupported-transition rate, earliest-suspicion and confirmation timing error, and agreement with independent adjudication where available.
- **Supporting result pattern:** explicit trajectory modeling provides a practically meaningful advantage over both assertion-plus-aggregation and long-context baselines, with gains increasing under longer, contradictory, or diagnostically complex records and transferring beyond one disease.
- **Defeating result pattern:** simple aggregation or long-context models are prospectively equivalent; states/transitions cannot be labeled reproducibly; gains vanish after controlling hindsight and temporal leakage; or no defensible independent reference standard exists for the core claims.

## 8. Inherited dangerous prior art

These are inherited search targets, not preclassified collisions. Phase 1 reviewers must inspect them independently.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| Unregistered, DOI `10.1136/amiajnl-2011-000203` | Uzuner et al., i2b2 2010 assertion task | Strong mention-level certainty/assertion foundation | Day 1 source characterization | Can assertion plus aggregation already recover the trajectory sufficiently well? |
| Unregistered, DOI `10.1038/s41746-025-01965-9` | Cui et al., *TIMER* | Longitudinal temporal instruction/modeling and evaluation | Day 1 page/section-level characterization | Does TIMER or related work encode patient-level diagnostic-state evolution rather than temporal reasoning generally? |
| Unregistered, ACL `2024.clinicalnlp-1.53` | *ChemoTimelines* shared task | Cross-document clinical timeline construction | Day 1 page/abstract characterization | Is diagnostic-state trajectory modeling a straightforward extension of existing timeline extraction? |
| Unregistered, PMID `41726535` | Wang et al. 2025, multiple-myeloma status and earliest-diagnosis pipeline | Distinguishes suspected, newly diagnosed, and historical disease states | Day 1 page/abstract characterization | Does it already contain a transferable trajectory formalism or only a disease-specific pipeline? |
| Unregistered, DOI `10.1038/s41746-025-01433-4` | Schuemie et al., *KEEPER* | Uses language models for case adjudication across diseases and directly targets cohort ground truth | Day 1 page/section-level characterization | Can structured-data-plus-LLM adjudication solve the downstream problem without trajectory representation? |
| Unregistered, DOI `10.64898/2026.03.23.26349012` | Dickerson et al. 2026, whole-chart longitudinal oncology abstraction | Reports high concordance and includes time-varying disease status | Day 1 abstract/page characterization | Does whole-chart abstraction already recover the target states and transitions at comparable depth? |
| Unregistered, DOI `10.64898/2026.02.10.26345124` | Paverd et al. 2026, longitudinal liver-disease trajectory reconstruction | Direct longitudinal trajectory terminology and open-model scaling | Day 1 abstract/page characterization | Is the proposed scientific object already implemented in another disease domain? |
| `LIT-015` | Faviez et al. 2024, partner-site disease-family detection from Electronic Health Records | Could preempt or narrow the rare-disease validation instantiation | Repository record not fully verified in Day 1 | Does it model diagnostic status over time or only detect disease? |
| Source family | Temporal knowledge graphs, hidden-state/sequential diagnosis models, probabilistic graphical models, process mining, longitudinal phenotyping | A mature parent discipline may already formalize diagnostic-state transitions | Not comprehensively searched on Day 1 | Is N2 new only in terminology or dataset? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether a general multi-disease diagnostic-state trajectory formalism and benchmark already exist | KT1 | Could substantially or fatally preempt the proposed object | Day 1 search non-finding only; not saturated |
| Whether the proposed states and transitions can be labeled without hindsight leakage or poor agreement | KT3 | Invalid ground truth would undermine the entire evaluation | Unresolved; resolving events offer a partial anchor |
| Whether explicit trajectory structure beats strong assertion-plus-aggregation and long-context baselines | KT4 | Failure removes the representational necessity claim | Proposed hypothesis only |
| Whether clinician adjudication and governed note access are obtainable | KT5 | Affects the strongest downstream validation | Public-data minimum path appears plausible; institutional validation uncertain |
| Whether the direction is one coherent thesis rather than ontology, benchmark, model, and cohort project placed together | KT2/ST1 | Could reduce it to one strong benchmark paper or require narrowing | Round 3 found a coherent common thesis, but Phase 1 must attack it |
| Whether stronger long-context models commoditize the inference contribution | KT6 | Could leave only the benchmark/annotation contribution | Unresolved; state-at-time validity may remain structural |

## 10. Feasibility assumptions inherited from Day 1

- Public longitudinal clinical records or shared-task corpora can support a minimum open benchmark, subject to data-use restrictions.
- Existing temporal and assertion annotations can provide partial scaffolding but will not automatically supply diagnostic-state ground truth.
- Resolving events such as pathology, specialist adjudication, or genetic confirmation can anchor some transitions without defining every state.
- A limited institutional cohort may be available for downstream validation, but data governance, note movement, annotation assignment, and clinician time remain unresolved; no access commitment is inferred.
- Public-data Aims 1 and 2 should remain scientifically meaningful if the institutional Aim 3 is delayed or unavailable.
- Appropriate computational resources for longitudinal modeling and evaluation are plausibly available without assuming frontier-model pretraining.

## 11. Packet provenance and change control

### Direct compressions

- The diagnostic-state object, failure conditions, baseline comparisons, inherited sources, and critical uncertainties come from S01-C2 and S03-C2.
- Resolving events, transition-aware metrics, evidence-horizon fidelity, and adjudication risk preserve the constituent formulations.

### Reconciled formulations

- The exact thesis combines the shared representational claim with the constraint-oriented and adjudication-oriented mechanisms accepted in Round 3.
- The aims are a common packet architecture: formalize/measure, infer/compare, and transfer/validate.

### Unresolved candidate-definition tension

The packet treats a clinically adjudicated downstream study as important but not the sole scientific identity. Fidelity auditors should determine whether this preserves the intended clinical anchor or weakens the constituent proposal too much. Any disagreement must be recorded without performing novelty research.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
