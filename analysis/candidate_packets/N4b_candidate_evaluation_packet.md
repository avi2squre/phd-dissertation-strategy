# N4b Candidate Evaluation Packet

- **Candidate identifier:** N4b
- **Candidate title:** Versioned Continual Assurance and Change Attribution for Clinical Artificial Intelligence
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifact and section:** `analysis/analysis_02/day1_candidate_generation_v2.md` D02-04
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N4b target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **versioned clinical failure-surface representation** combined with **coverage-aware, budgeted regression-test selection** and **change-attribution machinery** for compound clinical artificial-intelligence systems whose base model, retrieval corpus, tools, prompts, policies, or input populations change over time.

The scientific unit is a clinically meaningful regression across system versions and its attribution to a changed system factor, not a critical step within one execution trajectory.

## 2. Exact falsifiable thesis

> A versioned failure-surface representation combined with sequential, coverage-aware test selection will detect clinically significant regressions earlier and attribute them to responsible system changes more accurately, at a fixed evaluation budget, than static benchmark reruns, undirected dynamic red-teaming, simple stratified regression suites, and accuracy-focused adaptive testing.

The thesis is defeated or materially weakened if:

- static or simply stratified regression suites achieve prospectively equivalent detection and attribution;
- dynamic red-teaming or computerized adaptive testing already provides the same version-aware attribution and budget efficiency;
- failure taxonomies or failure-surface structure do not transfer across releases;
- automated or human adjudication noise dominates the change signal;
- component changes cannot be disentangled because releases alter multiple coupled factors without valid interventions;
- a comparable versioned assurance framework already exists.

## 3. Included scientific scope

The common Phase 1 target includes:

1. A versioned representation of clinically meaningful failure modes and their observed prevalence or risk.
2. Compound systems containing separable factors such as base model, retrieval corpus, tools, prompts, policies, and input population.
3. Paired or controlled version comparisons where one or more changes can be identified and, where feasible, experimentally isolated.
4. Sequential or adaptive selection of tests under a fixed assurance budget.
5. Detection of new regressions, recovery of previously known failures, and maintenance of failure lineage across releases.
6. Attribution of regression to changed components or factors, with calibrated uncertainty and false-alarm control.
7. Comparison with full static reruns, stratified suites, undirected dynamic red-teaming, random sampling, and accuracy-focused adaptive testing.
8. Evaluation under injected changes, historical releases, or controlled system variants with known or partially known change provenance.
9. Explicit handling of adjudicator uncertainty, judge drift, and repeated-measurement noise where they materially affect regression detection.

## 4. Explicitly excluded scientific scope

The following are not part of N4b's mandatory identity:

- Localization of a causal failure step within one agent execution; that is N4a.
- Generic benchmark updating, dynamic question generation, or continuous evaluation without version-aware attribution.
- A general monitoring dashboard or machine-learning operations product without a scientific failure-surface or test-selection contribution.
- A promise to isolate causal effects when multiple unobserved changes occur without adequate intervention or provenance.
- Measurement-error science as the primary thesis; that is N7, although N7 methods may serve this direction.
- A requirement to monitor one named proprietary model provider or one commercial application programming interface.
- A requirement to use one particular dynamic-red-team generator or adaptive-testing algorithm.
- Runtime selective action by an agent; that is N1.
- Combining version-level assurance with within-trajectory step attribution unless a genuinely unified formalism is introduced and separately approved as a redefined candidate.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| D02-04 — Change-Attributed Continual Assurance for Clinical Foundation-Model Systems | Versioned failure surface; paired component perturbation; regression discovery; change attribution; sequential test allocation; failure lineage | Complete scientific source for the normalized singleton | Within-run step localization; one particular model family, benchmark, or clinical task |

N4b and N4a share a broad assurance/failure-attribution family but remain distinct dissertation directions because their causal units and decisive experiments differ.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Represent versioned failure surfaces and change factors | Can clinically meaningful failures, system versions, changed factors, and uncertainty be represented so regression and lineage are measurable? | Develop failure ontology, version/factor model, paired test bank, and reference changes | A versioned failure surface is a valid object beyond aggregate accuracy | Reproducible failure classes, controlled/injected ground truth, transfer analysis, and calibrated measurement of change |
| Aim 2 — Detect regressions efficiently under a budget | Can sequential, coverage-aware test selection discover consequential regressions earlier than static, random, or accuracy-focused testing? | Adaptive test selection with coverage, risk, and false-alarm constraints | Structured failure coverage improves detection efficiency | Better time-to-detection and recall of clinically significant regressions at matched test cost, with prospective thresholds |
| Aim 3 — Attribute regressions to system changes | Can detected failures be localized to responsible model, retrieval, tool, prompt, policy, or population changes with defensible uncertainty? | Paired factor interventions, change attribution, and failure-lineage updates | Version-aware attribution provides actionable information beyond detection alone | Higher attribution accuracy on known/injected changes and useful uncertainty under coupled changes across releases |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a pair or sequence of compound clinical-system versions with controlled or documented changes and a test bank stratified by failure mechanism.
- **Strongest comparator:** a full static benchmark rerun, a simple stratified regression suite, random or uncertainty-based test sampling, undirected dynamic red-teaming, and accuracy-focused computerized adaptive testing.
- **Primary thesis-relevant outcomes:** time or test budget to detect a clinically significant regression, regression recall at fixed budget, false-alarm rate, attribution accuracy, calibration, and failure-lineage fidelity.
- **Supporting result pattern:** the proposed method detects important regressions with fewer tests and attributes them to changed factors more accurately than serious baselines across more than one release sequence or system configuration.
- **Defeating result pattern:** simple stratified suites or existing adaptive/dynamic methods are prospectively equivalent; attribution collapses under realistic coupled changes; adjudication noise overwhelms signal; or the failure-surface representation does not transfer.

## 8. Inherited dangerous prior art

These inherited sources are starting points, not established collision dispositions.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| `LIT-032` | Pan et al., dynamic red-teaming for health and medicine, DOI `10.1038/s44360-026-00152-8` | Already claims dynamic, automatic, systematic evaluation that evolves with models | SCREENED | Does it track versioned failure lineage or attribute regressions to changed components? |
| Unregistered, DOI `10.18653/v1/2026.acl-long.1218` | Zhang et al., dynamic medical diagnostic evaluation | Dynamic benchmark generation and reevaluation of model performance | Day 1 page/abstract characterization | Does its dynamic evaluation already provide version-aware regression attribution? |
| Unregistered, DOI `10.1038/s41746-026-02671-w` | Zheng et al., computerized adaptive testing for cost-effective medical-model evaluation | Directly addresses efficient test selection under budget | Day 1 relevant-section characterization | Can standard adaptive testing match failure-coverage-aware selection and regression detection? |
| Unregistered, arXiv `2604.23954` | Bilionis et al., risks of artificial-intelligence model updates using clinical data | Directly studies instability, arbitrariness, and fairness after updates | Day 1 abstract/page characterization | Does it offer a general failure-surface and attribution method or only empirical update-risk analysis? |
| Unregistered | Chang et al., iterative benchmark across model versions | Reports version reversals and longitudinal evaluation | Day 1 source characterization | Does it already maintain failure lineage or identify responsible changes? |
| Unregistered | *DyReMe* or related dynamic medical evaluation | Dynamic generation of diagnostic evaluations | Day 1 source characterization | Is N4b novel beyond dynamic item generation plus standard regression testing? |
| Source family | Software regression testing, change-impact analysis, causal debugging, fault localization, sequential experimental design, active testing, reliability growth models | Mature parent disciplines may contain the central attribution and budget-allocation machinery | Not comprehensively searched on Day 1 | Does clinical adaptation provide an independent scientific contribution or only a new application? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether versioned attribution adds science beyond dynamic red-teaming, adaptive testing, and standard regression suites | KT1/KT4 | Could remove both novelty and methodological necessity | Central Day 1 rejection trigger; unresolved |
| Whether changed components can be isolated under realistic coupled releases | KT3 | Attribution may be unidentifiable without controlled interventions | Controlled variants are plausible; operational releases may remain confounded |
| Whether failure taxonomies and test coverage transfer across versions | KT6/ST2 | Non-transfer would reduce the method to repeated benchmark rebuilding | Unresolved |
| Whether judge/adjudicator drift and label noise dominate regression detection | KT3 | Could make the target measurement unreliable | Recognized but not empirically resolved |
| Whether detection, budgeted selection, and attribution form one thesis | KT2/ST1 | Could become several assurance projects | Day 1 framed them as one efficient attributed-assurance thesis; requires attack |
| Whether sufficient release histories or controlled compound-system variants are available | KT5 | Necessary for convincing evaluation | Synthetic/injected changes appear feasible; real histories uncertain |
| Whether rapid advances commoditize dynamic evaluation faster than the dissertation can contribute | KT6 | High moving-field risk | The versioned attribution object may remain structural; unresolved |

## 10. Feasibility assumptions inherited from Day 1

- Controlled system variants and injected changes can provide an executable minimum path with known change provenance.
- Public model releases, open retrieval corpora, configurable tools, prompts, and policies can instantiate compound-system changes without access to proprietary internals.
- A clinically meaningful test bank and failure ontology can be constructed or adapted from public benchmarks.
- Repeated evaluation is computationally feasible at a bounded research scale; full frontier-model retraining is not assumed.
- Expert adjudication can be limited to clinically consequential failures and uncertainty calibration; no access commitment is inferred.
- Historical or prospective external system-version data would strengthen validation but is not assumed as the sole path.

## 11. Packet provenance and change control

### Direct compressions

- The central object, exact thesis, failure conditions, source set, and critical uncertainty are compressed from D02-04.
- The focus on fixed-budget detection, factor attribution, and failure lineage is preserved directly.

### Reconciled formulations

- The aims separate representation, efficient detection, and attribution as tests of one versioned-assurance thesis.
- The packet makes adjudication noise explicit while preserving it as a measurement issue rather than converting N4b into N7.

### Unresolved candidate-definition tension

Round 3 noted that a unified counterfactual-attribution formalism spanning N4a and N4b might be possible, but it would constitute a redefined hypothesis. Fidelity reviewers must ensure this packet remains strictly version/component-level and does not silently absorb within-trajectory attribution.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
