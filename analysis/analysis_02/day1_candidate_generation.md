# Day 1 — Blind Independent Candidate Dissertation Direction Generation

- **Date:** 2026-08-31
- **Analysis stream:** `analysis_02`
- **Repository SHA used:** `86230f478b0a47a0198adbe325c42b0561fe8288`
- **Permitted repository inputs:** `README.md`; `OPERATING_PROTOCOL.md`; accepted entries in `decisions/`; structural repository READMEs; `context/user_goals_and_constraints.md`; `context/advisor_landscape.md`; `literature/index.md`; targeted literature records or source identifiers; Stream 02's own historical provenance only as optional provenance rather than an answer key
- **Excluded scientific-generation inputs:** substantive Analysis Stream 01 or 03 outputs; another stream's Day 1 candidates, rankings, recommendations, or literature interpretations; substantive Discussion Stream 01 or 03 entries; `candidate_programs/`; `decisions/current_rankings.md`; `decisions/scoring_framework.md`
- **External-search scope:** targeted searches of primary scholarly literature and official proceedings/publisher pages, emphasizing 2024–2026 work and dangerous prior art in selective prediction, longitudinal clinical reasoning, neuro-symbolic constraint methods, automated causal inference, target-trial emulation, dynamic evaluation, and model-update monitoring; this was not a systematic review or a global novelty search
- **Analysis status:** **FROZEN — BLIND FIRST PASS**

**Post-generation clarification amendment (2026-08-31):** Section 14 for each candidate was expanded to apply the existing IHI-primary-advisor plus Dr. Rui Zhang complementarity constraint using current official UMN pages. No candidate identity, scientific thesis, aim, verdict, or portfolio comparison was changed. During the targeted DEC-002 lookup after the scientific first pass had already been frozen, a broad repository text search inadvertently displayed snippets from `decisions/current_rankings.md`; those snippets were not used to revise the candidate science, verdicts, or comparison. The artifact was re-frozen after the Section 14-only substantive amendment.

## Independence, evidentiary, and stopping notes

This artifact independently generates candidate dissertation directions rather than preserving the repository's historical candidate set. Historical Stream 02 reasoning informed the questions worth testing but did not determine which directions survived current scrutiny. Existing LIT identifiers are reused only as stable source references; source interpretations below were made independently for this artifact. Newly found sources are cited in place and were not added to the shared literature registry.

The inferential standard used throughout is:

> published finding → observed limitation → cross-paper inference → preliminary gap hypothesis → proposed research hypothesis

Claims of field-wide absence are deliberately avoided. Search stopped after four distinct, falsifiable methodological directions had survived an initial collision check and additional searching was revealing closer baselines and narrower formulations, but was no longer changing the set that merits Day 2 adversarial review.

### Repository-convention declarations

- **Question evaluated:** Which three or four independently generated, current, literature-informed candidate dissertation directions are sufficiently coherent, falsifiable, important, and feasible to merit separate Day 2 adversarial review for a Health Informatics PhD?
- **Evidence used:** the permitted repository context listed above; existing LIT identifiers as source pointers; and the targeted primary scholarly literature cited within each candidate.
- **Key assumptions:** public, credentialed, or synthetic data can support an initial methodological study; suitable complementary expertise can be identified; and later novelty review will search adjacent non-medical method literatures more deeply.
- **Recommendation and uncertainty:** the candidate-specific Day 1 verdicts below are preliminary within-stream recommendations; all positive verdicts remain conditional on novelty, ground-truth, advising, and resource checks.
- **Agreements/disagreements with other analyses:** not assessed because the blind first-pass rule excluded other streams' substantive outputs.
- **Accepted decisions:** no accepted decision is recommended for reconsideration in this artifact.

## Candidate overview

| ID | Candidate dissertation direction | Central scientific object | Day 1 verdict |
|---|---|---|---|
| D02-01 | Dual-clock evidence-state control for longitudinal clinical agents | A provenance-linked belief-state representation and selective multi-action controller | ADVANCE WITH MAJOR UNCERTAINTY |
| D02-02 | Learned temporal clinical constraints for auditable representation repair | A probabilistic constraint-induction and proof-carrying repair framework | ADVANCE WITH MAJOR UNCERTAINTY |
| D02-03 | Machine-checkable causal data-fit contracts for EHR target-trial emulation | A formal contract that maps causal questions to data support, diagnostics, restricted estimands, or refusal | ADVANCE |
| D02-04 | Change-attributed continual assurance for clinical foundation-model systems | A versioned failure-surface model with budgeted regression discovery and fault localization | ADVANCE WITH MAJOR UNCERTAINTY |

The table is a map, not a cross-stream ranking or final selection.

---

## D02-01 — Dual-clock evidence-state control for longitudinal clinical agents

### 1. Candidate identity

**Title:** Dual-clock evidence-state control for longitudinal clinical agents

**One-sentence identity:** This direction studies whether a clinical agent that explicitly represents both patient-event time and external-evidence validity time can learn when to answer, retrieve, ask, preserve a belief, revise it, or defer, rather than treating every new observation or document as an instruction to regenerate an answer.

### 2. Central scientific problem

Longitudinal clinical reasoning is not only sequence processing. A system must distinguish at least two independently changing clocks:

- **patient time:** symptoms, tests, diagnoses, treatments, and outcomes evolve;
- **knowledge/evidence time:** guidelines, publications, drug warnings, and the validity of previously retrieved evidence evolve.

The unresolved methodological problem is how to maintain an auditable claim-level state under those two clocks and select an action under heterogeneous uncertainty. A system may need to retrieve because evidence is stale, ask because a patient-state variable is missing, preserve a belief because new information is irrelevant, revise because a prior premise was superseded, or defer because expected harm exceeds the value of acting. Collapsing these cases into confidence-threshold abstention or unconditional retrieval wastes resources and can create incorrect belief changes.

This matters because current clinical-agent evaluations remain much easier and more static than real care, while medical models still overcommit under uncertainty. Incorrectly revising a longitudinal state can contaminate every later decision, not merely one response.

### 3. Falsifiable dissertation thesis

**Proposed research hypothesis:** For longitudinal clinical tasks with controlled patient and evidence updates, a provenance-linked dual-clock belief representation plus a cost-sensitive selective controller will reduce unsupported belief revisions and clinically weighted decision loss, at matched action cost, relative to long-context generation, conventional RAG, self-reflection, and answer-versus-abstain policies.

This thesis is falsified if the explicit representation and controller do not improve out-of-distribution risk–cost trade-offs, if benefits disappear against strong retrieval and conformal-abstention baselines, or if a much simpler recency heuristic performs equivalently. The aims below test representation adequacy, policy effectiveness, and generalization of the same thesis; they are not independent fashionable projects.

### 4. Evidentiary basis

#### Especially relevant sources

1. Cui et al., “TIMER: temporal instruction modeling and evaluation for longitudinal clinical records,” *npj Digital Medicine* (2025), DOI [10.1038/s41746-025-01965-9](https://doi.org/10.1038/s41746-025-01965-9).
2. Schmidgall et al., “AgentClinic: a multimodal benchmark for tool-using clinical AI agents,” *npj Digital Medicine* (2026), DOI [10.1038/s41746-026-02674-7](https://doi.org/10.1038/s41746-026-02674-7).
3. Cocchieri et al., “LLMs (Almost) Never Abstain Under Medical Uncertainty,” ACL 2026, DOI [10.18653/v1/2026.acl-long.1365](https://doi.org/10.18653/v1/2026.acl-long.1365) (**LIT-026**, repository status SCREENED).
4. Wang et al., “LINS: A general medical Q&A framework for enhancing the quality and credibility of LLM-generated responses,” *Nature Communications* (2025), DOI [10.1038/s41467-025-64142-2](https://doi.org/10.1038/s41467-025-64142-2) (**LIT-025**, SCREENED).
5. Tayebati et al., “CAP: Conformalized Abstention Policies for Context-Adaptive Risk Management for LLMs and VLMs,” ACML/PMLR 304 (2025), [PMLR paper page](https://proceedings.mlr.press/v304/tayebati26a.html).
6. Wang et al., “MedCite: Can Language Models Generate Verifiable Text for Medicine?,” Findings of ACL 2025, DOI [10.18653/v1/2025.findings-acl.967](https://doi.org/10.18653/v1/2025.findings-acl.967) (**LIT-024**, SCREENED).

#### Claim → source → evidentiary status

| Claim | Source(s) | Evidentiary status |
|---|---|---|
| Models have measurable difficulty reasoning over multi-visit records, and common clinical instruction sets are temporally skewed toward retrieval rather than synthesis. | TIMER | **Source-supported finding.** Reported by the authors for their benchmark analysis and model evaluations. |
| Sequential, tool-using clinical simulations can be substantially harder than static medical QA, and models differ in their use of retrieval, notes, and reflection tools. | AgentClinic | **Source-supported finding.** Applies to the paper's simulated environments; it is not prospective clinical evidence. |
| Contemporary LLMs systematically overcommit on a medical abstention benchmark, including settings where critical question information is withheld. | MedQAbstain / LIT-026 | **Source-supported finding.** The benchmark is medical multiple-choice QA, not longitudinal care. |
| Retrieval and citation pipelines can improve evidence validity, timeliness, traceability, and citation quality. | LINS / LIT-025; MedCite / LIT-024 | **Source-supported finding.** These studies support component feasibility, not the proposed controller. |
| Per-instance conformal policies can balance prediction, prediction sets, and abstention with calibrated coverage in general LLM/VLM tasks. | CAP | **Source-supported finding and dangerous prior art.** It occupies adaptive abstention, but not the proposed dual-clock, multi-action longitudinal state. |
| Patient-time uncertainty, evidence-time staleness, and action choice should be modeled jointly rather than as one scalar confidence. | The sources above considered together | **Cross-paper inference.** No cited paper establishes this proposed decomposition. |

### 5. Closest prior work

The closest collision is not one paper but a boundary formed by CAP's adaptive abstention, LINS/MedCite's evidence-traceable retrieval and citation, TIMER's time-aware longitudinal modeling, and AgentClinic's sequential tool-use evaluation. MedQAbstain occupies the medical abstention problem. KGARevion (**LIT-001**, arXiv:2410.04660) also generates, verifies, and revises biomedical claims against a knowledge graph.

The candidate therefore cannot claim novelty for retrieval, provenance, temporal modeling, belief revision, or abstention separately. It survives only if the scientific object is the joint, typed state and the policy over materially distinct actions under asynchronous patient and knowledge changes.

### 6. Evidence-supported limitations of existing approaches

**Limitations explicitly reported by sources:**

- TIMER reports deficits in longitudinal temporal reasoning and skew in existing evaluation data.
- AgentClinic and Liu et al. (**LIT-030**, DOI [10.1038/s41746-026-02443-6](https://doi.org/10.1038/s41746-026-02443-6)) report that sequential clinical agents remain imperfect, costly, and incompletely evaluated on longitudinal workflows.
- MedQAbstain reports systematic overcommitment.
- LINS and MedCite address evidence grounding and citation quality, but their stated objects are response generation/evaluation rather than persistent belief management.

**Limitations inferred here:**

- Answer-versus-abstain policies do not by themselves decide whether retrieval or clarification has positive value.
- A timestamp on an encounter is not an evidence-validity interval; using one temporal axis cannot express a stable patient fact supported by superseded guidance, or a new patient event assessed using current evidence.
- Re-generating a full answer after each update does not guarantee minimal, justified belief revision.

These are cross-paper inferences requiring direct verification against a broader agent-control literature.

### 7. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

There appears to be unresolved methodological space for a claim-level, provenance-linked representation with separate patient-event and evidence-validity semantics, coupled to a calibrated policy over answer, retrieve, ask, preserve, revise, and defer actions. The proposed gap is not “medical agents do not abstain” and not “medical answers lack citations”; both are already active research areas.

### 8. Proposed methodological contribution

The dissertation would contribute:

1. **A dual-clock evidence-state representation** in which each claim carries patient-time scope, evidence-validity scope, provenance, polarity, uncertainty type, dependencies, and supersession relations.
2. **A selective action controller** that estimates the expected value and risk of answer, retrieve, ask, preserve, revise, and defer, subject to action cost and harm constraints.
3. **A longitudinal evaluation methodology** that scores not only final answers but state transitions: justified preservation, warranted revision, stale-evidence use, provenance coverage, and time to safe resolution.

The controller could use constrained reinforcement learning, contextual bandits, or model-based planning, but the dissertation contribution must be the formal state/action problem and validated learning objective—not a prompt router around existing tools.

### 9. Coherent dissertation aims

**Aim 1 — Measure the problem and make action quality observable.**

- **Question:** Which combinations of patient updates, evidence updates, missing information, and contradictions require each selective action?
- **Method:** Construct a versioned longitudinal environment with claim-level provenance and clinician-adjudicated action constraints; include counterfactual pairs that vary one clock while holding the other fixed.
- **Experiment:** Benchmark long-context LLMs, standard RAG, time-aware instruction-tuned models, static abstention, semantic-entropy policies, CAP-like policies, and oracle components.
- **Expected evidence:** A taxonomy of failure modes, inter-rater reliability for permissible actions, and measured headroom over simple policies.

**Aim 2 — Learn dual-clock state transitions and selective control.**

- **Question:** Does explicit two-clock state improve calibrated action selection and belief maintenance?
- **Method:** Learn claim-state updates and a cost-sensitive controller with constraints on unsupported answer/revision risk.
- **Experiment:** Paired tests under missingness, delayed observations, contradictory notes, retracted/superseded evidence, irrelevant updates, and varying action costs; ablate each state field and action.
- **Expected evidence:** Lower clinically weighted regret and stale/unsupported revision rates at matched cost and coverage.

**Aim 3 — Test transfer beyond one disease or model family.**

- **Question:** Does the controller generalize across specialties, institutions or simulated documentation styles, evidence corpora, and stronger foundation models?
- **Method:** Freeze the state schema and controller interface; adapt only clearly declared components.
- **Experiment:** External evaluation on at least one distinct clinical trajectory task and, if feasible, a non-clinical scientific evidence-update task.
- **Expected evidence:** Preserved ranking and calibration under model, corpus, and domain shift—or clear boundaries showing where the thesis fails.

### 10. Publication decomposition

1. **Measurement/benchmark:** dual-clock longitudinal scenarios, action ontology, and transition metrics.
2. **Core method:** evidence-state representation plus selective controller, with formal risk/cost objective and strong ablations.
3. **External validation/generalization:** transfer across clinical areas, evidence sources, and model generations.

This is a three-paper decomposition only if each unit has an independent scientific claim. If Aim 3 fails, a defensible dissertation could still rest on a rigorous benchmark and a method that succeeds in preregistered in-domain settings, provided its boundary conditions are reported rather than hidden.

### 11. Evaluation strategy

- **Datasets/environments:** synthetic-but-clinically-reviewed trajectories for exact intervention control; credentialed MIMIC-IV/MIMIC-IV-ED sequences where appropriate; public medical QA/evidence corpora with publication dates; TIMER/AgentClinic-compatible tasks if licenses permit; versioned guideline or PubMed evidence snapshots.
- **Strongest baselines:** long-context generation; standard and iterative RAG; LINS-like evidence pipelines; TIMER-style tuning; KGARevion-style verify/revise; semantic entropy; conformal abstention; CAP-like adaptive abstention; rule-based recency and missingness heuristics; oracle retrieval and oracle uncertainty.
- **Ablations:** remove patient time, evidence time, provenance, dependency edges, uncertainty typing, individual actions, calibration, and action costs.
- **Primary metrics:** clinically weighted decision loss; selective risk–coverage and risk–cost curves; unsupported revision rate; missed-revision rate; stale-evidence rate; action regret against adjudicated permissible sets; calibration error; provenance precision/recall; resolution latency.
- **Robustness/generalization:** temporal reorderings, delayed documentation, contradictory sources, evidence retraction/supersession, site-style shift, specialty shift, model replacement, and adversarial irrelevant updates.
- **Statistics:** paired bootstrap confidence intervals; mixed-effects models with case and model as random effects; calibration confidence bands; multiplicity control for prespecified primary contrasts; subgroup reporting rather than only aggregate means.
- **Human evaluation:** clinicians should adjudicate action permissibility, consequence severity, and whether a belief revision is justified. LLM judges may assist triage but cannot be the sole reference for safety or provenance.

### 12. Required resources and feasibility

**Known available:** public model APIs/open-weight models; PubMed metadata and date-versionable scholarly corpora; open benchmark code for several baselines; synthetic data generation; PhysioNet datasets under their existing credentialing requirements.

**Plausibly available:** clinical informatics collaborators for annotation; local compute for open models; access to MIMIC notes after credentialing; historical guideline versions; adaptation of AgentClinic or TIMER assets subject to licenses.

**Currently uncertain:** enough longitudinal gold-standard action labels; access to institution-specific multi-encounter notes; reliable evidence-version histories; whether permissible actions have adequate expert agreement; compute for repeated multi-model policy training.

The minimum viable path should use controlled public/synthetic environments first. The central claims must not depend on one restricted dataset or one collaborator. Restricted clinical data should be external validation, not the sole source of positive results.

### 13. Novelty-collision risks

- CAP and related conformal policies may already cover more multi-action selective control than the abstract suggests.
- Agent-memory and partially observable decision-process work may already formalize preserve/revise/retrieve policies outside healthcare.
- A reviewer may argue that “dual clock” is merely feature engineering around a POMDP or event-sourcing system.
- If action labels are produced from hindsight, apparent gains may reflect annotation leakage rather than metacognitive control.
- Frontier models with long context, reliable tools, and calibrated uncertainty may commoditize state extraction and simple routing.
- Combining TIMER, RAG, provenance, and abstention without a new objective or identifiable theoretical property would collapse into systems engineering.

### 14. Advisor / expertise complementarity

**Required methodological configuration:** the primary methodological need is sequential decision-making under uncertainty, calibrated selective prediction, and longitudinal state estimation. This must be joined to EHR data quality, clinical knowledge representation, evidence provenance, and clinical evaluation. Formal methods or knowledge-representation expertise would strengthen the state semantics.

The current official [IHI Graduate Program Directory](https://healthinformatics.umn.edu/graduate-program/graduate-program-directory) lists both faculty below as Core Faculty, making them plausible IHI primary-advisor options subject to formal confirmation:

- **Steven Johnson — strongest fit if the direction is framed around longitudinal EHR state, clinical knowledge representation, and decision-support infrastructure.** Johnson's [official IHI profile](https://healthinformatics.umn.edu/staff/steven-johnson) identifies secondary use and data quality of EHR data, clinical decision support, ontologies/clinical knowledge representation, healthcare data science, and machine learning. [Dr. Rui Zhang's official profile](https://med.umn.edu/bio/rui-zhang) identifies clinical NLP/information extraction, LLM/AI methods, multimodal biomedical data, biomedical literature, and knowledge graphs. The combination is complementary because Johnson can anchor the semantics, data quality, EHR infrastructure, and decision-support evaluation, while Zhang can anchor neural extraction, evidence retrieval, knowledge-graph grounding, and the agent implementation.
- **Erich Kummerfeld — strongest fit if the direction is framed around the controller's statistical learning, latent-state assumptions, and formal validation.** Kummerfeld's [official IHI profile](https://healthinformatics.umn.edu/staff/erich-kummerfeld) emphasizes statistical and machine-learning methods, causal and latent-variable discovery, theorem development, and simulation benchmarking. Zhang would contribute the clinical NLP/LLM, EHR/literature, and knowledge-graph layer. The complementarity is a methods-versus-substrate division: Kummerfeld would anchor controller identification, assumptions, and controlled evaluation; Zhang would anchor extraction and evidence-aware clinical agent behavior.

Neither public profile establishes a perfect direct match to constrained reinforcement learning or conformal sequential control, so additional expertise in sequential decision-making or uncertainty quantification may still be necessary. These are methodological-fit judgments only; willingness, availability, funding, commitment, and final advising eligibility are not inferred.

### 15. Foundation-model resilience

The durable object is not a particular base model's reasoning accuracy. It is how a changing system represents temporal scope, assigns evidence, decides whether to act, and exposes calibrated state transitions. Stronger models may improve extraction and planning but do not eliminate asymmetric action costs, changing evidence, missing observations, or the need to audit why a belief changed. Resilience is therefore high only if the work produces model-agnostic representations, policies, or guarantees; a prompt recipe would have low resilience.

### 16. Publication and execution risk

- **Novelty bar:** high, because abstention, RAG, provenance, temporal reasoning, and agent routing are all active.
- **Time to first credible unit:** moderate; a carefully designed measurement paper is plausible before the full controller.
- **Dependence on one high-risk experiment:** moderate; Aim 1 can stand alone, but the dissertation thesis requires Aim 2 to beat strong simple policies.
- **Ground-truth difficulty:** high; multiple actions may be defensible, and clinical consequences vary.
- **Reproducibility:** moderate to high with open trajectories and recorded model versions; lower with proprietary APIs or private EHRs.
- **Risk of being overtaken:** high for generic routing, lower for a rigorous dual-time formalism and transition-level evaluation.

### 17. Generalizability

**Healthcare-specific contribution:** representing encounter time, uncertain documentation, guideline validity, evidence hierarchy, and asymmetric clinical action costs.

**Methodologically transferable contribution:** selective control of persistent agents whose environment state and governing knowledge evolve on different clocks—for example, scientific assistants, legal systems, or maintenance agents. Healthcare is not merely a testbed because its temporal documentation, evidence hierarchy, and harm structure shape the method.

### 18. Strongest reason to reject the direction

The strongest objection is that the direction may bundle already-established components behind a new vocabulary, while requiring expensive and contestable expert labels for an “optimal” action. If a simple retrieve-on-staleness/ask-on-missingness/abstain-on-low-confidence policy matches the learned controller, the central thesis loses methodological force.

### 19. What evidence would change the recommendation?

- **Substantially strengthen:** high expert agreement on permissible action sets; large oracle headroom over static policies; a formal risk or regret result; reproducible gains across model families and specialties.
- **Substantially weaken:** low action-label reliability; improvements limited to one synthetic generator; gains vanish after matching retrieval budget and calibration.
- **Kill outright:** verified prior work already unifies the two temporal axes and the same action set with stronger guarantees, or preregistered experiments show no benefit over simple policies.

### 20. Day 1 verdict

**ADVANCE WITH MAJOR UNCERTAINTY**

The central thesis is coherent, clinically meaningful, technically deep, and aligned with artificial metacognition without depending on anthropomorphic claims. It advances only as the joint state/control problem; its novelty and label validity are serious Day 2 risks.

---

## D02-02 — Learned temporal clinical constraints for auditable representation repair

### 1. Candidate identity

**Title:** Learned temporal clinical constraints for auditable representation repair

**One-sentence identity:** This direction studies how to induce executable probabilistic temporal and ontological constraints from clinical data and expert knowledge, then use them to detect, localize, and minimally repair contradictions in longitudinal patient-state representations while emitting machine-checkable traces.

### 2. Central scientific problem

Neural clinical extractors and generative agents can map text into concepts and graphs, but the resulting representation may violate temporal order, type restrictions, negation/uncertainty scope, laterality, episode boundaries, or domain rules. Fixed expert systems can catch known violations, yet manually authored rule bases are costly, brittle, and difficult to transfer. Pure neural models can learn regularities but do not distinguish a reliable clinical constraint from a site-specific correlation and rarely produce a verifiable repair certificate.

The scientific problem is to learn which constraints should govern a clinical representation, quantify when they apply, and use them for minimal repair without overwriting valid exceptions or uncertainty.

### 3. Falsifiable dissertation thesis

**Proposed research hypothesis:** A jointly learned probabilistic temporal-constraint model with explicit applicability conditions and proof-carrying minimal repair will improve contradiction detection, false-correction rate, and downstream longitudinal reasoning under domain shift compared with unconstrained neural extraction, prompt-only self-revision, knowledge-graph lookup, and fixed-rule validation.

The thesis fails if learned constraints do not transfer beyond the training site/domain, if repair harms semantic fidelity despite reducing formal violations, or if fixed rules plus a strong language model perform equivalently. All aims test the same claim: learned executable constraints can add reliable, auditable structure beyond either neural or fixed-symbolic methods alone.

### 4. Evidentiary basis

#### Especially relevant sources

1. Prenosil et al., “Neuro-symbolic AI for auditable cognitive information extraction from medical reports,” *Communications Medicine* (2025), DOI [10.1038/s43856-025-01194-x](https://doi.org/10.1038/s43856-025-01194-x) (**LIT-028**, SCREENED).
2. Zhang et al., “A neural-symbolic AI agent system for biomedical concept mapping,” *npj Digital Medicine* (2026), DOI [10.1038/s41746-026-02594-6](https://doi.org/10.1038/s41746-026-02594-6) (**LIT-029**, SCREENED).
3. Su et al., “KGARevion: An AI Agent for Knowledge-Intensive Biomedical QA,” ICLR 2025, arXiv:[2410.04660](https://arxiv.org/abs/2410.04660) (**LIT-001**, READ).
4. Theodorou et al., “ConSequence: Synthesizing Logically Constrained Sequences for Electronic Health Record Generation,” AAAI 2024, DOI [10.1609/aaai.v38i14.29460](https://doi.org/10.1609/aaai.v38i14.29460).
5. Cui et al., TIMER, *npj Digital Medicine* (2025), DOI [10.1038/s41746-025-01965-9](https://doi.org/10.1038/s41746-025-01965-9).
6. Zhang et al., “Temporal Cohort Logic,” *AMIA Annual Symposium Proceedings* (2022 proceedings; PubMed record 2023), PMID [37128360](https://pubmed.ncbi.nlm.nih.gov/37128360/).

#### Claim → source → evidentiary status

| Claim | Source(s) | Evidentiary status |
|---|---|---|
| A fixed-rule neuro-symbolic system corrected reported trigger-word, missing-temporal-reasoning, and hallucinated-context failures in a narrow medical-report extraction study. | Prenosil et al. / LIT-028 | **Source-supported finding.** It was a proof of concept on 206 reports with a human-designed rule base, not evidence of broad generalization. |
| Neural-symbolic agentic reformulation improves long-tail biomedical concept mapping on several benchmarks. | Zhang et al. / LIT-029 | **Source-supported finding.** This addresses concept normalization, not trajectory-wide constraint induction. |
| KG-based verification and revision can improve biomedical QA. | KGARevion / LIT-001 | **Source-supported finding.** The KG is used to validate generated triplets; this is dangerous overlap for any generic “generate then verify” claim. |
| Hard and soft temporal/spatial constraints can be efficiently enforced in synthetic EHR generation. | ConSequence | **Source-supported finding.** The constraints are supplied rather than learned from heterogeneous clinical evidence. |
| Formal temporal languages and time-aware learning are feasible in biomedicine. | Temporal Cohort Logic; TIMER | **Source-supported finding.** Neither source alone establishes the proposed repair framework. |
| Learning applicability-scoped constraints and using them for minimal auditable repair is distinct from fixed validation or concept mapping. | Cross-source comparison | **Cross-paper inference.** Requires adversarial review of constraint learning, program synthesis, and database repair literatures. |

### 5. Closest prior work

Prenosil et al. is the closest biomedical proof that symbolic rules can repair LLM failures. KGARevion is the closest generate–verify–revise architecture. ConSequence is the closest explicit temporal-constraint enforcement method in EHR sequences. Zhang et al. occupies neural-symbolic biomedical mapping, while TIMER occupies longitudinal temporal modeling.

Outside the initial medical search, probabilistic logic, differentiable logic, inductive logic programming, program synthesis, and database-repair work are likely the most dangerous methodological neighbors. Day 2 must search those fields directly; medical novelty alone is insufficient.

### 6. Evidence-supported limitations of existing approaches

**Limitations explicitly reported by sources:**

- Prenosil et al. reports missing temporal reasoning and context hallucination in the LLM-only condition; its own solution depends on a human-authored ontology/rule base and is evaluated in a narrow report type.
- Zhang et al. frames rule-based mapping as interpretable but difficult to scale and learning methods as weak on long-tail concepts and explainability.
- ConSequence reports that earlier constrained-generation approaches may not guarantee satisfaction or efficiently handle temporal constraints.
- TIMER reports deficiencies in multi-visit temporal reasoning.

**Limitations inferred here:**

- Triple-level KG membership cannot express all interval, episode, negation, and exception constraints.
- A zero-violation output can still be clinically wrong if the rule is inapplicable or the repair deletes a legitimate exception.
- Fixed constraints cannot adapt to new documentation practices without manual maintenance; unconstrained learning may encode institutional artifacts as rules.

### 7. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

There appears to be room for a clinical representation-repair framework that jointly (a) induces interpretable temporal/ontological constraints with explicit scopes and uncertainty, (b) localizes which extracted facts cause a violation, and (c) proposes minimal repairs with proof traces and calibrated permission to leave a case unresolved. The novelty cannot be “LLM plus rules” or “KG verification.”

### 8. Proposed methodological contribution

The proposed object is a **probabilistic temporal constraint and repair calculus**:

- a typed interval-based language for events, concepts, negation, uncertainty, provenance, and exceptions;
- constraint induction from data, ontologies, guidelines, and limited expert labels, with applicability and confidence estimates;
- a minimal-repair algorithm that can correct, retract, split, re-time, or leave unresolved an assertion;
- a proof trace naming the violated constraints, supporting evidence, and repair cost;
- a benchmark that separates violation detection, constraint validity, repair fidelity, and downstream utility.

### 9. Coherent dissertation aims

**Aim 1 — Define and measure clinically meaningful representation violations.**

- **Question:** Which temporal and ontological failures can be annotated reliably, and which require preserving ambiguity?
- **Method:** Develop a typed constraint language and perturbation benchmark from open/credentialed clinical sequences, with natural and controlled violations.
- **Experiment:** Measure violation prevalence, expert agreement, and downstream impact on cohort queries, summarization, or clinical QA.
- **Expected evidence:** A validated error taxonomy, benchmark, and an empirical ceiling for rule-based detection.

**Aim 2 — Induce constraints and perform proof-carrying minimal repair.**

- **Question:** Can constraints be learned without turning common correlations into false clinical rules?
- **Method:** Combine constrained program induction or probabilistic logic with provenance-aware neural proposal models and explicit exception handling.
- **Experiment:** Compare against unconstrained extraction, prompt self-revision, ontology/KG validation, fixed rules, and neural constrained decoding; ablate each knowledge source and repair operation.
- **Expected evidence:** Higher violation detection and semantic repair accuracy with lower false-correction rates, plus trace fidelity verified by experts.

**Aim 3 — Test transfer and downstream value.**

- **Question:** Do learned constraints transfer across institutions, specialties, and representation tasks?
- **Method:** Separate invariant constraints from site-specific constraints; calibrate or abstain under shift.
- **Experiment:** Train on one dataset/domain, test on another; measure both constraint transfer and effects on a downstream longitudinal reasoning task.
- **Expected evidence:** Demonstrated transferable constraint classes and explicit failure boundaries.

### 10. Publication decomposition

1. **Formalism/benchmark:** clinical temporal-constraint language, violation corpus, and evaluation protocol.
2. **Core method:** probabilistic constraint induction and proof-carrying minimal repair.
3. **Transfer/downstream validation:** cross-site or cross-domain constraint transfer and effect on cohort/QA tasks.

If Aim 3 fails, Aims 1 and 2 can still support a defensible dissertation if they establish a general method and carefully bounded in-domain evidence. If Aim 2 fails to outperform fixed rules, the thesis is not defensible merely from the benchmark.

### 11. Evaluation strategy

- **Datasets/environments:** Synthea for controlled sequences; MIMIC-IV and MIMIC-IV-Note under PhysioNet requirements; clinical temporal-relation corpora such as i2b2/n2c2 where access permits; open biomedical ontologies; a second domain with different event structure for transfer.
- **Strongest baselines:** unconstrained structured extraction; TIMER-style temporal models; KGARevion-style KG verification; Prenosil-style fixed rules; ConSequence-style constraint enforcement; constrained decoding; prompt-based critique/revision; database-repair solvers with oracle rules.
- **Ablations:** constraint source, temporal operators, provenance, uncertainty, exception handling, repair minimality, neural proposer, symbolic solver, and abstention.
- **Primary metrics:** constraint precision/recall; violation localization F1; repair exact match and semantic equivalence; false-correction rate; minimal repair cost; temporal-relation F1; proof-trace validity; downstream query/QA performance.
- **Robustness/generalization:** documentation paraphrase, time shifts, missing events, contradictory notes, site vocabulary, rare exceptions, ontology version changes, and specialty transfer.
- **Statistics:** paired bootstrap or permutation tests; hierarchical models across constraint families and sites; confidence intervals for rare but severe false corrections; prespecified non-inferiority margins for unchanged valid cases.
- **Human evaluation:** domain experts validate constraint applicability, exceptions, and whether repairs preserve clinical meaning. Evaluation must allow multiple acceptable repairs and “unresolved.”

### 12. Required resources and feasibility

**Known available:** open ontologies and terminology services; Synthea; public code for logic/constraint solvers; PhysioNet pathways to credentialed MIMIC data; existing temporal NLP datasets subject to their agreements.

**Plausibly available:** a small expert panel for constraint review; NLP annotation support; moderate GPU compute plus CPU solver infrastructure; collaboration with a clinical NLP or knowledge-representation group.

**Currently uncertain:** enough naturally occurring violations; annotation reliability for exceptions; access to cross-site data; computational tractability of repair on long trajectories; whether rules learned in one institution transfer.

The first two aims can proceed on public/credentialed resources, but credible transfer evidence likely needs a second dataset. The direction should not rely on one mentor-controlled corpus.

### 13. Novelty-collision risks

- Inductive logic programming or differentiable-logic work may already provide the core learning method.
- Database-repair research may already formalize minimal repairs and provenance more rigorously.
- Prenosil, KGARevion, ConSequence, and newer biomedical neural-symbolic systems sharply reduce novelty for integration claims.
- A reviewer may see the clinical constraint language as an application-specific schema rather than a scientific contribution.
- Learned constraints may encode documentation frequency, demographic bias, or treatment practice rather than clinical validity.
- Stronger structured-output models may commoditize extraction; fixed ontology APIs may beat learned constraints on many errors.

### 14. Advisor / expertise complementarity

**Required methodological configuration:** the direction needs neuro-symbolic or probabilistic-logic learning, temporal/formal constraint solving, minimal repair and provenance, plus clinical NLP, EHR representation, and domain validation. A database theory or formal-methods collaborator would materially strengthen the repair semantics.

The current official [IHI Graduate Program Directory](https://healthinformatics.umn.edu/graduate-program/graduate-program-directory) lists both faculty below as Core Faculty, making them plausible primary-advisor options subject to formal confirmation:

- **Steven Johnson — strongest fit if the dissertation centers on clinical ontologies, data-quality constraints, and EHR representation repair.** Johnson's [official IHI profile](https://healthinformatics.umn.edu/staff/steven-johnson) explicitly identifies clinical knowledge representation and ontologies, EHR data quality and secondary use, clinical decision support, and machine learning. [Dr. Rui Zhang](https://med.umn.edu/bio/rui-zhang) contributes clinical NLP/information extraction, LLM methods, biomedical literature mining, multimodal EHR analysis, and knowledge-graph development. The combination is complementary because Johnson can anchor the symbolic vocabulary, data-quality semantics, clinical-system integration, and downstream decision-support validity, while Zhang can anchor the neural extraction/proposal layer and knowledge-graph-grounded language processing.
- **Sisi Ma — strongest fit if the dissertation centers on learning probabilistic constraints from high-dimensional biomedical data and benchmarking their transfer.** Ma's [official IHI profile](https://healthinformatics.umn.edu/staff/sisi-ma) emphasizes statistical modeling, machine learning, causal discovery tailored to biomedical data, multimodal high-dimensional analysis, and benchmarking new and existing methods. Zhang would contribute the NLP/IE, LLM, literature, and knowledge-graph substrate from which candidate constraints and structured assertions are derived. The combination separates statistical constraint induction and rigorous benchmarking from language-based extraction and biomedical knowledge construction; a functional-genomics validation branch would also align with Ma's biomedical causal-modeling background.

Neither option alone supplies the full database-repair/formal-verification stack, so an additional collaborator in logic, programming languages, or database theory may be essential. Methodological fit does not establish willingness, availability, funding, commitment, annotation access, or final advising eligibility.

### 15. Foundation-model resilience

Better foundation models may reduce raw extraction errors, but they do not guarantee constraint satisfaction, explain applicability, distinguish hard rules from exceptions, or certify a minimal repair. The direction remains interesting if it produces executable semantics and independently checkable traces. It becomes weak if “neuro-symbolic” means only asking a stronger model to critique its own output.

### 16. Publication and execution risk

- **Novelty bar:** very high because neural-symbolic medicine is now visibly active.
- **Time to first credible unit:** moderate; the benchmark/formalism is publishable if empirically grounded.
- **Dependence on one high-risk experiment:** high for the thesis, because learned constraints must outperform strong fixed and neural baselines.
- **Ground-truth difficulty:** high, especially for exceptions and missingness.
- **Reproducibility:** high on released perturbations and solvers; lower for restricted natural-error corpora.
- **Risk of being overtaken:** high for generic LLM-plus-rules systems, moderate for a rigorous constraint-induction and repair theory.

### 17. Generalizability

**Healthcare-specific contribution:** representations must encode clinical event intervals, documentation uncertainty, negation, episode boundaries, ontologies, and legitimate exceptions.

**Methodologically transferable contribution:** learning applicability-scoped constraints and proof-carrying minimal repairs for neural-to-structured pipelines in scientific databases, compliance, and other temporally structured domains.

### 18. Strongest reason to reject the direction

The strongest objection is epistemic: observational regularities are not clinical rules. A learned constraint system may look auditable while institutionalizing spurious practice patterns and “repairing” legitimate rare cases into conformity. If that cannot be controlled and measured, explicit logic makes the system more confidently wrong rather than safer.

### 19. What evidence would change the recommendation?

- **Substantially strengthen:** high inter-expert agreement on a useful constraint core; a clear theoretical distinction from existing repair/program-induction methods; lower false-correction rates under cross-site shift; downstream benefits not explained by simpler validation.
- **Substantially weaken:** most useful constraints are easy to hand-code; learned rules fail on rare exceptions; expert trace review is not reproducible.
- **Kill outright:** strong prior work already provides the same scoped constraint induction and minimal repair, or controlled tests show that reducing formal violations does not improve—and sometimes harms—semantic correctness.

### 20. Day 1 verdict

**ADVANCE WITH MAJOR UNCERTAINTY**

The direction has real methodological depth and a non-ceremonial role for neuro-symbolic AI. It also faces the highest novelty collision and epistemic-validity risks in this set. It should advance only to targeted Day 2 searches in program induction, temporal logic, and database repair.

---
## D02-03 — Machine-checkable causal data-fit contracts for EHR target-trial emulation

### 1. Candidate identity

**Title:** Machine-checkable causal data-fit contracts for EHR target-trial emulation

**One-sentence identity:** This direction studies formal, executable contracts that determine whether an intended target-trial estimand is supported by a specific EHR data-generating process and that return a validated design, a defensible restricted estimand, a request for missing information, or a refusal to estimate.

### 2. Central scientific problem

Target-trial emulation imposes useful design discipline, but a well-written protocol does not make its causal contrast identifiable in an EHR. Eligibility, time zero, treatment strategies, confounders, adherence, outcomes, and follow-up must be mapped to data generated by care and documentation processes rather than randomization. Current automation can translate study descriptions into structured specifications and executable code, yet faster execution can scale an invalid design as readily as a valid one.

The methodological problem is how to make the mapping from causal question to available data explicit and machine-checkable before estimation. The system must represent untestable assumptions honestly, compile testable implications into diagnostics, detect estimand drift, and treat “not identifiable with these data” as a valid output.

This matters scientifically because false precision in real-world evidence can influence clinical and policy decisions, and operational errors can persist despite sophisticated estimators.

### 3. Falsifiable dissertation thesis

**Proposed research hypothesis:** A typed causal data-fit contract that jointly encodes the target-trial protocol, causal assumptions, temporal observability, data provenance, and executable diagnostics will detect invalid or estimand-altering EHR emulations and reduce causal estimation error and false assurance relative to reporting checklists, unconstrained LLM assistants, and code-generation pipelines, while preserving automation for data-supported questions.

The thesis is falsified if contract verdicts do not predict bias or estimand mismatch in settings with known ground truth, if experts cannot agree on contract semantics, or if standard diagnostics/checklists perform equivalently. The aims test contract expressiveness, decision validity, and empirical transfer as one coherent thesis.

### 4. Evidentiary basis

#### Especially relevant sources

1. Wang et al., “An operational target trial emulation framework for causal inference using electronic health record data,” *npj Digital Medicine* (2026), DOI [10.1038/s41746-026-02563-z](https://doi.org/10.1038/s41746-026-02563-z).
2. Kim et al., “From study design to executable code: automating target trial emulation with large language models,” *JAMIA Open* (2026), DOI [10.1093/jamiaopen/ooag131](https://doi.org/10.1093/jamiaopen/ooag131).
3. Sawarni, Tan, and Syrgkanis, “CausalReasoningBenchmark: A Real-World Benchmark for Disentangled Evaluation of Causal Identification and Estimation,” arXiv:[2602.20571](https://arxiv.org/abs/2602.20571) (v2, 2026).
4. Habibdoust and Song, “TrialCalibre: A Fully Automated Causal Engine for RCT Benchmarking and Observational Trial Calibration,” arXiv:[2604.25832](https://arxiv.org/abs/2604.25832) (2026).
5. Hernán and Robins, “Using Big Data to Emulate a Target Trial When a Randomized Trial Is Not Available,” *American Journal of Epidemiology* (2016), DOI [10.1093/aje/kwv254](https://doi.org/10.1093/aje/kwv254).
6. Su et al., “TrialEmulation: An R Package to Emulate Target Trials for Causal Analysis of Observational Time-to-event Data,” arXiv:[2402.12083](https://arxiv.org/abs/2402.12083) (2024).

#### Claim → source → evidentiary status

| Claim | Source(s) | Evidentiary status |
|---|---|---|
| Target-trial specification helps prevent design errors, but validity still depends on mapping the trial components and assumptions to observational data. | Hernán and Robins; Wang et al. | **Source-supported finding/framework.** |
| In EHR settings, care-driven observation, missingness, time-zero construction, treatment assignment, and follow-up can make the intended causal contrast unsupported; a valid conclusion can be not to pursue the emulation. | Wang et al. | **Source-supported finding/framework.** The paper explicitly frames EHR TTE as a data-constrained design problem. |
| LLM-assisted standardization can map selected free-text design elements to structured OHDSI/Strategus specifications and deterministic code with high field-level performance under study conditions. | Kim et al. / THESEUS | **Source-supported finding and dangerous prior art.** The reported scope centered on standardized fields and human review, not full causal validity certification. |
| Current automated causal systems can identify a high-level strategy more often than they correctly specify all identification details. | CausalReasoningBenchmark | **Source-supported finding.** In v2, the reported baseline obtained 79% high-level strategy identification but 34% full identification-specification correctness. |
| Multi-agent automation of observational calibration is already proposed. | TrialCalibre | **Source-supported finding and dangerous prior art.** The short paper is a conceptualized system, which makes generic “causal agent” novelty untenable. |
| A formal contract that connects assumptions and observability to executable diagnostics could reduce false assurance. | Synthesis above | **Cross-paper inference and proposed research hypothesis.** No cited source demonstrates that result. |

### 5. Closest prior work

Wang et al. is the closest conceptual account of data-constrained target-trial feasibility. THESEUS is the closest executable LLM-assisted workflow. TrialEmulation provides implementation infrastructure, while TrialCalibre is a direct collision with broad autonomous-causal-engine framing. CausalReasoningBenchmark is the closest evaluation showing that identification details, not only numerical estimation, are a bottleneck.

The candidate therefore cannot be “an agent that automates target-trial emulation.” Its proposed contribution must be a machine-checkable semantics for data fitness, estimand change, assumption status, and refusal, plus evidence that those contracts improve causal validity.

### 6. Evidence-supported limitations of existing approaches

**Limitations explicitly reported by sources:**

- Wang et al. details systemic EHR barriers and emphasizes that statistical adjustment cannot recover a contrast unsupported by the data.
- THESEUS reports lower and more variable performance for some fields, restricts its proof of concept to selected specification components, and includes human review before code generation.
- CausalReasoningBenchmark separates identification from estimation and reports a large gap between high-level strategy recognition and full specification correctness.
- The target-trial framework prevents some design errors but does not solve data limitations or unmeasured confounding.

**Limitations inferred here:**

- A schema that faithfully copies a study description can reproduce an invalid assumption without detecting it.
- Passing balance or overlap diagnostics after cohort construction does not prove that time zero, eligibility, treatment, and outcome were operationalized without post-baseline or selectively observed information.
- Existing checklists are human-readable but not necessarily executable, compositional, or capable of returning a formally restricted estimand.

### 7. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

There appears to be unresolved space for an executable causal-contract layer that sits between target-trial specification and estimation, distinguishes declared assumptions from testable data conditions, detects when the implemented study targets a different estimand, and supports structured refusal or restriction. This claim must be tested against causal programming languages, automated data-quality systems, negative-control frameworks, and formal methods for causal identification—not only health-informatics papers.

### 8. Proposed methodological contribution

The dissertation would contribute a **causal data-fit contract language and compiler**:

- typed objects for population, treatment strategies, assignment, time zero, follow-up, outcomes, estimand, censoring, confounding, transportability, and data provenance;
- explicit labels for assumed, observed, computable, proxy-derived, and unavailable elements;
- static checks for temporal leakage, ill-defined interventions, incompatible time anchors, and unsupported mappings;
- compiled diagnostics for positivity, measurement/observation processes, missingness, sensitivity, negative controls, and robustness;
- a decision layer returning `supported`, `supported for a restricted estimand`, `requires information`, or `not supported`;
- a provenance-preserving record of every design compromise and its effect on interpretation.

An LLM may translate prose into the contract, but a deterministic/causal engine must evaluate the contract. The contribution is not natural-language code generation.

### 9. Coherent dissertation aims

**Aim 1 — Formalize data fitness and build a falsification benchmark.**

- **Question:** Can common EHR target-trial failures and estimand changes be represented in an executable, expert-auditable contract?
- **Method:** Define semantics with causal-inference experts; create challenge cases from published designs, simulations, and semi-synthetic EHRs with controlled violations.
- **Experiment:** Compare contract and expert verdicts; measure whether each violation changes bias, coverage, or the estimand.
- **Expected evidence:** Expressiveness, inter-rater agreement, a benchmark with known failure mechanisms, and clear classes that remain untestable.

**Aim 2 — Learn/compile contract completion and validity decisions.**

- **Question:** Can a system translate a question and data dictionary into a complete contract and safely decide when to restrict or refuse?
- **Method:** Use constrained semantic parsing for proposal generation and a symbolic/causal compiler for checking; calibrate selective decisions rather than letting the language model certify itself.
- **Experiment:** Compare checklists, free-form LLM critique, THESEUS-like structured extraction, and oracle contracts across natural and perturbed protocols/data dictionaries.
- **Expected evidence:** Higher full-specification accuracy, violation recall, and decision calibration with fewer false-supported cases.

**Aim 3 — Test whether contracts improve end-to-end real-world evidence validity.**

- **Question:** Do contract-guided designs yield more reproducible, better-calibrated causal estimates across data sources?
- **Method:** Execute supported and deliberately violated emulations using OHDSI/Strategus or equivalent reproducible pipelines; use negative controls, simulations, and selected RCT triangulation where justified.
- **Experiment:** Multi-dataset comparison of unguided, checklist-guided, and contract-guided workflows.
- **Expected evidence:** Reduced bias/false coverage under known truth, more consistent estimates across sites, and honest refusal when assumptions or data fail.

### 10. Publication decomposition

1. **Formalism/benchmark:** contract semantics and controlled causal data-fit challenge set.
2. **Core method:** constrained contract completion, compiler, and calibrated validity/refusal decisions.
3. **Empirical validation:** reproducible target-trial emulations across datasets, negative controls, and selected trial triangulation.

If Aim 3 encounters data-access failure, Aims 1 and 2 could still support a dissertation only with strong simulation/semi-synthetic evidence and at least one real-data demonstration. If the contract cannot detect known design failures in Aim 1, later publications do not rescue the central thesis.

### 11. Evaluation strategy

- **Datasets/environments:** synthetic structural causal models with known effects; semi-synthetic longitudinal EHRs; MIMIC-IV for appropriate non-proprietary demonstrations; public OHDSI tools and publicly documented studies; multiple OMOP data dictionaries; RCT-linked or negative-control tasks where legally and scientifically appropriate.
- **Strongest baselines:** human reporting checklists; free-form frontier-LLM review; THESEUS-like structured extraction; TrialEmulation/Strategus workflows; static rule checks; expert causal review; oracle protocol and oracle data dictionary.
- **Ablations:** remove provenance, temporal checks, observation-process model, sensitivity compilation, restriction/refusal, deterministic compiler, and human review.
- **Primary metrics:** full contract exact/semantic correctness; violation detection sensitivity and specificity; false-supported rate; estimand-match accuracy; bias, RMSE, confidence-interval coverage, and type-I error under known truth; negative-control calibration; cross-site heterogeneity; time and effort.
- **Robustness/generalization:** paraphrased protocols, incomplete dictionaries, coding drift, alternative time-zero definitions, missing confounders, poor overlap, informative observation, site shift, and intervention ambiguity.
- **Statistics:** repeated simulations over data-generating mechanisms; paired comparisons on identical studies; bootstrap uncertainty for real-data contrasts; empirical coverage/type-I error; hierarchical analysis across failure families; predeclared primary validity endpoints.
- **Human evaluation:** causal-inference experts adjudicate semantics and design validity; clinicians/informaticians assess whether data mappings reflect care processes. Agreement and unresolved cases are outcomes, not nuisances to erase.

### 12. Required resources and feasibility

**Known available:** mature causal-inference and OHDSI software; public simulation frameworks; public protocol/reporting literature; CausalReasoningBenchmark; credentialed MIMIC pathways; reproducible containerized analysis tools.

**Plausibly available:** one causal-inference/biostatistics collaborator; access to at least one OMOP environment or synthetic OMOP instance; faculty expertise in EHR data generation; compute requirements that are moderate relative to foundation-model training.

**Currently uncertain:** multi-site patient-level access; usable RCT comparators; expert time for contract gold standards; whether some data-fit judgments can be operationalized without detailed local workflow knowledge; institutional support for external validation.

The method should be developed and falsified on simulation plus public/credentialed resources before depending on a restricted network. A successful dissertation cannot require a single enclave, health system, or collaborator to supply every positive result.

### 13. Novelty-collision risks

- THESEUS and rapidly advancing OHDSI automation may extend from specification extraction into validity checks.
- TrialCalibre and other causal agents may claim an overlapping end-to-end architecture.
- Causal programming languages, do-calculus engines, study-design checkers, or data-quality tools may already implement substantial contract semantics.
- Reviewers may argue that the work formalizes expert checklists without new causal theory.
- Many causal assumptions are not testable from observed data; a contract can document but not verify them.
- Stronger foundation models may commoditize prose-to-schema translation, leaving only the checker as the durable contribution.

The direction becomes incremental engineering if it only wraps existing diagnostics in JSON or an agent interface.

### 14. Advisor / expertise complementarity

**Required methodological configuration:** the primary advisor must bring credible causal-method depth—identification assumptions, causal discovery/inference, simulation, and statistical validation—while the broader team supplies EHR/OMOP data-generation knowledge, data quality, machine-checkable specification, and clinical interpretation.

The current official [IHI Graduate Program Directory](https://healthinformatics.umn.edu/graduate-program/graduate-program-directory) lists both faculty below as Core Faculty, making them plausible primary-advisor options subject to formal confirmation:

- **Erich Kummerfeld — strongest fit for a formally centered causal-contract dissertation.** Kummerfeld's [official IHI profile](https://healthinformatics.umn.edu/staff/erich-kummerfeld) identifies novel causal and latent-variable discovery algorithms, proofs about their properties, simulation benchmarking, and application to health data. [Dr. Rui Zhang](https://med.umn.edu/bio/rui-zhang) contributes clinical NLP/information extraction, LLMs, EHR and biomedical-literature mining, and knowledge graphs. The combination is complementary because Kummerfeld can anchor causal semantics, assumptions, falsification simulations, and validity claims, while Zhang can anchor protocol-to-structure translation, extraction of computable variables from text, and the AI interface—without allowing the LLM to certify causal validity.
- **Sisi Ma — strongest fit if the direction emphasizes biomedical causal modeling and empirical benchmarking across multimodal data.** Ma's [official IHI profile](https://healthinformatics.umn.edu/staff/sisi-ma) identifies statistical modeling, machine learning, causal discovery tailored to biomedical data, multimodal high-dimensional analysis, and benchmark design. Zhang would contribute NLP/IE for protocol, literature, and unstructured-EHR operationalization plus knowledge-graph and LLM expertise. Ma would anchor the causal/statistical tests and biomedical experiment design; Zhang would anchor the language-to-contract and data-extraction layer.

Neither match removes the need for explicit expertise in target-trial emulation, longitudinal causal inference, OMOP/EHR data quality, and possibly programming languages. These are public-evidence fit assessments only; willingness, availability, funding, commitment, data access, and final advising eligibility remain unverified.

### 15. Foundation-model resilience

This is the most foundation-model-resilient direction in the set if the contract semantics and compiler are model independent. Better language models can improve protocol parsing but cannot make an unsupported estimand identifiable, recover unobserved events, or remove the need to expose assumptions and data provenance. The direction loses resilience if its primary contribution is prompt-based critique or code generation.

### 16. Publication and execution risk

- **Novelty bar:** high, but the narrow contract/refusal object has more headroom than generic causal automation.
- **Time to first credible unit:** moderate; a formalism and falsification benchmark can precede multi-site data access.
- **Dependence on one high-risk experiment:** moderate; simulations and benchmark results can establish early claims, while real-data validation remains essential.
- **Ground-truth difficulty:** moderate in simulation, very high in real EHRs.
- **Reproducibility:** high for contracts, simulations, and open pipelines; lower for restricted multi-site analyses.
- **Risk of being overtaken:** high for LLM translation, lower for rigorous data-fit semantics, falsification, and estimand-aware refusal.

### 17. Generalizability

**Healthcare-specific contribution:** contracts must model care-driven observation, coding and encounter processes, treatment adherence, clinical time zero, and EHR provenance; these are integral rather than decorative.

**Methodologically transferable contribution:** executable data-fit contracts for causal analyses in any observational domain, including economics, public policy, and platform experimentation, where a desired estimand may not be supported by available data.

### 18. Strongest reason to reject the direction

The strongest objection is that formalization may create a misleading aura of certification around inherently untestable causal assumptions. If the system cannot distinguish “diagnostic passed” from “causal validity established,” it could make automation more dangerous. The direction also requires genuine causal-method advising and may be a poor fit if that expertise cannot be secured.

### 19. What evidence would change the recommendation?

- **Substantially strengthen:** expert agreement on contract semantics; strong sensitivity to known causal-design failures with low false-refusal rates; demonstrable bias/coverage improvements; successful independent reproduction across data sources.
- **Substantially weaken:** most verdicts depend on unobservable local knowledge; contracts add documentation but do not change designs; real-data users bypass refusal outputs.
- **Kill outright:** established tools already implement equivalent semantics and validation, or controlled experiments show no relationship between contract results and causal error/estimand fidelity.

### 20. Day 1 verdict

**ADVANCE**

This is a coherent, high-impact, technically deep direction with a durable scientific object and strong foundation-model resilience. Its biggest risks are untestable assumptions, causal-expertise requirements, and collision with causal programming/automation work—not lack of importance.

---

## D02-04 — Change-attributed continual assurance for clinical foundation-model systems

### 1. Candidate identity

**Title:** Change-attributed continual assurance for clinical foundation-model systems

**One-sentence identity:** This direction studies how to maintain a versioned, clinically grounded model of a system's failure surface and efficiently detect and localize safety regressions caused by changes in the base model, retrieval corpus, tools, prompts, policies, or input population.

### 2. Central scientific problem

Clinical foundation-model systems are compound and mutable. A release may change the base model while keeping the prompt constant; a retrieval index may ingest new evidence; a tool may alter its API; a safety policy may improve one subgroup and degrade another. Static benchmark averages cannot determine which component caused a regression, whether a failure was pre-existing, or which tests should be rerun under a limited evaluation budget.

Dynamic red-teaming and adaptive testing now demonstrate that fresh tests and high-frequency evaluation are feasible. The unresolved problem is change attribution and efficient assurance across versions: maintaining coverage of clinically meaningful failure mechanisms, selecting the next test for maximum information, controlling false alarms, and producing a reproducible failure lineage.

### 3. Falsifiable dissertation thesis

**Proposed research hypothesis:** A versioned causal failure-surface representation combined with sequential, coverage-aware test selection will detect clinically significant regressions earlier and localize their responsible system changes more accurately, at a fixed evaluation budget, than static benchmark reruns, undirected dynamic red-teaming, and accuracy-focused adaptive testing.

The thesis fails if dynamic red-teaming or simple stratified regression suites match detection and localization performance, if failure taxonomies do not transfer across releases, or if automated adjudication error dominates the monitoring signal. The aims all test efficient, attributed continual assurance—not unrelated benchmark creation.

### 4. Evidentiary basis

#### Especially relevant sources

1. Pan et al., “Addressing benchmarking gaps in large language models for health and medicine with dynamic red-teaming,” *Nature Health* (2026), DOI [10.1038/s44360-026-00152-8](https://doi.org/10.1038/s44360-026-00152-8) (**LIT-032**, SCREENED).
2. Zhang et al., “Inflated Excellence or True Performance? Rethinking Medical Diagnostic Benchmarks with Dynamic Evaluation,” ACL 2026, DOI [10.18653/v1/2026.acl-long.1218](https://doi.org/10.18653/v1/2026.acl-long.1218).
3. Zheng et al., “Leveraging computerized adaptive testing for cost-effective evaluation of large language models in medical benchmarking,” *npj Digital Medicine* (2026), DOI [10.1038/s41746-026-02671-w](https://doi.org/10.1038/s41746-026-02671-w).
4. Bilionis et al., “An empirical evaluation of the risks of AI model updates using clinical data: stability, arbitrariness, and fairness,” arXiv:[2604.23954](https://arxiv.org/abs/2604.23954) (v2, 2026; reported as IEEE EMBC 2026).
5. Chang et al., “Red teaming ChatGPT in medicine to yield real-world insights on model behavior,” *npj Digital Medicine* (2025), DOI [10.1038/s41746-025-01542-0](https://doi.org/10.1038/s41746-025-01542-0).
6. Schmidgall et al., AgentClinic, *npj Digital Medicine* (2026), DOI [10.1038/s41746-026-02674-7](https://doi.org/10.1038/s41746-026-02674-7).

#### Claim → source → evidentiary status

| Claim | Source(s) | Evidentiary status |
|---|---|---|
| Dynamic adversarial evaluation can expose failures hidden by high static medical benchmark performance. | Pan et al. / LIT-032 | **Source-supported finding.** The reported DAS framework is direct dangerous prior art for any generic dynamic health red-teaming proposal. |
| Fresh, clinically confounded diagnostic cases reveal weaknesses not captured by exam-style benchmarks. | DyReMe | **Source-supported finding.** This supports dynamic case generation, not change attribution. |
| Adaptive testing can approximate full-bank model rankings with a small fraction of items and substantially lower cost. | Zheng et al. | **Source-supported finding.** It measures standardized medical knowledge and explicitly does not replace safety/prospective evaluation. |
| Updating a clinical model can change stability, arbitrariness, and subgroup fairness even when updating is necessary. | Bilionis et al. | **Source-supported finding.** Demonstrated in a pediatric diabetes prediction case study. |
| Later model versions can regress on prompts that earlier versions handled appropriately. | Chang et al. | **Source-supported finding.** Their iterative benchmark found such reversals across tested ChatGPT versions. |
| A versioned factor model can localize regressions and optimize test allocation across compound system changes. | Synthesis above | **Proposed research hypothesis.** None of the cited studies proves this. |

### 5. Closest prior work

DAS/LIT-032 is the closest and most dangerous overlap: it already claims dynamic, automatic, systematic red-teaming that evolves with models. DyReMe generates dynamic clinical diagnostic evaluations. Computerized adaptive testing already optimizes item selection for efficient measurement. Chang et al. and Bilionis et al. explicitly study changes across model versions or updates.

The candidate survives only by centering **attribution across a versioned compound system**, calibrated regression detection, and coverage-aware test allocation. “Continuous evaluation,” “dynamic benchmark,” or “automated red team” alone are no longer plausible dissertation contributions.

### 6. Evidence-supported limitations of existing approaches

**Limitations explicitly reported by sources:**

- DAS argues static benchmarks become obsolete or gameable and reports large dynamic failure rates across robustness, privacy, bias, and hallucination.
- DyReMe reports that public exam benchmarks omit clinically grounded confounders and broader trustworthiness dimensions.
- Zheng et al. limits adaptive testing to efficient foundational-knowledge screening and states that it is not a substitute for real-world or safety validation.
- Chang et al. demonstrates that aggregate “newer model” expectations can hide prompt-level regressions.
- Bilionis et al. shows model updating can alter stability and fairness.

**Limitations inferred here:**

- Existing dynamic evaluators mostly search for failures in the current target; they do not necessarily estimate which changed component caused a new failure.
- Adaptive item response theory optimizes trait estimation, not discovery of rare, interacting safety failures.
- Re-running every test after every component change is financially and clinically expensive, while aggregate scores can mask severe subgroup regressions.

### 7. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

There appears to be unresolved methodological space for a continual-assurance framework that represents system versions and failure mechanisms jointly, uses controlled paired perturbations to attribute regressions, and allocates tests sequentially under explicit detection and false-alarm objectives. This gap is narrower than dynamic red-teaming and must be tested against software regression testing, causal fault localization, active testing, reliability engineering, and ML monitoring literatures.

### 8. Proposed methodological contribution

The dissertation would contribute:

1. **A versioned failure-surface representation** linking clinical task, harm mechanism, subgroup/context, system component versions, evidence source, and observed counterexample.
2. **A paired counterfactual test design** that holds a case or component constant while perturbing model, retrieval, tool, instruction, policy, or input factors to estimate change attribution.
3. **A budgeted sequential assurance algorithm** that selects tests to maximize expected clinically weighted failure discovery and component localization while controlling false alarms.
4. **An assurance dossier format** preserving counterexample lineage, adjudication uncertainty, mitigations, and re-test obligations.

This must produce statistical or algorithmic contributions beyond an evaluation dashboard.

### 9. Coherent dissertation aims

**Aim 1 — Define and measure versioned clinical regressions.**

- **Question:** Which failure changes are reproducible, clinically meaningful, and attributable rather than stochastic?
- **Method:** Build a factorial benchmark of archived system versions and controlled component changes with clinician-validated failure categories.
- **Experiment:** Compare aggregate scores, paired-case analyses, and replicated outputs; estimate adjudicator and model stochasticity.
- **Expected evidence:** A validated failure ontology, reproducibility thresholds, and quantified regression prevalence.

**Aim 2 — Learn budgeted regression discovery and fault localization.**

- **Question:** Can sequential selection discover serious regressions and identify responsible changes using fewer evaluations?
- **Method:** Combine hierarchical Bayesian or causal factor models, active test selection, and severity-weighted objectives with explicit false-alarm control.
- **Experiment:** Hidden-change challenges across model, corpus, prompt, tool, and policy updates; compare static suites, random/stratified sampling, CAT, and DAS-like search.
- **Expected evidence:** Lower detection delay and evaluation cost, higher severe-failure recall, and more accurate component attribution.

**Aim 3 — Test prospective transfer to a changing clinical-agent workflow.**

- **Question:** Does the assurance method remain useful as tasks and models evolve beyond the development benchmark?
- **Method:** Shadow-monitor a non-deployed or research clinical agent across planned updates, with all data and model versions recorded.
- **Experiment:** Prospective pre/post update audits and replay of accumulated counterexamples; evaluate whether predicted high-risk regions capture later expert-confirmed regressions.
- **Expected evidence:** Prospective utility, reusable counterexamples, and clear limits on transfer.

### 10. Publication decomposition

1. **Measurement/benchmark:** versioned clinical regression benchmark and reproducibility methodology.
2. **Core method:** budgeted sequential detection and causal/component fault localization.
3. **Prospective/generalization study:** continual assurance in a changing compound clinical agent.

If Aim 3 fails because a partner workflow is unavailable, Aims 1 and 2 can support a dissertation if the hidden-change benchmark spans multiple independently sourced systems. If Aim 2 does not beat simple stratified regression suites, a benchmark and dashboard alone are insufficient.

### 11. Evaluation strategy

- **Datasets/environments:** archived open-weight model releases; versioned retrieval corpora; AgentClinic and other licensed/open clinical-agent simulations; MedQA/HealthBench-derived seeds only where licenses permit; DyReMe-style generated cases; clinician red-team cases; synthetic component faults with known attribution.
- **Strongest baselines:** full static rerun; random and stratified sampling; computerized adaptive testing; DAS-like dynamic red-teaming; DyReMe-style dynamic generation; standard drift/change-point monitoring; software regression prioritization; oracle change labels.
- **Ablations:** failure hierarchy, severity weights, paired design, version graph, adjudication uncertainty, active selection, replay memory, and each component-change factor.
- **Primary metrics:** severe-regression recall; detection delay; false-alarm rate; evaluation cost; component-attribution accuracy; failure-mode coverage/diversity; worst-group risk; reproducibility; counterexample retention value.
- **Robustness/generalization:** stochastic generations, judge drift, multiple simultaneous changes, unseen tasks, new models, evidence-corpus updates, prompt paraphrases, tool failures, and subgroup shifts.
- **Statistics:** sequential testing with alpha-spending or false-discovery control; survival/time-to-detection analysis; paired mixed-effects models; uncertainty propagation from human labels; confidence intervals on rare severe events.
- **Human evaluation:** clinicians adjudicate harm severity and clinical correctness on sampled/contested cases. Privacy experts or other domain reviewers should assess specialized axes. LLM judges require calibration against humans and monitoring for judge-version drift.

### 12. Required resources and feasibility

**Known available:** multiple open-weight model versions; public benchmark seeds and agent environments; containerization/version control; dynamic-evaluation and red-team papers/code where released; moderate cloud/API compute.

**Plausibly available:** clinician review of a targeted rather than exhaustive sample; a research clinical-agent pipeline for shadow evaluation; archived retrieval snapshots; software/reliability expertise.

**Currently uncertain:** stable access to proprietary historical model versions; a prospective partner workflow; enough ground-truth component changes; costs for large adaptive searches; validity of automated judges across versions; licensing of some benchmark content.

The core benchmark should be reproducible with open models and synthetic/controlled changes. Proprietary APIs can be a stress test but not the only evidence. No PHI or private institutional performance data should be required for the first two aims.

### 13. Novelty-collision risks

- DAS already occupies dynamic, automated, evolving health red-teaming and explicitly anticipates evaluation after model updates.
- DyReMe occupies dynamic clinical case generation; CAT occupies efficient repeated testing.
- Software testing and fault-localization research may already provide stronger algorithms than a health-specific reinvention.
- A failure graph plus scheduler may be judged as quality-assurance engineering unless it has formal detection/localization properties and convincing experiments.
- LLM judges and generated attacks may co-adapt or share blind spots with the evaluated model.
- As base models improve, many current failure prompts will stop discriminating; the method must preserve mechanisms, not memorize cases.

### 14. Advisor / expertise complementarity

**Required methodological configuration:** the direction needs statistical ML evaluation, sequential/adaptive experimental design, change detection and fault localization, together with EHR data quality, clinical decision-support context, and safety adjudication. Software reliability or psychometrics would be valuable additional strengths.

The current official [IHI Graduate Program Directory](https://healthinformatics.umn.edu/graduate-program/graduate-program-directory) lists both faculty below as Core Faculty, making them plausible primary-advisor options subject to formal confirmation:

- **Sisi Ma — strongest fit if the dissertation's center is the statistical benchmark, sequential test-selection method, and attribution analysis.** Ma's [official IHI profile](https://healthinformatics.umn.edu/staff/sisi-ma) emphasizes statistical modeling, machine learning, causal analysis, and benchmarking novel and existing methods on biomedical data. [Dr. Rui Zhang](https://med.umn.edu/bio/rui-zhang) contributes clinical AI/LLM and NLP/IE systems, multimodal biomedical data, knowledge graphs, and publicly documented work on model fairness. The combination is complementary because Ma can anchor statistical validity, comparison design, and attribution methodology, while Zhang supplies realistic changing clinical-AI systems, language-model failure modes, and domain-grounded evaluation targets.
- **Steven Johnson — strongest fit if the dissertation is framed around compound clinical-system changes, EHR data quality, and decision-support assurance.** Johnson's [official IHI profile](https://healthinformatics.umn.edu/staff/steven-johnson) identifies EHR data quality and secondary use, clinical decision support, ontologies, machine learning, research data-warehouse oversight, and national research-network collaborations. Zhang would contribute the LLM/NLP/knowledge-graph components and health-AI model behavior. The complementarity is systems-oriented: Johnson can anchor data and workflow change, clinical decision-support infrastructure, and reproducible EHR evaluation; Zhang can anchor the rapidly changing foundation-model and language-processing components whose failures must be monitored.

A clinical safety expert and a software-reliability or sequential-testing collaborator may still be required, particularly for prospective Aim 3. Methodological fit does not establish willingness, availability, funding, commitment, access to a monitored workflow, or final advising eligibility.

### 15. Foundation-model resilience

Continual assurance becomes more—not less—necessary when base models and compound systems change rapidly. The scientific contribution survives if it concerns versioned failure mechanisms, efficient detection, attribution, and auditable evidence. It does not survive if it is a fixed benchmark of today's model weaknesses or a vendor-specific monitoring wrapper.

### 16. Publication and execution risk

- **Novelty bar:** very high because dynamic medical evaluation advanced sharply in 2026.
- **Time to first credible unit:** relatively short for a versioned-regression measurement paper.
- **Dependence on one high-risk experiment:** moderate; prospective Aim 3 is risky, but controlled hidden-change studies can test Aim 2.
- **Ground-truth difficulty:** high for harm and attribution; lower for injected component changes.
- **Reproducibility:** high with open models and archived containers, low with disappearing proprietary versions.
- **Risk of being overtaken:** high for generic red-teaming, lower for rigorous change attribution and sequential assurance.

### 17. Generalizability

**Healthcare-specific contribution:** clinically weighted failure modes, subgroup harms, evidence updates, privacy, and workflow consequences determine the evaluation objective and human adjudication.

**Methodologically transferable contribution:** continual assurance and fault localization for changing compound AI systems in finance, law, science, and critical infrastructure. Healthcare is integral because rare severe failures and component interactions make average-accuracy monitoring inadequate.

### 18. Strongest reason to reject the direction

DAS and neighboring work may have consumed the most publishable novelty, leaving a labor-intensive evaluation platform with no central scientific advance. If attribution is unreliable because model stochasticity, judge error, and simultaneous updates overwhelm controlled effects, the proposed failure-surface formalism will not justify a dissertation.

### 19. What evidence would change the recommendation?

- **Substantially strengthen:** a clear formal distinction from DAS/CAT; accurate localization of hidden component changes; large cost reductions at fixed severe-regression recall; prospective prediction of later failures.
- **Substantially weaken:** active selection finds only easy failures; human labels are unstable; version-factor effects do not transfer; full reruns are cheap enough to dominate.
- **Kill outright:** adjacent work already performs equivalent versioned attribution and budgeted testing in compound clinical agents, or controlled evaluations show no advantage over stratified replay plus dynamic red-teaming.

### 20. Day 1 verdict

**ADVANCE WITH MAJOR UNCERTAINTY**

The direction is important, artifact-rich, executable, and highly resilient to stronger models. It advances only in the narrower change-attribution and sequential-assurance form; generic continuous evaluation or red-teaming is already too crowded.

---

## Portfolio-level analysis

### A. Candidate diversity check

The four candidates are genuinely different scientific directions, though two pairs share a broader family boundary:

- **D02-01 and D02-04** both concern reliable clinical agents. D02-01 is a *runtime decision problem*—what the agent should do with an evolving belief state for one case. D02-04 is a *lifecycle measurement problem*—how an evaluator should discover and attribute regressions across system versions. They would collapse into one thesis only if D02-04 were reduced to evaluating D02-01.
- **D02-02 and D02-03** both use explicit machine-checkable structures. D02-02 learns and applies constraints to repair clinical representations. D02-03 checks whether a causal question is supported by a data-generating process and may refuse estimation. Their semantics, ground truth, experiments, and expertise needs differ substantially.

No candidate is merely an application variant of another. Cross-stream normalization may later choose to merge or split them, but this blind pass should preserve the distinctions.

### B. Qualitative comparison

This comparison is intentionally qualitative and does not apply the canonical weighted scoring framework.

| Dimension | D02-01: dual-clock control | D02-02: constraint repair | D02-03: causal data-fit contracts | D02-04: continual assurance |
|---|---|---|---|---|
| Scientific importance | Very high: unsafe longitudinal action and belief revision | High: invalid structured clinical representations contaminate downstream reasoning | Very high: invalid real-world evidence can create false causal conclusions | High: compound systems can regress silently across updates |
| Methodological depth | High if formulated as constrained sequential decision-making | High if constraint induction and repair are genuinely new | Very high: causal semantics, formal checking, selective automation | High if sequential design and attribution are rigorous |
| Preliminary novelty headroom | Medium; component fields are crowded | Medium-to-low until logic/repair collisions are searched | Medium-to-high for the narrow data-fit/refusal contract, despite automation collisions | Medium-to-low because DAS, DyReMe, CAT, and monitoring are close |
| Publication tractability | Medium; benchmark first, controller harder | Medium; benchmark/formalism first, core learning risky | Medium-to-high; formalism/benchmark and method decompose naturally | High for measurement, medium for core attribution method |
| Empirical feasibility | Medium; action labels and dual-time corpora are hard | Medium-to-low; natural violations, exceptions, and transfer labels are hard | Medium; simulation is strong, real EHR causal truth is hard | Medium-to-high with open versions and injected changes; prospective validation uncertain |
| Artifact/reuse potential | High: environment, state schema, controller interfaces | High: constraint language, corpus, solver | Very high: contract language, compiler, benchmark, reproducible workflows | Very high: versioned benchmark, test selector, assurance dossiers |
| Foundation-model resilience | High if representation/policy is model agnostic | Medium-to-high if formal verification is real; low for prompt critique | Very high: better models cannot manufacture identifiability | Very high: changing stronger systems still require assurance |
| Advisor/resource feasibility | Needs sequential decision/UQ plus clinical informatics | Needs neuro-symbolic/formal methods plus clinical NLP and experts | Needs genuine causal inference plus EHR/OMOP and formal specification | Needs evaluation/statistics/software reliability plus clinical safety |
| Transferable technical depth | Sequential decision-making, uncertainty, state estimation | Logic, constraint learning, program repair | Causal inference, formal specification, reproducible analytics | Sequential experimentation, monitoring, fault localization |
| Largest unresolved uncertainty | Whether a learnable multi-action policy beats simple rules with reliable labels | Whether learned “constraints” are valid and novel rather than site correlations | Whether meaningful validity conditions can be machine-checked without implying causal certification | Whether versioned attribution adds science beyond DAS plus standard regression testing |

### C. Missing-direction check

**Question:** What strong scientific direction might have been overlooked because of anchoring on historical repository discussions?

The most serious omitted direction is **adaptive human–AI epistemic team design**: learning when a clinical AI should expose uncertainty, solicit specific human expertise, or allocate decision authority, then measuring team—not model—performance. This could yield a thesis in human–AI delegation, information value, and cognitive forcing functions. It was not promoted to a fifth candidate today for three reasons: prospective human studies and IRB/participant access create a major feasibility dependency; ground truth for team utility is difficult; and the runtime allocation component partly overlaps D02-01. It deserves a Day 2 missing-neighbor check, especially if D02-01's labels prove infeasible.

Other plausible omitted families—privacy-preserving cross-institution learning, multimodal phenotyping, and causal representation learning—were not advanced because the first-pass search did not reveal a comparably precise, resource-feasible thesis that displaced one of the four above. This is not a rejection of those families.

### D. Intellectual-interest note

The user's interests in neuro-symbolic AI and artificial metacognition are treated as positive signals, not selection criteria:

- D02-02 earns its place only because executable constraint induction and repair could constitute a substantive methodological contribution; the neuro-symbolic label does not rescue it from severe novelty and epistemic-validity risk.
- D02-01 operationalizes a defensible form of artificial metacognition—selective action over an explicit belief state—without claiming consciousness or relying on self-reported confidence. It still advances only with major uncertainty.
- D02-03 currently receives the strongest Day 1 verdict despite being less directly aligned with those interests, because its causal thesis is unusually coherent, durable, and falsifiable.

## Day 1 freeze and handoff boundary

This artifact is frozen as Analysis Stream 02's blind first pass. It does not establish global novelty, a finalist set, or a canonical ranking. The next scientifically justified work would be separate Day 2 adversarial novelty testing of the exact proposed objects and dangerous neighbors identified above. No such testing, cross-stream comparison, candidate normalization, or repository-wide synthesis is included here.
