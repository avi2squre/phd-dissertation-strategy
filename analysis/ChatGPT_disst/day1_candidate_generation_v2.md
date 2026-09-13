# Analysis Stream 01 — Day 1 Candidate Generation — Common Analysis Schema v2

> **FORMAT-NORMALIZED DERIVATIVE OF FROZEN BLIND FIRST PASS. NO NEW SCIENTIFIC ANALYSIS PERFORMED.**
>
> Original frozen artifact: `analysis/analysis_01/day1_candidate_generation.md`  
> Original repository base SHA: `86230f478b0a47a0198adbe325c42b0561fe8288`  
> Original frozen-artifact branch: `analysis/stream01-day1-blind`  
> Original frozen-artifact blob SHA: `81c3de3603b8c9168c34c84501aa89ee93bb2af1`  
> Normalization rule: scientific content, candidate definitions, evidence interpretations, aims, verdicts, and portfolio conclusions are preserved. New v2 fields are populated only by extracting or compressing reasoning already present in the frozen artifact.

# Layer I — Executive navigation

## A. Analysis metadata

- **Date:** 2026-08-31
- **Analysis stream:** `analysis_01`
- **Repository SHA used:** `86230f478b0a47a0198adbe325c42b0561fe8288`
- **Analysis status:** **FROZEN — BLIND FIRST PASS**
- **Permitted inputs used:** root `README.md`; `OPERATING_PROTOCOL.md`; `decisions/decision_log.md`; `context/user_goals_and_constraints.md`; `context/advisor_landscape.md`; shared literature registry where already known; Stream 01 historical provenance as prior context; targeted public literature searches performed on 2026-08-31.
- **Inputs deliberately excluded:** new Day 1 outputs from Streams 02 and 03; substantive Stream 02/03 conclusions as candidate-generation inputs; existing `candidate_programs/` as an answer key; canonical weighted scoring during candidate generation.
- **External-search scope:** targeted, non-systematic literature retrieval focused on 2025–2026 work on clinical AI agents, abstention/selective prediction, neuro-symbolic biomedical AI, longitudinal clinical reasoning, dynamic/process-aware agent evaluation, and agentic target-trial emulation / real-world evidence.
- **Parallelism:** no multi-agent decomposition; one reasoning process plus targeted retrieval.
- **Stopping condition:** stop after 3–4 sufficiently specified candidate dissertation directions are generated and additional Day 1 searching is unlikely to change which directions deserve adversarial review on Day 2.

## B. Repository-convention declarations

1. **Question evaluated:** Which 3–4 literature-informed, falsifiable dissertation research directions appear strong enough to deserve adversarial Day 2 review?
2. **Evidence used:** the permitted repository context above plus targeted current public literature.
3. **Key assumptions:** candidate directions should be methodologically substantive, falsifiable, feasible enough for a Health Informatics PhD, and capable of surviving stronger foundation models where possible.
4. **Recommendation and uncertainty:** candidate-specific verdicts below are preliminary within-stream triage judgments, not canonical selections.
5. **Other analyses consulted:** no new Stream 02 or Stream 03 Day 1 outputs or substantive conclusions were used as candidate-generation inputs.
6. **Accepted decisions challenged:** none in the frozen Day 1 artifact.

## C. Candidate overview table

| ID | Candidate dissertation direction | Central scientific object | Day 1 verdict | Critical uncertainty / rejection trigger |
|---|---|---|---|---|
| C1 | Evidence-State Control for Selective Clinical AI Agents | Typed evidence-state representation + selective-action controller + process-aware evaluation protocol | ADVANCE WITH MAJOR UNCERTAINTY | Whether this is genuinely new beyond belief-state estimation, POMDPs, selective prediction, active sensing, and general agent-controller research. |
| C2 | Temporally Constrained Diagnostic-State Reasoning from Longitudinal EHRs | Diagnostic-state representation + temporal transition constraints + trajectory-consistency objective/benchmark | ADVANCE WITH MAJOR UNCERTAINTY | Whether diagnostic-state transitions are already captured by temporal KG, probabilistic graphical-model, or sequential-diagnosis literature, or cannot be labeled reliably. |
| C3 | Data-Fitness-Aware Autonomous Target-Trial Emulation | Machine-readable TTE validity representation + data-fitness/identifiability checker + revision/abstention policy | ADVANCE | Whether the AI-methodological contribution exceeds deterministic causal rules/checklists and established TTE operational guidance. |
| C4 | Process-Aware Dynamic Assurance and Failure Localization for Clinical AI Agents | Failure ontology + critical-step localizer + counterfactual replay/intervention + dynamic stress generator | HOLD | Whether causal critical-step attribution remains a defensible gap beyond MedCTA, DAS, AgentRx, and related 2026 work. |

The table is a navigation map, not a canonical ranking.

---

# Layer II — Full candidate analysis

# C1 — Evidence-State Control for Selective Clinical AI Agents

## 1. Candidate identity

**Title:** Evidence-State Control for Selective Clinical AI Agents

**One-sentence identity:** Develop explicit, structured representations of an agent’s evidentiary state and a decision-theoretic controller that chooses among answering, retrieving, verifying, revising, asking, or deferring during sequential clinical reasoning.

## 2. Central scientific object

A **typed evidence-state representation**, a **selective-action controller**, and a **process-aware evaluation protocol** for choosing among answer / retrieve / verify / revise / ask / defer actions under heterogeneous uncertainty.

## 3. Central scientific problem

Current medical LLMs and agentic systems can be highly capable yet still overcommit under uncertainty, fail to exploit tools reliably, and provide only modest gains over strong base models in sequential clinical tasks. Existing work increasingly measures abstention, uncertainty, tool use, and reflection, but these components are often evaluated separately. The deeper problem is **selective control under heterogeneous uncertainty**: when an autonomous clinical agent is missing evidence, facing contradictory evidence, outside validated conditions, or uncertain about a tool result, how should it decide what action to take next?

This matters because a safe autonomous agent is not merely one that knows when it is uncertain. It must choose an appropriate corrective action conditioned on *why* it is uncertain and what evidence is available.

## 4. Falsifiable dissertation thesis

**Proposed research hypothesis:**

> Explicit, structured evidence-state representations combined with a learned or decision-theoretic selective controller will reduce unsafe commitment and improve cost-adjusted task utility relative to uncertainty-only, confidence-threshold, and generic reflection/tool-routing baselines in sequential clinical reasoning.

This thesis can be falsified if structured evidence-state control does not outperform simpler uncertainty or orchestration baselines after controlling for model capability and tool access.

## 5. Evidentiary basis

### Source-supported finding
**Claim:** Medical LLMs systematically overcommit under uncertainty and rarely abstain even when essential question information is removed.  
**Source:** Cocchieri et al., *LLMs (Almost) Never Abstain Under Medical Uncertainty*, ACL 2026, DOI `10.18653/v1/2026.acl-long.1365` (existing `LIT-026`).

### Source-supported finding
**Claim:** Clinical agent benchmarks reveal large performance degradation in sequential settings and substantial variability in whether agents benefit from retrieval, reflection, and persistent notes.  
**Source:** Schmidgall et al., *AgentClinic*, npj Digital Medicine 2026, DOI `10.1038/s41746-026-02674-7`.

### Source-supported finding
**Claim:** Contemporary agentic systems can yield only modest gains over baseline LLMs despite tool access, leaving reliability and orchestration unresolved.  
**Source:** Liu et al., *Benchmarking large language model-based agent systems for clinical decision tasks*, npj Digital Medicine 2026, DOI `10.1038/s41746-026-02443-6` (existing `LIT-030`).

### Source-supported finding
**Claim:** Recent decision-theoretic healthcare abstention work explicitly frames abstention as a safety-relevant decision problem rather than merely a calibration metric.  
**Source:** Presacan et al., *When silence is safer: a review and decision-theoretic framework for LLM abstention in healthcare*, npj Digital Medicine 2026, DOI to verify in shared registry before canonical use.

### Cross-paper inference
Current work establishes the importance of abstention, sequential tool use, and agent reliability separately. It does not yet establish that a **typed evidence-state representation** is the right sufficient statistic for choosing among multiple corrective actions.

## 6. Closest and dangerous prior work

1. Cocchieri et al. 2026, MedQAbstain — dangerous prior art for abstention-specific claims.
2. Presacan et al. 2026 — dangerous prior art for decision-theoretic abstention framing.
3. AgentClinic — dangerous prior art for sequential decision making, reflection, retrieval, and persistent-state evaluation.
4. Liu et al. 2026 — dangerous prior art for planner–executor–verifier agent benchmarking.
5. General agent-controller and selective-prediction literature outside medicine — must be searched aggressively on Day 2 because the core contribution may already exist under non-medical terminology.

## 7. Evidence-supported limitations of existing approaches

### Directly supported
- MedQAbstain shows that strong medical LLMs rarely abstain under constructed uncertainty.
- AgentClinic shows that static QA performance does not transfer cleanly to sequential clinical decision environments.
- Liu et al. show that adding agentic infrastructure and tools does not guarantee large gains.

### Inferred limitation
Current clinical work does not appear to provide a general, explicit state representation distinguishing failure modes such as missing evidence, contradictory evidence, unverifiable evidence, distributional mismatch, tool failure, and unresolved causal assumptions, together with a controller mapping those states to corrective actions.

## 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

A potentially unresolved gap is the absence of a rigorously evaluated **evidence-state control layer** for clinical agents that represents *why* the system should not yet commit and uses that representation to choose among distinct actions rather than collapsing all uncertainty into a scalar confidence or binary abstention decision.

Day 2 must search general AI, selective prediction, POMDP, active information acquisition, metacognitive control, and agent-routing literature to determine whether this is genuinely new or simply renamed existing decision theory.

## 9. Proposed methodological contribution

1. **Evidence-state representation:** a typed, structured state containing support, contradiction, missingness, provenance quality, tool reliability, temporal freshness, and task-specific validity signals.
2. **Selective-action controller:** a policy choosing answer / retrieve / verify / revise / ask / defer under explicit utility and cost functions.
3. **Evaluation protocol:** process-aware metrics that distinguish correct commitment, appropriate information acquisition, unnecessary escalation, and unsafe overcommitment.

The dissertation novelty should live in the representation/control problem, not in merely wiring tools together.

## 10. Coherent dissertation aims

### Aim 1 — Represent and measure evidentiary state
**Question:** Can clinically meaningful evidence states be operationalized and annotated reliably?  
**Method:** Define a typed evidence-state schema; construct benchmark cases with controlled missing, contradictory, stale, or low-quality evidence.  
**Experiment:** Compare evidence-state classifiers/estimators against confidence-only and uncertainty baselines.  
**Expected evidence:** Improved prediction of when the current agent answer/action is unsafe or incomplete.

### Aim 2 — Learn selective corrective actions
**Question:** Does explicit evidence state improve action selection?  
**Method:** Develop rule-based, decision-theoretic, and learned controllers over the same evidence-state interface.  
**Experiment:** Compare with direct answering, confidence thresholding, generic self-reflection, fixed retrieval, and planner–executor–verifier baselines.  
**Expected evidence:** Lower unsafe-commitment rate and higher utility at matched latency/cost.

### Aim 3 — Generalize across models/tasks
**Question:** Does the control mechanism transfer across model families, specialties, and task types?  
**Method:** External validation on clinical QA, longitudinal chart reasoning, and tool-use benchmarks.  
**Experiment:** Frozen-controller transfer and adaptation studies.  
**Expected evidence:** Benefits persist beyond one base model or benchmark.

## 11. Publication decomposition

1. **Paper 1:** Evidence-state taxonomy + benchmark/measurement study.
2. **Paper 2:** Selective controller method + ablations.
3. **Paper 3:** Cross-model/task generalization and human-in-the-loop evaluation.

If Aim 3 fails, Aims 1–2 could still yield a defensible methodological dissertation if the representation and controller are strong. If Aim 1 cannot be annotated reliably, the entire direction is substantially weakened.

## 12. Evaluation strategy

- AgentClinic and comparable sequential clinical benchmarks.
- MedQAbstain-derived uncertainty conditions.
- Custom controlled perturbations for evidence missingness, contradiction, provenance degradation, and tool failure.
- Baselines: direct LLM, calibrated confidence/entropy, conformal/selective prediction where applicable, binary abstention, fixed retrieve-then-answer, generic reflection, planner–executor–verifier.
- Metrics: selective risk, coverage, unsafe-commitment rate, action appropriateness, calibration, utility under action/latency cost, tool-call efficiency, failure recovery.
- Human clinician adjudication for ambiguous action appropriateness on a limited validation set.

## 13. Required resources and feasibility

### Known available
- Public clinical QA and agent benchmarks.
- General software/tooling for agent orchestration.

### Plausibly available
- Public or synthetic longitudinal cases for controlled perturbations.
- Clinician/domain-expert review through local collaborations.

### Currently uncertain
- Sufficient expert annotation capacity for evidence-state labels.
- Access to realistic restricted clinical workflows for external validation.

The first publishable unit can be built largely from public/synthetic data, reducing dependence on restricted resources.

## 14. Novelty-collision risks

- “Evidence state” may reproduce concepts from belief-state estimation, POMDPs, selective prediction, active sensing, or metacognitive control under new terminology.
- Decision-theoretic abstention work may already cover much of the proposed controller.
- Strong frontier models may improve self-assessment enough that explicit state adds little.
- Reviewer objection: state labels may be hand-engineered abstractions without demonstrated causal utility.
- Reviewer objection: gains may come from extra retrieval/tool calls rather than the state representation.

## 15. Advisor / expertise complementarity

**Required expertise preserved from the frozen artifact:**
- biomedical NLP / LLM agents / knowledge grounding;
- decision theory, uncertainty, causal/statistical reasoning, or sequential decision making;
- clinical informatics evaluation and workflow design.

The frozen artifact states that this direction benefits from complementarity between biomedical-agent expertise and a primary advisor with stronger formal/statistical or decision-theoretic methods.

**Specific IHI primary-advisor name(s): NOT PRESENT IN ORIGINAL FROZEN ARTIFACT.**

## 16. Foundation-model resilience

Moderately high. If frontier models become stronger, the research object remains the **policy for acting under evidence constraints**, not raw answer generation. However, resilience depends on demonstrating that explicit state/control adds value beyond increasingly capable native self-monitoring.

## 17. Publication and execution risk

- **Novelty bar:** High; adjacent general-AI literature is likely extensive.
- **Time to first paper:** Moderate; benchmark/taxonomy work could start quickly.
- **Single risky dependency:** Annotation validity of evidence states.
- **Ground truth difficulty:** Moderate to high.
- **Reproducibility:** Good if built on public benchmarks and frozen policies.
- **Moving-field risk:** High.

## 18. Generalizability

### Healthcare-specific
Clinical evidence semantics, risk utility, provenance, and escalation rules.

### Transferable
Selective action under incomplete/contradictory evidence, tool routing, active information acquisition, process-aware reliability.

## 19. Strongest reason to reject the direction

The core idea may already be well captured by existing sequential decision theory, selective prediction, and agent-controller research; “artificial metacognition” could become relabeling rather than a new method.

## 20. Evidence that would change the recommendation

**Strengthen:** A Day 2 search showing that existing abstention/controller work largely uses scalar uncertainty or terminal abstention and lacks typed evidence-state control over multiple corrective actions.  
**Weaken:** General-agent literature demonstrating essentially the same representation and action policy.  
**Kill:** Evidence that explicit state adds no value over calibrated uncertainty or simple retrieve/abstain baselines across strong models.

## 21. Day 1 verdict and verdict rationale

**ADVANCE WITH MAJOR UNCERTAINTY**

The direction has a clean falsifiable thesis, strong relevance to autonomous-system reliability, good publication decomposition, and substantial cross-domain transfer potential. Its main risk is novelty collision with general sequential-decision and selective-prediction literature.

## 22. Critical uncertainty / rejection trigger

Whether general sequential-decision, selective-prediction, belief-state, or agent-controller literature already captures essentially the same representation/action policy, or explicit evidence state adds no value over simpler calibrated uncertainty/retrieve/abstain baselines.

---

# C2 — Temporally Constrained Diagnostic-State Reasoning from Longitudinal EHRs

## 1. Candidate identity

**Title:** Temporally Constrained Diagnostic-State Reasoning from Longitudinal EHRs

**One-sentence identity:** Develop a neuro-symbolic representation and inference framework that tracks how diagnostic hypotheses should evolve across longitudinal clinical evidence and constrains unsupported transitions between suspected, ruled-out, provisional, and confirmed states.

## 2. Central scientific object

A **diagnostic-state ontology/representation**, **temporal transition model**, **trajectory-consistency objective**, and **trajectory benchmark** for evidence-conditioned longitudinal diagnostic reasoning.

## 3. Central scientific problem

Clinical reasoning unfolds over time. Diagnoses move through states as evidence accumulates, tests return, contradictory findings emerge, and treatment responses become known. Yet many LLM evaluations reduce longitudinal records to static prediction or summary tasks. A model can produce the correct final diagnosis while misrepresenting *when* evidence justified that conclusion, inventing certainty too early, failing to preserve unresolved alternatives, or ignoring contradictory evidence.

The methodological problem is therefore not simply temporal language modeling. It is **state-transition fidelity under evolving evidence**.

## 4. Falsifiable dissertation thesis

> Explicit diagnostic-state representations plus temporally grounded symbolic transition constraints will reduce unsupported diagnostic-state changes and improve longitudinal reasoning fidelity relative to unconstrained LLM, retrieval-only, and generic temporal-model baselines.

The thesis is falsified if structured constraints do not improve trajectory-level fidelity or merely trade errors for excessive conservatism.

## 5. Evidentiary basis

### Source-supported finding
**Claim:** LLMs struggle with longitudinal EHR reasoning; TIMER was created specifically to model/evaluate instruction-following over longitudinal records.  
**Source:** Cui et al., *TIMER: temporal instruction modeling and evaluation for longitudinal clinical records*, npj Digital Medicine 2025, DOI `10.1038/s41746-025-01965-9`.

### Source-supported finding
**Claim:** Sequential clinical decision-making is substantially more difficult than static QA and requires interaction under incomplete information.  
**Source:** AgentClinic, DOI `10.1038/s41746-026-02674-7`.

### Source-supported finding
**Claim:** Neural-symbolic agent architectures can improve an explicitly structured biomedical task by separating neural interpretation from symbolic/deterministic linking.  
**Source:** Zhang et al., *A neural-symbolic AI agent system for biomedical concept mapping*, npj Digital Medicine 2026, DOI `10.1038/s41746-026-02594-6` (existing `LIT-029`).

### Source-supported finding
**Claim:** A recent medical NeSy roadmap argues that integration of data-driven inference with explicit clinical knowledge may improve transparency/accountability and identifies multiple architecture types.  
**Source:** Wong et al., *Neuro-symbolic artificial intelligence in medicine*, Nature Biomedical Engineering 2026, DOI `10.1038/s41551-026-01728-1` (existing `LIT-027`).

### Source-supported finding
**Claim:** Longitudinal health-agent research emphasizes follow-up, coherent reasoning over time, and sustained accountability as distinct requirements.  
**Source:** Lin et al., *A framework for longitudinal health AI agents*, Nature Health 2026; DOI to verify before canonical reuse.

### Cross-paper inference
These literatures motivate temporal reasoning and structured neuro-symbolic control, but do not by themselves establish that explicit **diagnostic-state transition constraints** are a novel or superior representation.

## 6. Closest and dangerous prior work

1. TIMER — dangerous prior art for longitudinal EHR reasoning and temporal instruction tasks.
2. AgentClinic — dangerous prior art for sequential diagnosis and interactive evidence acquisition.
3. MCM neural-symbolic concept mapping — dangerous prior art for claiming novelty merely from neural + symbolic integration.
4. Longitudinal health-agent frameworks — dangerous prior art for broad longitudinal-agent claims.
5. Temporal knowledge graphs / temporal clinical event modeling — major Day 2 search target.

## 7. Evidence-supported limitations of existing approaches

### Directly supported
- Static benchmark performance poorly captures sequential clinical reasoning difficulty.
- Longitudinal EHR tasks present temporal-ordering and context-integration challenges.
- Existing neural-symbolic biomedical work often targets bounded mapping/verification tasks rather than evolving diagnostic belief trajectories.

### Inferred limitation
Current systems appear to lack an explicit normative layer for whether a diagnostic-state transition was justified by the evidence available **at that time**, as distinct from whether the final answer is retrospectively correct.

## 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

A potentially unresolved problem is trajectory-level diagnostic reasoning in which the system must maintain explicit candidate states, evidence provenance, and temporal transition constraints, and is evaluated against the evidence actually available at each step rather than only the endpoint diagnosis.

Day 2 must aggressively search clinical NLP, temporal KGs, probabilistic graphical models, disease-progression models, sequential diagnosis, and diagnostic-process mining to determine whether the proposed representation is truly novel.

## 9. Proposed methodological contribution

1. **Diagnostic-state ontology/representation**: suspected, possible, provisional, confirmed, ruled-out, historical, conflicting, unknown, with confidence/evidence provenance.
2. **Temporal transition model**: rules or learned constraints governing allowable state changes given new evidence.
3. **Trajectory-consistency objective**: penalizes premature certainty, unsupported reversals, evidence omission, and retrospective leakage.
4. **Trajectory benchmark**: evaluates correctness at each evidence horizon.

The methodological contribution must be more than adding rules after generation; ideally constraints affect inference or learning.

## 10. Coherent dissertation aims

### Aim 1 — Define and validate diagnostic-state trajectories
**Question:** Can clinical diagnostic evolution be represented consistently enough to support evaluation?  
**Method:** Create state/transition schema and annotated/synthetic benchmark episodes.  
**Experiment:** Inter-annotator agreement and comparison with simpler binary confirmed/not-confirmed labels.  
**Expected evidence:** State representation captures clinically meaningful distinctions reliably.

### Aim 2 — Develop temporally constrained inference
**Question:** Do explicit transition constraints improve longitudinal reasoning?  
**Method:** Neuro-symbolic controller or constrained decoder over evolving evidence.  
**Experiment:** Compare with unconstrained LLM, retrieval-only, temporal prompting, TIMER-like models, and KG lookup.  
**Expected evidence:** Fewer unsupported transitions and less temporal leakage at matched endpoint accuracy.

### Aim 3 — Generalize across conditions and model families
**Question:** Are benefits robust beyond one disease or dataset?  
**Method:** External validation across rare-disease and common-disease longitudinal tasks.  
**Experiment:** Cross-condition transfer and model-family ablations.  
**Expected evidence:** Transition framework generalizes or clearly identifies domain limits.

## 11. Publication decomposition

1. Diagnostic-state representation + benchmark.
2. Constrained inference method.
3. External validation / cross-condition generalization.

If the constrained method fails, Aim 1 may still produce a valuable benchmark and failure taxonomy. If the state representation itself proves unreliable, the direction should be abandoned.

## 12. Evaluation strategy

- Longitudinal EHR benchmarks such as TIMER-compatible tasks.
- Simulated evidence-release sequences to prevent retrospective leakage.
- Public longitudinal notes when legally available; restricted EHR only for later validation.
- Metrics: transition precision/recall, premature-confirmation rate, unsupported-reversal rate, temporal leakage, evidence-grounding fidelity, final diagnosis accuracy, calibration by evidence horizon.
- Baselines: standard LLM, retrieval-augmented LLM, chronological summarization, temporal language models, temporal KG methods, post-hoc rule checking.
- Ablations: remove symbolic constraints, provenance, temporal masking, state memory.

## 13. Required resources and feasibility

### Known available
- Public literature/EHR-derived longitudinal benchmarks.
- Existing biomedical KG/NLP expertise.

### Plausibly available
- Local clinical informatics expertise for annotation schema.
- Public synthetic rare-disease trajectories and guideline-derived episodes.

### Currently uncertain
- Real longitudinal EHR access and labels for state transitions.
- Cost of clinician annotation.

A public/synthetic benchmark can provide an early paper while restricted-data validation remains optional.

## 14. Novelty-collision risks

- Temporal KGs and probabilistic diagnostic-state models may already formalize similar state transitions.
- Reviewer objection: state labels could be ontology engineering rather than algorithmic novelty.
- Reviewer objection: constraints may simply enforce conservative outputs without improving useful decision-making.
- Strong LLMs with long context may reduce temporal-order errors.
- Retrospective ground truth for “when a diagnosis became justified” can be inherently ambiguous.

## 15. Advisor / expertise complementarity

**Required expertise preserved from the frozen artifact:**
- biomedical NLP / knowledge graphs / clinical LLMs;
- temporal modeling, probabilistic reasoning, or formal methods;
- clinical informatics and EHR data-generating processes.

The frozen artifact states that this direction strongly benefits from complementarity between Zhang-style biomedical NLP/KG expertise and a primary advisor with formal/statistical/temporal or clinical-data methodology.

**Specific IHI primary-advisor name(s): NOT PRESENT IN ORIGINAL FROZEN ARTIFACT.**

## 16. Foundation-model resilience

High if the contribution is a normative/evaluable representation of evidence-dependent state transitions rather than prompt engineering. Even stronger base models still face temporal provenance and decision-timing requirements. Resilience is weaker if improved long-context reasoning solves the benchmark without explicit structure.

## 17. Publication and execution risk

- **Novelty bar:** High.
- **Time to first paper:** Moderate; benchmark/state representation is tractable.
- **High-risk dependency:** Clinically meaningful annotation of state transitions.
- **Ground truth:** Difficult and potentially subjective.
- **Reproducibility:** Good with public/synthetic benchmark.
- **Moving-field risk:** High but narrower than generic agentic AI.

## 18. Generalizability

### Healthcare-specific
Diagnostic-state semantics and clinical evidence interpretation.

### Transferable
Temporal belief-state tracking, evidence-conditioned state transitions, provenance-aware sequential reasoning.

## 19. Strongest reason to reject the direction

The apparent novelty may dissolve once temporal knowledge-graph, probabilistic graphical-model, and sequential-diagnosis literature are reviewed; the proposed “diagnostic-state” representation could be a domain-specific rebranding of established temporal state-space modeling.

## 20. Evidence that would change the recommendation

**Strengthen:** Evidence that current longitudinal benchmarks emphasize final outputs and lack evidence-horizon transition validity.  
**Weaken:** Strong prior work already models diagnostic belief transitions with explicit evidence timing.  
**Kill:** No reliable clinician agreement on the target state/transition labels or no benefit beyond chronological prompting/temporal masking.

## 21. Day 1 verdict and verdict rationale

**ADVANCE WITH MAJOR UNCERTAINTY**

This is scientifically coherent and highly aligned with biomedical NLP/KG strengths, but its true novelty depends on adjacent temporal/probabilistic literature that must be searched before promotion.

## 22. Critical uncertainty / rejection trigger

Whether adjacent temporal/probabilistic/sequential-diagnosis literature already provides the same diagnostic-state representation, or state/transition labels cannot be defined reliably enough to support the thesis.

---

# C3 — Data-Fitness-Aware Autonomous Target-Trial Emulation

## 1. Candidate identity

**Title:** Data-Fitness-Aware Autonomous Target-Trial Emulation

**One-sentence identity:** Develop an autonomous causal-analysis framework that explicitly reasons about whether an EHR can support each target-trial component and refuses or revises emulations when data-generation constraints make the intended causal estimand non-identifiable or operationally invalid.

## 2. Central scientific object

A **machine-readable target-trial validity representation**, **data-fitness/identifiability checker**, **revision/abstention policy**, and **audit trace** linking causal conclusions to data-support checks and design decisions.

## 3. Central scientific problem

Agentic systems are rapidly being applied to protocol extraction, cohort construction, clinical trial design, and end-to-end target-trial emulation. The emerging danger is that automation can make an invalid emulation easier to execute. EHR-based target-trial validity depends on whether eligibility, time zero, treatment assignment, confounding control, follow-up, and outcomes can actually be realized from data generated by routine care.

The central methodological problem is therefore **autonomous causal-design validity under imperfect observational data**, not simply automating more pipeline steps.

## 4. Falsifiable dissertation thesis

> An agentic TTE system that explicitly models data-generating constraints, design feasibility, and causal identifiability before executing analysis will produce fewer invalid emulations and more reliable causal conclusions than automation that directly translates protocols into cohorts and estimators.

The thesis is falsified if feasibility/identifiability reasoning does not improve validity, if experts cannot adjudicate the target criteria reliably, or if simple checklists perform as well as the proposed agentic method.

## 5. Evidentiary basis

### Source-supported finding
**Claim:** EHR-based TTE validity can fail because core target-trial components cannot be credibly implemented under healthcare-driven observation processes; this can change the estimand itself.  
**Source:** Wang et al., *An operational target trial emulation framework for causal inference using electronic health record data*, npj Digital Medicine 2026, DOI `10.1038/s41746-026-02563-z`.

### Source-supported finding
**Claim:** Advanced adjustment methods may fail to recover randomized-trial effects when important confounding is unobserved in real-world EHR data.  
**Source:** Fan et al., *Evaluating bias in target trial emulation for heart failure across statistical and deep learning methods*, Nature Communications 2026, DOI `10.1038/s41467-026-74999-6`.

### Source-supported finding
**Claim:** Agentic systems are already being used to automate RWE extraction and trial-design workflows across multiple diseases and health systems.  
**Source:** *Empowering clinical trial design with agentic intelligence and real-world data* (EmulatRx), Nature Communications 2026, DOI `10.1038/s41467-026-74501-2`.

### Source-supported finding
**Claim:** LLM-driven protocol extraction and phenotyping pipelines for TTE have been demonstrated with human validation.  
**Source:** 2026 medRxiv preprint, *LLM-Driven Target Trial Emulation with Human-in-the-Loop Validation for Randomized Trial*, DOI `10.64898/2026.04.09.26350523`.

### Source-supported finding
**Claim:** Autonomous agentic trial-emulation pipelines are being investigated at scale and can quantify health-system-specific EHR–RCT discrepancies.  
**Source:** 2026 medRxiv preprint, *Agentic Trial Emulation to Learn Health System-specific Drug Effects At Scale*, DOI `10.64898/2026.02.19.26346539`.

### Cross-paper inference
As automation becomes feasible, the unsolved scientific contribution may shift from “can an LLM execute TTE?” toward “can an autonomous system know when an emulation is causally/data-operationally valid enough to execute and interpret?”

## 6. Closest and dangerous prior work

1. Wang et al. 2026 — dangerous prior art for the data-fitness/operational-validity conceptual framework.
2. EmulatRx — dangerous prior art for agentic RWE/trial-design automation.
3. LLM-driven TTE preprint — dangerous prior art for protocol-to-pipeline automation.
4. Agentic Trial Emulation preprint — dangerous prior art for automated EHR emulation and discrepancy calibration.
5. Classical TTE / causal identifiability / positivity / measurement-error literature — essential Day 2 search area.

## 7. Evidence-supported limitations of existing approaches

### Directly supported
- Operational TTE can fail before effect estimation because EHR observation does not support the conceptual trial design.
- Stronger statistical models cannot automatically repair unobserved confounding.
- Agentic automation of TTE/trial design is now plausible and active.

### Inferred limitation
Current agentic frameworks appear oriented toward executing/refining workflows rather than formalizing **a refusal/revision boundary** tied to data fitness and identifiability before causal estimates are generated.

## 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

A potentially high-value gap is an autonomous TTE system whose primary intelligence is not protocol extraction but **causal feasibility adjudication**: representing target-trial assumptions, mapping each assumption to observable EHR evidence, identifying unsupported components, revising the estimand/design when defensible, and otherwise abstaining from causal claims.

## 9. Proposed methodological contribution

1. **Machine-readable target-trial validity representation** linking estimand/design components to data requirements and causal assumptions.
2. **Data-fitness/identifiability checker** that tests whether required constructs can be operationalized without post-baseline conditioning, severe missingness, or unsupported assumptions.
3. **Revision/abstention policy** that modifies the target estimand/design or stops analysis when criteria fail.
4. **Audit trace** connecting each causal conclusion to data-support checks and design decisions.

The novelty must exceed a static checklist by showing algorithmic reasoning/generalization and calibrated refusal/revision behavior.

## 10. Coherent dissertation aims

### Aim 1 — Formalize data-fitness-aware TTE state
**Question:** Can causal-design feasibility be represented in machine-readable, testable form?  
**Method:** Translate TTE operational principles into structured constraints and data diagnostics.  
**Experiment:** Retrospective annotation of published emulations / synthetic violations.  
**Expected evidence:** Reliable detection of known invalid or altered estimands.

### Aim 2 — Build an autonomous design checker/reviser
**Question:** Does explicit feasibility reasoning improve automated TTE validity?  
**Method:** Agent/controller that maps protocols and data dictionaries to constraints, executes diagnostics, proposes revisions, or abstains.  
**Experiment:** Compare with direct LLM automation, checklist-only systems, and human-designed pipelines.  
**Expected evidence:** Fewer invalid emulations and better agreement with expert causal judgments.

### Aim 3 — Evaluate across health systems / trial families
**Question:** Does the framework generalize under different EHR data-generating processes?  
**Method:** Multi-dataset or semi-synthetic validation.  
**Experiment:** Emulate known RCTs across public/partner data sources; test transport of validity decisions.  
**Expected evidence:** Identifies when the same trial is emulable in one data environment but not another.

## 11. Publication decomposition

1. Formal representation + benchmark of TTE data-fitness failures.
2. Autonomous checker/reviser method.
3. Multi-system external validation / causal calibration.

If later cross-system validation is unavailable, Aims 1–2 remain potentially publishable. If static rule-based checking matches the agentic method, the “agentic” component should be abandoned rather than defended artificially.

## 12. Evaluation strategy

- Public EHR data such as MIMIC-IV for feasibility demonstrations where causal questions are suitable.
- Semi-synthetic data with known causal structure/violations.
- Published RCTs with corresponding observational data where available.
- Baselines: human-authored TTE, direct LLM protocol-to-code, checklist-only validation, causal estimators without pre-analysis fitness reasoning.
- Metrics: violation detection, expert agreement, estimand fidelity, false-safe rate, appropriate abstention/revision, EHR–RCT concordance as a secondary—not definitive—metric.
- Negative controls and sensitivity analyses are central.

## 13. Required resources and feasibility

### Known available
- Public TTE methodological literature.
- Public EHR datasets and semi-synthetic simulation capability.

### Plausibly available
- OMOP expertise / local data infrastructure.
- Causal-inference collaborators.

### Currently uncertain
- Access to multi-health-system RWD for strongest external validation.
- Expert time to adjudicate causal-design validity.

The first two aims can be built with public/semi-synthetic resources.

## 14. Novelty-collision risks

- Wang et al. already provide a strong operational data-fitness framework; converting it to software may be incremental.
- EmulatRx and other agentic TTE systems are moving rapidly.
- Classical causal-inference software already includes diagnostics for positivity, missingness, and design validity.
- Reviewer objection: causal validity cannot be delegated to an LLM without formal guarantees.
- Reviewer objection: “agentic” adds little beyond a deterministic constraint engine.

## 15. Advisor / expertise complementarity

**Required expertise preserved from the frozen artifact:**
- causal inference / target-trial emulation / RWE;
- EHR data modeling and data-generating processes;
- biomedical NLP/agents for protocol interpretation and workflow automation.

The frozen artifact states that this direction has unusually clear complementarity between an external biomedical NLP/agent advisor and an IHI primary advisor with causal/RWE depth.

**Specific IHI primary-advisor name(s): NOT PRESENT IN ORIGINAL FROZEN ARTIFACT.**

## 16. Foundation-model resilience

Very high if the contribution is formal causal/data-fitness reasoning and auditable design constraints. Stronger language models may automate more extraction/code generation, increasing rather than eliminating the need to ensure the resulting causal study is valid.

## 17. Publication and execution risk

- **Novelty bar:** Moderate to high.
- **Time to first paper:** Potentially good via benchmark/formalization.
- **High-risk dependency:** Demonstrating advantage beyond deterministic rules/checklists.
- **Ground truth:** Expert causal adjudication is difficult.
- **Reproducibility:** Strong with simulation/public data.
- **Moving-field risk:** High for agentic automation, lower for causal validity.

## 18. Generalizability

### Healthcare-specific
EHR observation mechanisms, target-trial design, clinical RWE.

### Transferable
Autonomous scientific-analysis systems that decide whether data support a requested estimand before executing an analysis; assumption-aware AI for scientific workflows.

## 19. Strongest reason to reject the direction

The strongest scientific core may already be the causal-inference framework itself, with the agent merely serving as an interface. If so, the AI contribution could be incremental and the dissertation may belong more naturally to applied causal inference than to novel AI methodology.

## 20. Evidence that would change the recommendation

**Strengthen:** Existing automated TTE systems show frequent design-validity errors that explicit feasibility reasoning can detect.  
**Weaken:** Deterministic implementation of published TTE rules performs equally well.  
**Kill:** No credible way to validate automated identifiability judgments or insufficient novelty beyond operationalizing established causal guidance.

## 21. Day 1 verdict and verdict rationale

**ADVANCE**

Of the four directions, this currently has the strongest combination of a consequential scientific failure mode, foundation-model resilience, clear advisor complementarity, and publication decomposition. Its central Day 2 question is whether the AI-methodological contribution is deep enough beyond causal-rule operationalization.

## 22. Critical uncertainty / rejection trigger

Whether deterministic implementation of established TTE/causal guidance performs equally well, leaving insufficient AI-methodological novelty or no credible way to validate automated identifiability judgments.

---

# C4 — Process-Aware Dynamic Assurance and Failure Localization for Clinical AI Agents

## 1. Candidate identity

**Title:** Process-Aware Dynamic Assurance and Failure Localization for Clinical AI Agents

**One-sentence identity:** Develop dynamic evaluation methods that diagnose *where and why* long-horizon clinical agents fail across information gathering, tool use, evidence grounding, policy compliance, and decision transitions rather than scoring only final answers.

## 2. Central scientific object

A **clinical failure ontology**, **critical-step localizer**, **counterfactual replay/intervention framework**, **dynamic stress generator**, and **assurance metric** for causal/process-level failure attribution.

## 3. Central scientific problem

Clinical AI agents act through trajectories: they gather evidence, invoke tools, maintain state, communicate, and make irreversible or costly intermediate choices. Final-answer accuracy can hide unsafe or inefficient trajectories. Recent benchmarks now expose sequential difficulty and process metrics, while dynamic red-teaming reveals severe reliability degradation under adaptive perturbations. The unresolved methodological problem is **causal/process-level failure attribution under long-horizon, stochastic agent execution**.

A useful assurance system should determine not merely that a trajectory failed, but the critical step, failure class, upstream cause, and whether a counterfactual correction at that step would have prevented downstream failure.

## 4. Falsifiable dissertation thesis

> Process-aware, dynamically generated evaluations with explicit failure localization will predict and explain clinically consequential agent failures more reliably than endpoint-only benchmarks and post-hoc LLM judging, and will enable targeted interventions that improve downstream safety without indiscriminately increasing oversight.

The thesis is falsified if process annotations do not improve failure prediction/localization or if targeted corrections based on the framework do not improve downstream outcomes over generic safeguards.

## 5. Evidentiary basis

### Source-supported finding
**Claim:** Dynamic adversarial testing can reveal severe reliability failures that static medical benchmarks miss.  
**Source:** Pan et al., *Addressing benchmarking gaps in large language models for health and medicine with dynamic red-teaming*, Nature Health 2026, DOI `10.1038/s44360-026-00152-8` (existing `LIT-032`).

### Source-supported finding
**Claim:** AgentClinic shows large degradation in sequential clinical tasks relative to static settings and supports tool/interaction-level analysis.  
**Source:** AgentClinic, DOI `10.1038/s41746-026-02674-7`.

### Source-supported finding
**Claim:** MedCTA introduces clinician-verified tool trajectories and process-aware metrics for tool selection, argument validity, execution stability, trajectory fidelity, and outcomes; frontier agents remain brittle.  
**Source:** Ashraf et al., *MedCTA: A Benchmark for Clinical Tool Agents*, arXiv `2606.11702` (preprint).

### Source-supported finding
**Claim:** Recent methodological commentary argues that agent benchmarks should assess full decision trajectories, action appropriateness, process safety, and resource stewardship.  
**Source:** Ruhrberg Estévez et al., *How to benchmark medical AI agents*, PLOS Medicine 2026, DOI `10.1371/journal.pmed.1005170`.

### Cross-domain dangerous prior art
**Claim:** General-agent research is already studying critical failure-step localization from execution trajectories.  
**Source:** Barke et al., *AgentRx: Diagnosing AI Agent Failures from Execution Trajectories*, Microsoft Research preprint, 2026.

### Cross-paper inference
The clinical evaluation field is clearly moving toward process-aware benchmarks; therefore a dissertation cannot simply propose “evaluate trajectories.” The remaining opportunity, if any, must be deeper: failure localization, counterfactual causal attribution, dynamic generation of stress conditions, and intervention selection under clinically meaningful constraints.

## 6. Closest and dangerous prior work

1. DAS dynamic red-teaming — dangerous prior art for dynamic safety evaluation.
2. AgentClinic — dangerous prior art for interactive clinical-agent benchmarking.
3. MedCTA — very dangerous prior art for process-aware tool-trajectory evaluation.
4. PLOS Medicine benchmarking framework — dangerous prior art for the conceptual argument that process matters.
5. AgentRx — dangerous prior art for cross-domain trajectory failure localization.

This is the candidate with the highest obvious collision burden on Day 1.

## 7. Evidence-supported limitations of existing approaches

### Directly supported
- Static health benchmarks can substantially overestimate reliability under adaptive stress.
- Sequential clinical agents exhibit failures in tool routing, stopping, and evidence acquisition.
- Existing process-aware benchmarks are emerging rapidly.

### Inferred limitation
Existing clinical benchmarks mostly characterize *what* failed rather than estimating the **critical causal failure step** and whether targeted intervention at that step would prevent downstream errors across stochastic reruns.

## 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

A potentially unresolved niche is **counterfactual process assurance**: dynamically stress an agent, identify the earliest clinically consequential failure, estimate whether that step causally propagated to the endpoint error, and use the attribution to select targeted monitoring/intervention.

This gap is fragile because AgentRx may already supply much of the general methodology.

## 9. Proposed methodological contribution

1. **Clinical failure ontology** spanning information acquisition, evidence grounding, temporal reasoning, tool use, policy/constraint violation, premature commitment, and escalation failure.
2. **Critical-step localizer** with evidence-backed attribution.
3. **Counterfactual replay/intervention framework** that repairs/replaces one trajectory step and measures downstream outcome changes across stochastic reruns.
4. **Dynamic stress generator** that adapts perturbations to the evolving trajectory rather than only mutating the initial prompt.
5. **Assurance metric** that combines endpoint correctness with process safety and recoverability.

## 10. Coherent dissertation aims

### Aim 1 — Measure and localize clinical-agent failures
**Question:** Can expert-meaningful critical failure steps be identified reproducibly?  
**Method:** Annotate trajectories from AgentClinic/MedCTA-like tasks with critical failure step/category.  
**Experiment:** Compare automated localizers with clinician/informatician adjudication and generic LLM judges.  
**Expected evidence:** Higher step-level attribution accuracy and inter-rater agreement.

### Aim 2 — Establish causal contribution of failure steps
**Question:** Does repairing the localized step actually change downstream outcomes?  
**Method:** Counterfactual trajectory replay with controlled step replacement and multiple stochastic reruns.  
**Experiment:** Compare critical-step repairs with random-step repair and generic retry/reflection.  
**Expected evidence:** Localized repairs yield larger downstream improvement than non-targeted interventions.

### Aim 3 — Dynamic assurance under distribution shift
**Question:** Does adaptive stress testing expose transferable failure mechanisms and support targeted safeguards?  
**Method:** Generate clinically plausible perturbations and monitor process-level degradation.  
**Experiment:** Cross-model, cross-specialty, and tool-failure evaluations.  
**Expected evidence:** Failure signatures generalize enough to inform monitoring policies.

## 11. Publication decomposition

1. Clinical failure taxonomy + annotated trajectory benchmark.
2. Critical-step localization / counterfactual attribution method.
3. Dynamic assurance and targeted intervention study.

Even if dynamic stress generation is less novel, the localization/causal-replay work could form the methodological spine.

## 12. Evaluation strategy

- AgentClinic.
- MedCTA or equivalent process-aware tool-use benchmarks.
- Long-horizon policy-rich healthcare workflows where available.
- Synthetic tool failures, missing evidence, contradictory outputs, and resource constraints.
- Metrics: critical-step localization accuracy, failure-class accuracy, counterfactual downstream effect, process-safety violations, endpoint utility, recovery efficiency, clinician agreement.
- Baselines: endpoint score, generic LLM judge, AgentRx-style diagnosis, static rule checker, random retry, full-trajectory reflection.

## 13. Required resources and feasibility

### Known available
- Public agent benchmarks and traceable trajectories.
- Ability to instrument agent runs and replay tool calls.

### Plausibly available
- Clinician/informatician review of a manageable subset.
- Synthetic policy/tool simulators.

### Currently uncertain
- Access/licensing of some benchmark tool environments.
- Expert annotation burden for causal failure labels.

A benchmark/localization first paper is plausible without restricted clinical data.

## 14. Novelty-collision risks

- MedCTA already provides process-aware evaluation.
- AgentRx already performs failure-step localization cross-domain.
- DAS already performs dynamic health red-teaming.
- Combining these three could be seen as integration rather than novelty.
- Counterfactual replay may be confounded by stochastic downstream behavior.
- Reviewer objection: “critical step” may not be uniquely identifiable in distributed/multi-causal failures.

## 15. Advisor / expertise complementarity

**Required expertise preserved from the frozen artifact:**
- biomedical agents/NLP/tool use;
- evaluation methodology / causal attribution / sequential systems;
- clinical safety/workflow expertise.

The frozen artifact states that this is a strong fit for complementary advising if the primary advisor contributes rigorous evaluation, causal/statistical, or systems methodology rather than duplicating biomedical NLP.

**Specific IHI primary-advisor name(s): NOT PRESENT IN ORIGINAL FROZEN ARTIFACT.**

## 16. Foundation-model resilience

High. Better agents increase the need for evaluation capable of detecting rarer and more complex failures. However, benchmark-specific failure taxonomies may age quickly; the method must remain model-agnostic and process-level.

## 17. Publication and execution risk

- **Novelty bar:** Very high due to 2026 benchmark activity.
- **Time to first paper:** Good if benchmark extension is accepted as meaningful.
- **High-risk dependency:** Demonstrating novelty beyond MedCTA + DAS + AgentRx.
- **Ground truth:** Difficult for causal failure attribution.
- **Reproducibility:** Strong with logged trajectories and replay infrastructure.
- **Moving-field risk:** Very high.

## 18. Generalizability

### Healthcare-specific
Clinical failure taxonomy, harm weighting, process constraints.

### Transferable
Failure localization, counterfactual trajectory attribution, dynamic assurance, targeted monitoring for autonomous agents in other high-stakes domains.

## 19. Strongest reason to reject the direction

The frontier is moving so quickly that the proposed contribution may already be decomposable into recently published components: dynamic red-teaming, process-aware medical-agent benchmarks, and general-agent failure localization. The combination could be judged incremental unless counterfactual attribution produces a genuinely new methodological result.

## 20. Evidence that would change the recommendation

**Strengthen:** A literature search showing no robust clinical method for causal critical-step attribution and targeted intervention.  
**Weaken:** AgentRx-like methods transfer trivially to clinical agents.  
**Kill:** MedCTA or imminent work already provides failure localization plus counterfactual trajectory repair at comparable depth.

## 21. Day 1 verdict and verdict rationale

**HOLD**

The scientific problem is important and highly resilient, but the 2026 literature is already crowded around process-aware benchmarking and dynamic assurance. Advance only if Day 2 identifies a defensible methodological gap in causal failure attribution/intervention.

## 22. Critical uncertainty / rejection trigger

Whether causal critical-step attribution/intervention remains scientifically distinct beyond MedCTA + DAS + AgentRx; if adjacent work already provides comparable localization and counterfactual repair, the direction should not advance.

---

# Layer III — Portfolio-level analysis

## A. Candidate diversity check

The four candidates are related by trustworthy autonomous biomedical AI but are scientifically distinct:

1. **Evidence-State Control** — intervention policy under uncertainty/evidence conditions.
2. **Diagnostic-State Trajectories** — temporal representation and constrained longitudinal inference.
3. **Data-Fitness-Aware TTE** — causal-design validity and autonomous scientific analysis.
4. **Dynamic Assurance/Failure Localization** — evaluation and causal diagnosis of agent trajectories.

Candidates 1 and 4 are the closest pair because both concern agent reliability. They should remain separate on Day 1: Candidate 1 changes **agent control**, while Candidate 4 changes **evaluation/assurance**. If later evidence shows the controller requires the same failure-state representation as the evaluator, normalization may merge them.

Candidate 2 is explicitly neuro-symbolic but narrow enough to be testable rather than using NeSy as an umbrella label. Candidate 3 is causal/RWE-focused and has the most domain-specific methodological core.

## B. Qualitative scientific comparison matrix

| Criterion | C1 Evidence-State Control | C2 Diagnostic-State Trajectories | C3 Data-Fitness-Aware TTE | C4 Dynamic Assurance |
|---|---|---|---|---|
| Scientific importance | High | High | Very high | Very high |
| Methodological depth | Potentially high | High if formalized | High | High |
| Falsifiability / discriminating experiment | Explicit state/control must beat simpler uncertainty/orchestration baselines | Structured constraints must improve trajectory fidelity without mere over-conservatism | Feasibility/identifiability reasoning must beat direct automation/checklists | Process annotations/localization must improve attribution and targeted correction outcomes |
| Preliminary novelty headroom | Uncertain | Uncertain | Moderate | Low–uncertain |
| Publication tractability | Good benchmark-first path | Good benchmark-first path | Good | Good but crowded |
| Empirical feasibility | Good with public tasks | Moderate | Moderate | Good |
| Time to uncertainty resolution | Early benchmark/annotation and simple-baseline tests can expose the central weakness | Annotation reliability and adjacency search are early resolvers | Comparison against deterministic rule/checklist implementations is the central early resolver | Day 2 collision search against MedCTA/DAS/AgentRx can resolve viability quickly |
| Artifact/reuse potential | High | High | High | Very high |
| Foundation-model resilience | High | High | Very high | Very high |
| IHI advisor/resource feasibility | Good | Good | Very good if causal expertise available | Good |
| Transferable technical depth | Very high | High | High–very high | Very high |
| Largest uncertainty | Collision with decision theory | Collision with temporal/probabilistic models | AI novelty beyond causal rules | Collision with 2026 assurance work |

The original frozen artifact also contained a preliminary within-stream ordering for Day 2 attention. That historical ordering is preserved conceptually as part of the original artifact and is not converted here into a canonical ranking; the candidate-specific verdicts remain the v2 triage surface.

## C. Missing-direction check

A serious omitted family in the frozen artifact is **active information acquisition / value-of-information optimization for clinical agents**: agents that choose the next question, test, retrieval, or measurement based on expected information gain, clinical utility, cost, and risk. This overlaps C1 but could become distinct if optimal information acquisition, rather than metacognitive/evidence-state control, is the scientific core. The frozen artifact also identified **scientific-agent reproducibility and executable provenance** for biomedical discovery workflows as another potentially strong but insufficiently investigated family.

## D. Intellectual-interest note

Neuro-symbolic AI and artificial metacognition remain scientifically plausible mechanisms, but neither should be used as a top-level dissertation identity. In the frozen analysis:

- Metacognition is operationalized most cleanly in C1 as selective evidence-state control.
- Neuro-symbolic reasoning is operationalized most cleanly in C2 as temporal state-transition constraints.

Both survive only in **narrow, falsifiable forms**, not because of personal interest alone.

## E. Stopping-condition statement

The original stopping condition was met: four distinct, literature-informed, falsifiable directions were specified, and additional Day 1 searching was judged unlikely to change which directions deserved adversarial Day 2 review. The next high-value computation identified by the frozen artifact was to attack their novelty and conceptual assumptions.

**Original scientific status remains: `FROZEN — BLIND FIRST PASS`.**

No candidate definition, canonical ranking, evidence file, literature registry, or decision log is changed by this format-normalized derivative.
