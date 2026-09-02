# N3 Candidate Evaluation Packet

- **Candidate identifier:** N3
- **Candidate title:** Machine-Checkable Causal Data-Fitness for Target-Trial Emulation
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifacts and sections:** `analysis/analysis_01/day1_candidate_generation_v2.md` C3; `analysis/analysis_02/day1_candidate_generation_v2.md` D02-03
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N3 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **typed, machine-checkable causal data-fitness contract and deterministic evaluation mechanism** that maps a proposed target-trial causal question and a specific Electronic Health Record data-generating process to one of several auditable outputs:

- supported as specified;
- supported only under a restricted or revised estimand;
- requires additional information or design clarification;
- not supported by the available data.

The contract represents target-trial elements, causal assumptions, temporal observability, data provenance, operational definitions, and executable diagnostics. A language model may translate prose into the contract, but the dissertation's durable object is the explicit semantics and validity-aware decision process, not generic code generation.

## 2. Exact falsifiable thesis

> A typed causal data-fitness contract that jointly encodes the target-trial protocol, causal assumptions, temporal observability, data provenance, and executable diagnostics will identify invalid or estimand-altering Electronic Health Record target-trial emulations, recommend defensible restriction, revision, information requests, or refusal, and reduce causal estimation error and false assurance relative to reporting checklists, direct language-model automation, and code-generation pipelines while preserving automation for questions genuinely supported by the data.

The thesis is defeated or materially weakened if:

- contract judgments do not predict bias, estimand mismatch, or invalidity in settings with controlled or otherwise defensible truth;
- the machine-checkable portion is too shallow while the decisive causal assumptions remain untestable and merely restated;
- qualified experts cannot agree on contract semantics or allowable outputs;
- standard diagnostics and well-designed checklists are prospectively equivalent;
- substantially equivalent contract/compiler or validity-gating systems already exist;
- automation can produce polished contracts without improving causal validity.

## 3. Included scientific scope

The common Phase 1 target includes:

1. A formal representation of target-trial elements and their mapping to available data.
2. Explicit separation between testable data conditions, diagnosable design defects, and untestable causal assumptions.
3. Temporal observability and alignment of eligibility, treatment assignment, time zero, follow-up, outcomes, and covariates.
4. Provenance for data elements, operational definitions, and transformations.
5. Executable diagnostics or static checks compiled from the contract where scientifically valid.
6. Explicit outcomes including support, restricted estimand, required information, revision, and refusal.
7. Evaluation under known or partially known truth using simulation, emulated data-generating processes, negative controls, benchmark cases, or expert adjudication.
8. Comparison with reporting checklists, standard diagnostics, direct language-model assistance, and existing target-trial automation systems.
9. An auditable interface through which a language model or other system may propose a contract while deterministic or formally constrained machinery evaluates it.

## 4. Explicitly excluded scientific scope

The following are not part of N3's mandatory identity:

- A claim that all causal identifiability assumptions can be empirically verified or certified.
- Generic automation of target-trial emulation, cohort construction, causal coding, or statistical estimation without a new data-fitness formalism.
- Autonomous end-to-end causal discovery.
- A promise that a passing contract proves an unbiased causal estimate.
- A requirement to use a multi-agent architecture or any particular foundation model.
- General claim-evidence verification; that is N6.
- Generic clinical data quality checking unrelated to a specified causal estimand.
- Replacing causal experts or eliminating human review for assumptions that cannot be machine-resolved.
- A single disease or institutional dataset as the scientific contribution.
- Commercial workflow automation as a substitute for methodological novelty.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S01-C3 — Data-Fitness-Aware Autonomous Target-Trial Emulation | Machine-readable validity representation; data-fitness and identifiability checker; revision/abstention policy; audit trace | Agent-facing workflow and selective-action formulation | A fully autonomous agent; generic pipeline automation; every original workflow component |
| D02-03 — Machine-Checkable Causal Data-Fit Contracts for Electronic Health Record Target-Trial Emulation | Typed contract language; deterministic compiler/checker; explicit assumption status; restricted-estimand and refusal outputs | Formal methodological core | That every causal condition is machine-testable; any one language-model translation mechanism |

The formulations are **same direction at two levels of formalization**. The contract/checker is the durable object; agentic translation is an interface or implementation variant.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Define contract semantics and benchmark validity states | Which target-trial and data-generating-process properties can be represented, checked, bounded, or explicitly marked untestable? | Formal language/ontology, compiler semantics, benchmark cases, and expert agreement | A machine-checkable data-fitness object can be defined without implying causal certification | Expressiveness analysis, expert agreement, diagnostic coverage, and clear boundaries between testable and untestable claims |
| Aim 2 — Build validity-aware checking and selective design revision | Can the contract correctly return supported, restricted, requires-information, or not-supported decisions and recommend defensible revisions? | Deterministic checks plus constrained completion/translation where appropriate | Explicit contracts improve validity decisions beyond checklists and direct automation | Better detection of unsupported designs and estimand drift; calibrated refusal/restriction; ablations of each contract component |
| Aim 3 — Test causal consequences and transfer | Do contract decisions predict bias or mismatch and improve end-to-end emulation validity across data environments and questions? | Simulation/controlled truth, multi-dataset validation, and prospective or retrospective expert comparison | Data-fitness reasoning reduces causal error and false assurance in practice | Lower causal estimation error or invalid-design rate, improved traceability, and defensible boundary conditions across settings |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a target-trial specification paired with a data-generating process and an available-data representation, including controlled violations and estimand-altering limitations.
- **Strongest comparator:** an expert-designed reporting/checklist workflow plus standard diagnostics, and a strong language-model or target-trial automation system with equivalent access to the specification and data dictionary.
- **Primary thesis-relevant outcomes:** correct support/restriction/refusal decision, estimand-mismatch detection, calibration of uncertainty/refusal, causal estimation error under known truth, and false-assurance rate.
- **Supporting result pattern:** the contract/checker detects consequential unsupported designs and estimand changes missed by checklists or direct automation, while retaining supported analyses and producing auditable reasons across multiple data environments.
- **Defeating result pattern:** checklists/standard diagnostics are prospectively equivalent; contract decisions do not predict bias; expert semantics are irreproducible; or the supposedly machine-checkable conditions reduce to superficial completeness checks with no causal consequence.

## 8. Inherited dangerous prior art

These are inherited targets rather than preclassified collisions. Phase 1 must inspect them and relevant parent literatures independently.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| Unregistered Day 1 source | Wang et al., conceptual account of data-constrained target-trial feasibility | Closest conceptual treatment of whether a target trial can be realized from available data | Day 1 page/section characterization | Does it already define an executable contract or only conceptual guidance? |
| Unregistered, official system/paper | *THESEUS*, language-model-assisted standardization to Observational Health Data Sciences and Informatics/Strategus specifications | Closest executable language-model-assisted target-trial workflow | Day 1 relevant-section characterization | Does it already validate data fitness, estimand change, and refusal, or primarily standardize fields and code? |
| Unregistered | *TrialEmulation* implementation infrastructure | Existing reusable target-trial emulation tooling | Day 1 source characterization | Would N3 be merely an additional preflight layer around established infrastructure? |
| Unregistered | *TrialCalibre* multi-agent observational-calibration proposal | Direct collision with broad autonomous causal-agent framing | Day 1 page/abstract characterization | Does it contain machine-checkable validity semantics and selective refusal or only an agentic workflow concept? |
| Unregistered | *CausalReasoningBenchmark* | Evaluates automated causal identification and reveals difficulty specifying full identification details | Day 1 relevant-section characterization | Does benchmark/task design already provide the formal object and evaluation needed for N3? |
| Source family | Target-trial emulation guidance, reporting checklists, estimand frameworks, data-quality diagnostics, cohort-method tooling | Strong simple alternatives and mature domain methodology | Partially inspected during Day 1 | Can a contract add science beyond encoding existing guidance? |
| Source family | Causal programming languages, probabilistic programming, causal query compilers, automated identification, formal specification, static analysis | Parent disciplines may already provide the core contract/compiler idea | Not comprehensively searched on Day 1 | Is N3 a domain-specific relabeling of existing formal methods? |

Exact bibliographic identities not fully registered in the Day 1 sources must be resolved during Phase 1 rather than guessed in this packet.

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether contract/compiler systems already exist in causal programming, formal methods, or target-trial tooling | KT1 | Could preempt the central object | Day 1 search was limited; unresolved |
| Which validity conditions can be machine-checked without claiming causal certification | KT3 | The scientific object fails if decisive judgments are unobservable or merely expert opinion encoded as software | Central unresolved conceptual question |
| Whether experts can agree on contract semantics, restricted estimands, and refusal conditions | KT3/KT5 | Unreliable semantics would undermine benchmark and evaluation | Unresolved |
| Whether checklists and standard diagnostics are practically equivalent | KT4 | Equivalent simple methods would remove methodological necessity | Proposed comparison only |
| Whether causal-error reduction can be evaluated with credible truth | KT3 | The thesis requires more than syntactic correctness | Simulation and benchmark truth appear plausible; real-world validation remains difficult |
| Whether the aims remain one contract-validity thesis rather than formal language, agent interface, and empirical causal study | KT2/ST1 | Overbreadth could require material narrowing | Round 3 found strong identity alignment, but Phase 1 must attack it |
| Whether sufficient causal-method expertise and multiple data environments are available | KT5 | Necessary for valid design and external evaluation | Plausible but not guaranteed; no commitment inferred |

## 10. Feasibility assumptions inherited from Day 1

- Public target-trial examples, synthetic data-generating processes, and simulated violations can support an initial benchmark with known truth.
- Existing open-source causal and Observational Health Data Sciences and Informatics tooling can serve as implementation substrates and baselines.
- Qualified causal-inference expertise can be incorporated into design and adjudication; no individual availability is assumed.
- At least one external data environment or materially different simulation family can be used to test transfer.
- Restricted institutional data may strengthen validation but is not assumed to be the only executable path.
- The project can represent untestable assumptions explicitly rather than falsely resolving them.

## 11. Packet provenance and change control

### Direct compressions

- The contract/checker object, four-way decision outputs, major failure conditions, dangerous prior-art categories, and critical uncertainties come from S01-C3 and D02-03.
- The distinction between causal validity checking and generic target-trial automation is preserved directly.

### Reconciled formulations

- The exact thesis adopts D02-03's formal contract/compiler semantics while retaining S01-C3's validity-aware revision, refusal, and audit-trace interface.
- The common aims formalize the shared three-stage architecture: semantics/benchmark, checking/selective revision, and causal consequence/transfer.

### Unresolved candidate-definition tension

The phrase `machine-checkable causal data-fitness` must not imply that untestable causal assumptions can be certified. Fidelity reviewers should assess whether the packet's explicit testable/untestable boundary preserves the candidate or narrows it materially.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
