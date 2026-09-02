# N4a Candidate Evaluation Packet

- **Candidate identifier:** N4a
- **Candidate title:** Process-Level Causal Failure Localization for Clinical Artificial Intelligence Agents
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifact and section:** `analysis/analysis_01/day1_candidate_generation_v2.md` C4
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N4a target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **process-level causal failure-localization framework** for long-horizon clinical agents, comprising:

- a clinically grounded failure ontology;
- a critical-step localizer over execution trajectories;
- counterfactual step replay or intervention across stochastic reruns;
- dynamic stress conditions that expose process failures;
- evaluation of whether targeted intervention at the localized step improves downstream safety.

The scientific unit is a failure-producing step or set of steps within one agent execution, not a component change across software/model releases.

## 2. Exact falsifiable thesis

> Process-aware evaluation with explicit critical-step localization and counterfactual step intervention will identify and explain clinically consequential failures within long-horizon agent trajectories more reliably than endpoint-only scoring, post-hoc language-model judging, generic trace diagnosis, random-step intervention, and full-trajectory retry or reflection; interventions targeted at the localized causal step will improve downstream safety or utility more than non-targeted safeguards.

The thesis is defeated or materially weakened if:

- process annotations do not improve failure prediction or localization;
- critical steps cannot be identified reproducibly because failures are diffuse, multicausal, or observer-dependent;
- counterfactual replay does not establish a stable causal effect under stochastic execution;
- generic failure-diagnosis methods transfer directly and perform equivalently;
- targeted repair is no better than random repair, generic retry, reflection, or broad oversight;
- existing work already combines comparable localization, counterfactual intervention, and clinical process evaluation.

## 3. Included scientific scope

The common Phase 1 target includes:

1. Long-horizon clinical-agent trajectories involving information gathering, evidence grounding, tool use, state maintenance, policy compliance, escalation, and intermediate decisions.
2. A clinically meaningful failure ontology capable of distinguishing process failures that endpoint accuracy conceals.
3. Localization of the earliest or most consequential failure-producing step, allowing multicausal or set-valued attribution where justified.
4. Counterfactual intervention in which a selected step is replaced, repaired, or constrained and downstream effects are measured across repeated stochastic continuations.
5. Dynamic or controlled stress conditions that generate clinically plausible missingness, contradiction, tool failure, policy conflict, or resource limitation.
6. Comparison against endpoint scores, generic language-model judges, rule checkers, trace-diagnosis methods, random-step repairs, retry, and reflection.
7. Metrics for localization validity, counterfactual downstream effect, process-safety violations, recovery, and expert agreement.
8. Reproducible logged trajectories and replay infrastructure.

## 4. Explicitly excluded scientific scope

The following are not part of N4a's mandatory identity:

- Regression discovery or attribution to changes across model, prompt, corpus, tool, policy, or software versions; that is N4b.
- Generic dynamic red-teaming without causal/process-level localization and targeted intervention.
- Generic process-aware benchmarking without a new failure-attribution method.
- A claim that every failed trajectory has one unique critical step.
- A requirement to infer human-like reasoning or expose proprietary chain-of-thought.
- A requirement to use one specific agent architecture, base model, or clinical specialty.
- General runtime action selection under uncertainty; that is N1.
- Measurement-error modeling of the evaluation instrument itself; that is N7.
- Combining all dynamic evaluation, agent diagnosis, and red-team systems as an engineering stack without a distinct causal-attribution contribution.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S01-C4 — Process-Aware Dynamic Assurance and Failure Localization for Clinical AI Agents | Failure ontology; critical-step localizer; counterfactual replay/intervention; dynamic stress generator; process-safety evaluation | Complete scientific source for the normalized singleton | Cross-version component attribution; every originally proposed workflow or clinical environment |

Round 3 split the broader assurance family because within-trajectory step attribution and across-version change attribution use different causal units, experiments, and theses.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Define and validate process-failure targets | Can clinically consequential trajectory failures and candidate critical steps be represented and identified with sufficient validity? | Develop ontology, annotation/controlled-truth procedure, and localization benchmark | Process information contains valid failure-localization signal beyond endpoint outcome | Localization ground truth or defensible partial truth, agreement, failure-class validity, and prediction gains over endpoint-only signals |
| Aim 2 — Establish causal contribution through intervention | Does intervening on the localized step change downstream outcomes more than non-targeted intervention? | Counterfactual replay with controlled step replacement and repeated stochastic continuations | Localized steps are causally consequential, not merely correlated with failure | Larger downstream safety/utility improvement for targeted versus random or generic repairs, with uncertainty from reruns quantified |
| Aim 3 — Test robustness under dynamic stress | Does the localization/intervention framework retain validity across stressors, models, and workflows? | Adaptive or controlled perturbation, transfer tests, and model-replacement evaluation | The attribution framework is not specific to one trace distribution | Transferable failure classes, stable intervention effects or explicit boundary conditions, and useful targeted safeguards |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a logged clinical-agent trajectory with an endpoint outcome and either injected/controlled failure location or an independently adjudicated candidate failure set.
- **Strongest comparator:** AgentRx-style trace diagnosis or another general failure localizer, a generic language-model judge, endpoint-only attribution, and random-step or full-trajectory repair.
- **Primary thesis-relevant outcomes:** critical-step or set localization validity, counterfactual downstream effect, recovery efficiency, clinically weighted safety, and uncertainty across stochastic continuations.
- **Supporting result pattern:** the method localizes a causally consequential step more accurately than serious baselines, and targeted intervention produces a reproducible downstream improvement exceeding random-step repair, retry, or reflection across more than one model/workflow.
- **Defeating result pattern:** no stable critical-step target exists; localization is not reproducible; intervention effects vanish across reruns; generic trace diagnosis is prospectively equivalent; or comparable prior work already performs the same localization-plus-intervention evaluation.

## 8. Inherited dangerous prior art

These are inherited Day 1 threats and require independent Phase 1 inspection.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| `LIT-032` or Day 1 DAS reference | Dynamic, automatic, systematic red-teaming for health/medical models | Occupies adaptive stress generation and dynamic safety evaluation | Repository status SCREENED / Day 1 page-level characterization | Does it also localize causal process failures and evaluate targeted interventions? |
| Unregistered | *AgentClinic* | Interactive clinical-agent benchmark with tools, notes, reflection, and sequential trajectories | Day 1 page/section-level characterization | Does its process evaluation already define the relevant failure targets or only benchmark outcomes? |
| Unregistered | *MedCTA* or equivalent medical tool-trajectory benchmark | Very close process-aware evaluation of clinical tool-use trajectories | Day 1 source characterization; exact depth to verify | Does it include critical-step localization and counterfactual repair at comparable depth? |
| Unregistered, DOI `10.1371/journal.pmed.1005170` | Ruhrberg Estévez et al., *How to benchmark medical AI agents* | Establishes process/trajectory evaluation as an explicit field requirement | Day 1 relevant-page characterization | Does the candidate add a method beyond implementing the proposed benchmarking principles? |
| Unregistered 2026 preprint | Barke et al., *AgentRx: Diagnosing AI Agent Failures from Execution Trajectories* | Direct parent-domain threat for critical failure-step localization | Day 1 abstract/page characterization | Does AgentRx already provide the localization, causal attribution, and intervention mechanism N4a proposes? |
| Source family | Program debugging, causal fault localization, counterfactual explanation, software testing, process mining, reinforcement-learning credit assignment | Mature parent disciplines may already contain the central attribution method | Not comprehensively searched on Day 1 | Is clinical application the only remaining novelty? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether MedCTA, AgentRx, DAS, or imminent related work already combine comparable localization and counterfactual repair | KT1 | Could fatally preempt the contribution | Day 1 identified a high collision burden; relevant methods not fully audited |
| Whether a critical step or failure set can be defined and validated | KT3 | The causal target may be unobservable or non-unique | Unresolved; controlled injection may supply partial truth |
| Whether targeted step repair causally improves outcomes beyond generic retry/reflection | KT4 | Failure would remove the methodological necessity claim | Proposed experiment only |
| Whether counterfactual replay is valid under stochastic downstream behavior and path dependence | KT3 | Intervention effects may be unstable or uninterpretable | Unresolved |
| Whether benchmark, ontology, localization, and dynamic stress remain one thesis | KT2/ST1 | Could become several assurance projects sharing vocabulary | Round 3 preserved N4a as a distinct direction but did not validate coherence |
| Whether realistic long-horizon workflows and expert review are available | KT5 | Affects ecological validity | Public/synthetic path appears plausible; clinical validation uncertain |
| Whether stronger native agent diagnostics commoditize the localizer | KT6 | Moving frontier may reduce empirical headroom | Structural intervention testing may remain durable; unresolved |

## 10. Feasibility assumptions inherited from Day 1

- Public agent benchmarks and traceable trajectories are available for a minimum open study.
- Controlled tool failures, missing evidence, contradictory outputs, and policy constraints can be injected to provide partial causal truth.
- Repeated stochastic continuations are computationally feasible at research scale.
- Limited clinician or domain-expert review may be obtainable for clinical consequence and failure-class validity; no commitment is inferred.
- A benchmark/localization first paper can be attempted without restricted clinical data.
- Logged traces or externally visible agent actions are sufficient; proprietary hidden chain-of-thought is not assumed.

## 11. Packet provenance and change control

### Direct compressions

- The object, thesis, aims, evaluation units, dangerous prior art, and rejection trigger are compressed from S01-C4.
- The within-trajectory causal unit and counterfactual intervention requirement are preserved from Round 3.

### Reconciled formulations

- The packet explicitly permits set-valued or multicausal attribution so that the candidate does not assume one unique critical step when the source did not justify that assumption.
- The scope boundary excludes N4b's version/component-change thesis.

### Unresolved candidate-definition tension

The candidate's identity depends on causal failure attribution, not merely process annotation. Fidelity reviewers should determine whether dynamic stress generation is necessary to the core thesis or should remain an optional validation mechanism. They should also flag any concern that allowing set-valued attribution materially changes the original candidate.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
