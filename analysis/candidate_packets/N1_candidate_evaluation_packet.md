# N1 Candidate Evaluation Packet

- **Candidate identifier:** N1
- **Candidate title:** Structured Evidence-State Selective Control for Clinical Artificial Intelligence
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifacts and sections:** `analysis/analysis_01/day1_candidate_generation_v2.md` C1; `analysis/analysis_02/day1_candidate_generation_v2.md` D02-01; `analysis/analysis_03/day1_candidate_generation_v2.md` C3
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N1 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **structured evidence/failure-state representation** linked to a **clinically cost-sensitive multi-action controller** and a **process-aware selective-evaluation framework**.

The state represents why immediate commitment may be unsafe or incomplete. Candidate state components include evidence support, missingness, contradiction, provenance, temporal validity, tool reliability, patient-event time, evidence-validity time, and task-structural failure signals. The controller chooses among actions such as answer, retrieve, verify, ask, preserve, revise or flag, and defer.

The packet does not require every candidate state component or every action to appear in the final method. It requires a meaningful structured state-to-action thesis rather than a generic prompt router.

## 2. Exact falsifiable thesis

> For sequential clinical reasoning tasks involving heterogeneous uncertainty and evolving information, an explicit structured evidence/failure-state representation coupled to a cost-sensitive multi-action controller will reduce unsafe commitment, unsupported belief revision, and clinically weighted decision loss at matched action cost and human workload relative to scalar confidence, answer-versus-abstain policies, fixed retrieval rules, generic self-verification, and generic reflection or tool-routing baselines.

The thesis is defeated or materially weakened if:

- structured state adds no practically meaningful benefit over calibrated scalar uncertainty or simple rules;
- richer actions add no value beyond binary abstention;
- the proposed state cannot be labeled, estimated, or validated reliably;
- the apparent gains arise only from additional retrieval, compute, or tool calls;
- substantially equivalent state-to-action control already exists in prior work.

## 3. Included scientific scope

The common Phase 1 target includes:

1. A structured, non-scalar account of why commitment may be unsafe or incomplete.
2. At least one explicit temporal component relevant to changing patient information, changing external evidence, or both.
3. A multi-action decision problem richer than answer versus abstain.
4. An explicit cost or utility model covering clinically asymmetric errors, action burden, latency, or human workload.
5. Comparison of alternative state or signal representations, including typed evidence state, dual-clock belief state, and task-structural failure signals.
6. Evaluation under controlled missingness, contradiction, stale or superseded evidence, tool unreliability, and distribution or documentation shift where feasible.
7. Process-level outcomes such as unsafe commitment, unsupported revision, appropriate escalation, risk-coverage trade-offs, and cost-adjusted utility.
8. Cross-model or cross-task validation sufficient to test whether the method is more than a one-model routing heuristic.

## 4. Explicitly excluded scientific scope

The following are not part of N1's mandatory scientific identity:

- A complete claim-evidence adequacy, study-quality, currency, and patient-applicability calculus; that is N6.
- Lifecycle regression testing or attribution across system releases; that is N4b.
- Causal localization of a critical failure step inside one agent trajectory as a primary thesis; that is N4a.
- Diagnostic-state trajectory reconstruction as the primary outcome; that is N2.
- A requirement to use reinforcement learning, conformal prediction, a partially observable Markov decision process, or any one controller family. These are candidate methods or baselines.
- A requirement to solve clinical question answering, extraction, generation, longitudinal chart reasoning, and tool-use simulation as four separate projects.
- A claim that task-structural signals must dominate model-internal confidence in every setting.
- A claim that the system possesses human-like metacognition.
- Generic retrieval-augmented generation, prompt routing, or planner-executor-verifier orchestration without a new state-to-action scientific contribution.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S01-C1 — Evidence-State Control for Selective Clinical AI Agents | Typed evidence/uncertainty state; multi-action controller; process-aware evaluation | Broad common core | Its complete original task suite and every proposed state field |
| D02-01 — Dual-clock Evidence-State Control for Longitudinal Clinical Agents | Provenance-linked belief state; patient-event and evidence-validity clocks; justified preservation and revision | Complementary temporal specialization and strong longitudinal instantiation | Longitudinal care as the only permissible task; every original action and environment component |
| S03-C3 — Selective Control for Clinical Language Systems under Asymmetric Risk | Task-structural failure signals; asymmetric cost; human-workload normalization; distribution-shift testing | Competing signal formulation and evaluation machinery | A separate thesis that structural signals must dominate under every site/language shift; extraction as a mandatory dissertation-wide setting |

The normalized relationship is **same direction with competing and complementary formulations**, not three additive dissertation spines.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Represent and measure evidence/failure state | Can structured state or task-derived signals identify when immediate commitment is unsafe more reliably than scalar confidence and generic self-verification? | Define the state/action ontology; create controlled cases; compare typed, dual-clock, structural, and scalar representations | Explicit state contains decision-relevant information beyond scalar uncertainty | Predictive validity, annotation reliability or controlled truth, and ablations isolating useful state components |
| Aim 2 — Learn or derive cost-sensitive multi-action control | Does conditioning on the structured state improve the choice among answer, retrieve, verify, ask, preserve, revise/flag, and defer? | Compare rule-based, decision-theoretic, and learned controllers at matched action budget | Structured state improves clinically weighted decision utility and reduces unsafe commitment/revision | Better risk-cost or utility frontier than simple rules, binary abstention, fixed retrieval, and generic orchestration |
| Aim 3 — Test robustness and transfer | Does the state-to-action mechanism retain value across model families, clinical tasks, evidence changes, and distribution shift? | Frozen-interface transfer, external validation, and model-replacement studies | The contribution is structural rather than one-model routing | Preserved or well-bounded gains under model, task, temporal, and documentation shift |

A reviewer may conclude that one aim is overbroad or that the target contains multiple theses. The reviewer must evaluate this packet as written rather than silently replacing it.

## 7. Decisive or discriminating experiment

- **Experimental unit:** a sequential clinical reasoning episode with controlled evidence state, permissible action set, and recorded action costs.
- **Strongest comparator:** calibrated scalar uncertainty plus a prospectively specified simple policy such as retrieve on staleness, ask on missingness, and defer below a confidence threshold; also include strong self-verification and answer-versus-abstain baselines.
- **Primary thesis-relevant outcomes:** clinically weighted decision loss, unsafe-commitment rate, unsupported-revision rate, risk-coverage/action-cost frontier, and human workload.
- **Supporting result pattern:** at matched model access, information, action budget, and workload, structured state produces a practically meaningful improvement over both simple policies and strong native self-verification across more than one model/task setting.
- **Defeating result pattern:** simple rules, calibrated confidence, or frontier self-verification are prospectively equivalent or superior; state annotations are unreliable; or gains disappear after matching retrieval/tool-call budget.

## 8. Inherited dangerous prior art

These sources and source families were identified during Day 1 as required starting points. Their presence in this packet does not establish a collision; Phase 1 reviewers must inspect and classify them independently.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| `LIT-026` | Cocchieri et al., *LLMs (Almost) Never Abstain Under Medical Uncertainty*, ACL 2026, DOI `10.18653/v1/2026.acl-long.1365` | Occupies medical abstention and overcommitment | Repository status SCREENED | Does it extend beyond binary abstention or multiple-choice QA into structured multi-action control? |
| `LIT-025` | Wang et al., *LINS*, Nature Communications 2025, DOI `10.1038/s41467-025-64142-2` | Combines evidence-traceable retrieval, response generation, and evidence validity/timeliness claims | SCREENED | Does its control logic or evidence state already cover the proposed state-to-action object? |
| `LIT-024` | Wang et al., *MedCite*, Findings of ACL 2025, DOI `10.18653/v1/2025.findings-acl.967` | Provides medical citation generation/evaluation and may supply verification signals | SCREENED | Is it merely a signal/component, or does it implement the proposed controller? |
| Unregistered, DOI `10.1038/s41746-025-01965-9` | Cui et al., *TIMER* | Time-aware longitudinal modeling | Day 1 page/section-level characterization | Does it represent persistent belief state or only model temporal instruction/records? |
| Unregistered, DOI `10.1038/s41746-026-02674-7` | Schmidgall et al., *AgentClinic* | Sequential clinical agents, tools, notes, reflection, and process evaluation | Day 1 page/section-level characterization | Does its agent state or action policy already implement N1's core? |
| `LIT-030` | Liu et al., clinical agent-system benchmarking, DOI `10.1038/s41746-026-02443-6` | Planner-executor-verifier orchestration and clinical-agent benchmarking | SCREENED | Is N1 novel beyond a richer evaluation and router? |
| Unregistered, PMLR 304 | Tayebati et al., *CAP: Conformalized Abstention Policies* | Adaptive, calibrated policy over prediction, prediction sets, and abstention | Day 1 page/abstract characterization | Does CAP or its parent literature subsume the multi-action policy after adding clinical costs? |
| `LIT-001` | Su et al., *KGARevion*, ICLR 2025, arXiv `2410.04660` | Generates, verifies, and revises claims using an external knowledge graph | READ in prior stream work | Does its verify-revise loop already supply the relevant evidence state and action policy? |
| Source family | Partially observable decision processes, belief-state control, active information acquisition, learning to defer, selective prediction, metareasoning | The central idea may already exist outside medicine under mature terminology | Not comprehensively searched on Day 1 | Is N1 a healthcare relabeling of established state estimation and sequential control? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether the proposed state-to-action object is novel beyond belief-state estimation, selective prediction, active sensing, learning to defer, and metareasoning | KT1 | A mature parent method could fatally collapse novelty | Unresolved; Day 1 search was not saturated outside medicine |
| Whether a structured state adds practical value over calibrated confidence and simple action rules | KT4 | Failure removes the need for the proposed complexity | Proposed hypothesis only |
| Whether permissible actions or state labels can be defined reliably | KT3 | Unreliable targets would undermine learning and evaluation | Unresolved; controlled truth may be possible for some cases |
| Whether N1 remains one thesis rather than a bundle of typed state, dual clocks, structural signals, and several tasks | KT2 | Overbreadth could require material narrowing | Round 3 accepted one identity with an explicit scope warning |
| Whether native self-verification improves fast enough to commoditize the control layer | KT6 | Could make the empirical gap model-contingent | Unresolved, moving frontier |
| Whether realistic evaluation is possible without restricted clinical workflows | KT5 | Core evidence may otherwise remain synthetic or benchmark-bound | Public/synthetic minimum path appears plausible; clinical external validation uncertain |

## 10. Feasibility assumptions inherited from Day 1

- Public clinical question-answering, agent, and longitudinal datasets can support an initial controlled environment.
- Synthetic or programmatically perturbed cases can provide known missingness, contradiction, staleness, and tool-failure conditions.
- At least a limited expert review can be obtained for ambiguous action appropriateness; no commitment is inferred.
- Adequate computation exists for inference, controller training, ablation, and multi-model evaluation, but large-scale foundation-model pretraining is not assumed.
- A valid public-data dissertation path should exist even if restricted clinical deployment data are unavailable.
- The strongest candidate formulation may require formal expertise in sequential decision making, uncertainty, or decision theory in addition to biomedical natural language processing expertise.

## 11. Packet provenance and change control

### Direct compressions

- The central objects, constituent theses, inherited prior art, failure conditions, and critical uncertainties are compressed from the three constituent Day 1 v2 artifacts.
- The distinction between typed state, dual clocks, and task-structural signals is preserved from the Round 3 reconciliation.

### Reconciled formulations

- The exact thesis and three common aims are coordinator reconciliations designed to encode the shared state-to-action scientific identity without requiring all constituent projects.
- The packet deliberately treats the three state/signal formulations as competitors or complements rather than cumulative requirements.

### Unresolved candidate-definition tension

Stream 03's Round 2 review argued that its original C3 structural-signals-under-shift clause could constitute a separate thesis. Round 3 retained it within N1 at the dissertation-identity level while imposing a scope constraint. Phase 1 reviewers must report a `CANDIDATE-DEFINITION DISAGREEMENT` if the packet still cannot be evaluated as one coherent thesis.

### Change control

This draft may be revised only during packet-fidelity review. Once the packet set is approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for any completed scans.
