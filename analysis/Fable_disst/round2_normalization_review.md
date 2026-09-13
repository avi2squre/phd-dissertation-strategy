# Stream 03, Round 2: Independent Adversarial Review of the Cross-Stream Candidate Normalization

- **Date:** 2026-08-31
- **Analysis-stream identifier:** Analysis Stream 03
- **Repository base SHA (canonical Day 1 checkpoint):** `4deee8eb8425b22e9532f1f3afd74791ef3e422c`
- **Branch:** `analysis03/round2-normalization-review`
- **Status:** FROZEN — ROUND 2 INDEPENDENT NORMALIZATION REVIEW
- **Inputs used:** the three frozen Day 1 v2 artifacts (`analysis/analysis_01/day1_candidate_generation_v2.md`, `analysis/analysis_02/day1_candidate_generation_v2.md`, `analysis/analysis_03/day1_candidate_generation_v2.md`); `analysis/COMMON_ANALYSIS_SCHEMA.md`; `analysis/README.md`; `OPERATING_PROTOCOL.md`; the coordinator's Round 1 normalization hypothesis as supplied in the task.
- **Excluded inputs:** any Stream 02 Round 2 response, artifact, branch, or conclusion; external literature (no new searches or fetches were performed); `decisions/current_rankings.md` as an answer key.
- **Task scope:** scientific-identity normalization only. No ranking, no finalist selection, no verdict averaging, no new candidates, no Day 2 falsification.
- **Stopping condition:** matrix, audits, mandated attacks, missed-relationship sweep, independent normalized set, and disagreement ledger complete; further rereading of the same three artifacts judged unlikely to change any relationship judgment.

**Comparison standard applied.** Candidates were compared on central scientific object, central scientific problem, falsifiable thesis, methodological contribution, aims, evaluation strategy, and critical uncertainty, in that priority order. Titles and vocabulary were treated as weak evidence. SAME DIRECTION is asserted only where a merge preserves one central falsifiable thesis and one coherent dissertation architecture. Where this review quotes or characterizes another stream's candidate, the characterization comes from that stream's frozen v2 artifact and nothing else.

---

## A. Conceptual relationship matrix (12 x 12)

Row/column order: S01-C1, S01-C2, S01-C3, S01-C4, D02-01, D02-02, D02-03, D02-04, S03-C1, S03-C2, S03-C3, S03-C4.
Legend: **S** = SAME DIRECTION, **P** = PARTIAL OVERLAP, **D** = DISTINCT, x = self.

| | S01-C1 | S01-C2 | S01-C3 | S01-C4 | D02-01 | D02-02 | D02-03 | D02-04 | S03-C1 | S03-C2 | S03-C3 | S03-C4 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| **S01-C1** evidence-state control | x | D | D | D | **S** | D | D | D | D | D | **P** | D |
| **S01-C2** diagnostic-state reasoning | D | x | D | D | **P** | **P** | D | D | D | **S** | D | D |
| **S01-C3** data-fitness TTE | D | D | x | D | D | D | **S** | D | D | D | D | D |
| **S01-C4** failure localization | D | D | D | x | D | D | D | **P** | D | D | D | D |
| **D02-01** dual-clock control | **S** | **P** | D | D | x | D | D | D | **P** | **P** | **P** | D |
| **D02-02** constraint repair | D | **P** | D | D | D | x | D | D | D | D | D | D |
| **D02-03** causal contracts | D | D | **S** | D | D | D | x | D | D | D | D | D |
| **D02-04** continual assurance | D | D | D | **P** | D | D | D | x | D | D | D | D |
| **S03-C1** adequacy verification | D | D | D | D | **P** | D | D | D | x | D | **P** | D |
| **S03-C2** diagnostic trajectories | D | **S** | D | D | **P** | D | D | D | D | x | D | D |
| **S03-C3** selective control | **P** | D | D | D | **P** | D | D | D | **P** | D | x | D |
| **S03-C4** measurement error | D | D | D | D | D | D | D | D | D | D | D | x |

Three SAME pairs; eight PARTIAL pairs. Several DISTINCT pairs carry component-level interfaces documented in section D; the matrix reserves P for pairs where a merge is at least arguable at direction level.

---

## B. Audit of the coordinator's N1 to N7, with the mandated attacks

### N1: Evidence-State and Selective Control (S01-C1, D02-01, S03-C3)

**ROUND 1 VERDICT: SPLIT** (retain S01-C1 + D02-01 as one direction; demote S03-C3 to PARTIAL OVERLAP and dissolve it across the normalized set as described in E).

1. **Shared scientific identity.** All three place a selective multi-action policy (answer / retrieve / ask / defer, with variants) over an explicit representation of *why* the system should not yet commit, evaluated with risk- or cost-aware selective metrics against scalar-confidence baselines. The action-policy layer converges strongly across all three artifacts, including near-identical action vocabularies.

2. **Distinctions lost by a three-way merge.** S01-C1 contributes the typed uncertainty-cause state (missing, contradictory, unverifiable, tool failure, distributional mismatch). D02-01 contributes the dual-clock semantics (patient-event time versus evidence-validity time), claim-level provenance and supersession, and transition-level evaluation of belief maintenance (justified preservation, warranted revision). S03-C3 contributes three things the merged direction does not need and cannot cleanly test: (a) the claim that *task-structural* signals (retrieval-candidate agreement, ontology consistency, verification counts) dominate model-internal confidence *under site and language shift*; (b) the extraction-pipeline setting, where selective prediction operates over thousands of span-and-normalization micro-decisions per document rather than case-level agent turns; (c) statistical risk control (conformal guarantees) and workload-normalized evaluation.

3. **One falsifiable thesis?** For S01-C1 + D02-01: yes. Merged thesis: an explicit, typed, provenance-linked evidence state with separate patient-time and evidence-validity semantics, coupled to a cost-sensitive selective controller, reduces unsafe commitment and unsupported belief revision relative to scalar-uncertainty, simple-policy, and generic orchestration baselines in longitudinal clinical tasks, at matched action cost. Both original theses are instances of this claim, and both fail under the same falsification (simple policies matching the explicit state). For the three-way merge: no. S03-C3's first clause is a claim about the *source* of failure-predictive signal, testable with no belief state and no agent, on different data with different metrics. Encompassing it forces either a second thesis or the deletion of S03-C3's identity.

4. **One coherent aim structure?** For the pair: yes; the Aim 1 / Aim 2 / Aim 3 structures of S01-C1 and D02-01 align nearly one-to-one (represent and measure; learn control; transfer), and D02-01's environment design (versioned evidence, counterfactual clock pairs) is the stronger instantiation of the shared Aim 1. For the trio: no; S03-C3's aims interleave extraction-pipeline instrumentation and shift studies that do not test the belief-state thesis.

5. **Recommended normalized formulation.** *Evidence-state selective control for longitudinal clinical agents*: typed, provenance-linked, dual-clock evidence state plus cost-sensitive multi-action controller plus transition-level selective evaluation (members: S01-C1, D02-01). S03-C3's controller and workload-normalized evaluation fold in as variant machinery; its structural-signals-under-shift hypothesis is preserved *by name* inside the normalized direction's signal-source aim, and its verification-derived signal idea is recorded as the interface to N6 (see D and E).

6. **Confidence: MODERATE.** The pairwise merge is clean (HIGH); the demotion of S03-C3 rests on a judgment that its shift-dominance clause is thesis-defining rather than incidental, which a Day 2 pilot could revisit.

**Mandated attack (should representation and control remain one direction?).** Within the merged pair, yes: the state is proposed *as the sufficient statistic for control*, so the representation claim and the control claim are jointly falsified or jointly supported; separating them would produce a representation with no behavioral test and a controller with no explanatory variable. What should *not* remain inside N1 is the risk-control machinery as an identity: conformal selective guarantees (S03-C3) are portable mathematics, not a direction, and treating them as N1 membership glue overstates convergence.

### N2: Longitudinal Diagnostic-State Trajectory Modeling (S01-C2, S03-C2)

**ROUND 1 VERDICT: ACCEPT** (with a strengthened formulation).

1. **Shared identity.** Both make the patient-level diagnostic state and its transitions the first-class scientific object; both reject endpoint-only evaluation for evidence-horizon evaluation; both propose state ontologies covering suspected / provisional / confirmed / ruled-out / historical; both propose transition-aware metrics and a benchmark; both identify mention-level assertion work as the solved foundation being exceeded.

2. **Distinctions lost by merging.** S01-C2's normative framing (was this transition *justified by the evidence available at that time*), its symbolic transition-constraint machinery, and its trajectory-consistency objective. S03-C2's resolving-event anchoring (genetic testing as natural labels), its annotation scheme and inter-annotator program, and its cohort-ground-truth application with clinician-adjudication fidelity as the decisive clinical test. A careless merge would collapse these into "temporal diagnosis modeling."

3. **One falsifiable thesis?** Yes: diagnostic state and its transitions, represented explicitly, are recoverable from longitudinal records more faithfully than snapshot extraction plus aggregation or unconstrained generation, with fidelity sufficient for a downstream clinical use with independent ground truth. S01-C2's constraint claim and S03-C2's representation claim are competing *mechanisms* inside this thesis, which is precisely what a healthy Aim 2 tests head-to-head rather than a sign of two theses.

4. **One coherent aim structure?** Yes: formalize and annotate (union of both Aim 1s, with S03-C2's agreement program and S01-C2's justified-at-time labels); model (state-carrying readers versus constraint-governed inference versus aggregation and long-context baselines); validate (S03-C2's adjudication-fidelity study plus S01-C2's cross-condition transfer).

5. **Recommended normalized formulation.** *Diagnostic-state trajectories from longitudinal clinical records*: a trajectory representation with resolving events and temporal transition constraints, an annotated benchmark with evidence-horizon and transition-aware metrics, competing trajectory-inference mechanisms, and validation against expert adjudication in a setting where structured data provably cannot resolve status.

6. **Confidence: HIGH.**

### N3: Data-Fitness-Aware Autonomous Target-Trial Emulation (S01-C3, D02-03)

**ROUND 1 VERDICT: ACCEPT.**

1. **Shared identity.** Identical scientific object at two levels of formalization: an explicit, machine-evaluable mapping from a target-trial estimand to what a specific EHR data-generating process can support, with revision/restriction and refusal as first-class outputs and an audit trail. Both theses have the same falsification: deterministic checklists performing equally kills both.

2. **Distinctions lost by merging.** D02-03's sharper semantics: the typed contract language and compiler, the four-valued decision output (supported / restricted estimand / requires information / not supported), and the explicit separation "an LLM may translate prose into the contract, but a deterministic engine must evaluate it." S01-C3's agentic revision framing and audit-trace emphasis. These are formalization-depth differences, not thesis differences.

3. **One falsifiable thesis?** Yes, essentially verbatim shared already.

4. **One coherent aim structure?** Yes; the two artifacts' aims align one-to-one (formalize and benchmark; checker/completion with calibrated decisions; multi-system validation).

5. **Recommended normalized formulation.** Adopt D02-03's contract-and-compiler semantics with the four-valued decision layer as the normalized object, retaining S01-C3's audit-trace and revision-policy vocabulary; title on the pattern *machine-checkable causal data-fit contracts for EHR target-trial emulation*.

6. **Confidence: HIGH.**

### N4: Dynamic Continual Assurance and Failure Attribution (S01-C4, D02-04)

**ROUND 1 VERDICT: SPLIT** (same research family, two directions), with a conditional REDEFINE option stated below.

1. **Shared identity.** Both are assurance-by-attribution: both build failure ontologies, both use paired or counterfactual designs, both target the inadequacy of endpoint scores, both name the same dangerous prior art cluster (dynamic red-teaming; process-aware benchmarks), and both produce reusable assurance artifacts.

2. **Distinctions lost by merging.** The unit of intervention. S01-C4 attributes failure to a *step within one trajectory* (critical-step localization, counterfactual step replay across stochastic reruns, targeted intervention at the step level). D02-04 attributes regression to a *changed component across system versions* (paired tests over model / corpus / tool / prompt / policy factors, budgeted sequential test selection, false-alarm control, failure lineage). Their baselines differ (trajectory-diagnosis systems versus adaptive testing, regression suites, and monitoring), their ground truths differ (clinician-adjudicated critical steps versus injected component changes), and their statistical machinery differs (replay variance versus sequential detection with alpha spending).

3. **One falsifiable thesis?** Not as proposed. "Process-aware evaluation with failure localization beats endpoint benchmarks" and "versioned attribution with budgeted selection beats static and undirected dynamic testing" are two theses; a dissertation containing both untransformed is the prohibited pattern of adjacent fashionable projects. **Mandated attack answered directly: they should not remain one direction at the direction level.**

4. **One coherent aim structure?** Only under a genuine reformulation. There is a candidate unifying object visible in the two artifacts' own machinery: both perform *counterfactual attribution over an explicit execution structure*, S01-C4 intervening on trajectory steps, D02-04 intervening on version components. A single formalism treating {component version} x {trajectory step} as the intervention set, with one attribution estimator and one budget-aware test-selection layer, would support one thesis ("counterfactual attribution over an explicit execution-and-version structure localizes causes of clinical-agent failure better than endpoint scoring, LLM judging, and undirected stress testing, at fixed budget"). Neither artifact states this unification; adopting it is a REDEFINE decision that should be made only if Day 2 confirms the shared machinery is real rather than verbal.

5. **Recommended normalized formulation.** Two directions in one family: *process-level failure attribution for clinical agent trajectories* (S01-C4) and *change-attributed continual assurance for compound clinical AI systems* (D02-04); optionally REDEFINE into *counterfactual failure attribution across execution steps and system versions* if and only if the unified intervention formalism survives Day 2 scrutiny.

6. **Confidence: MODERATE.** The split is well supported by the artifacts; the conditional unification is a genuine possibility that prevents overconfidence in the split.

### N5: Learned Temporal Clinical Constraints and Auditable Representation Repair (D02-02)

**ROUND 1 VERDICT: ACCEPT** (distinct), with one missed relationship recorded.

1. **Shared identity with others:** none at thesis level. Its object (probabilistic constraint induction with applicability scopes plus proof-carrying minimal repair) and its ground truth (semantic repair fidelity, false-correction rate) belong to representation validity, not diagnostic reasoning, agent control, or evaluation science.
2. **Distinctions preserved:** the epistemic core (learned regularity versus valid clinical rule) is unique in the portfolio.
3. **One thesis with any neighbor?** No. Its nearest neighbor is S01-C2 (see D): S01-C2's "temporal transition model: rules or learned constraints governing allowable state changes" is a special case of D02-02's constraint language applied to the diagnostic-state layer, but the two theses answer different questions (do learned constraints transfer and repair safely, versus does trajectory structure improve diagnostic fidelity), with different falsifications.
4. **Aim structure:** self-contained.
5. **Recommended formulation:** unchanged from D02-02, with an explicit interface note: its induced constraint classes are a candidate supplier of N2's transition model.
6. **Confidence: HIGH** for distinctness; the interface note is MODERATE.

### N6: Adequacy-Aware Clinical Evidence Verification (S03-C1)

**ROUND 1 VERDICT: ACCEPT** (distinct, adjacent to N1), with the adjacency sharpened.

**Mandated attack (separate direction or upstream component of N1?).** Separate direction. The component relationship is real: a per-dimension verifier's verdicts are a natural field of N1's evidence state, exactly as the coordinator's note suggests. But componenthood does not collapse identity: S03-C1's thesis (adequacy and currency violations exist at rates invisible to entailment-only checking, and enforcing per-dimension verification changes system reliability rankings) is fully testable with no agent, no belief state, and no action policy, on static claim-evidence pairs with expert labels; N1's thesis is not tested by any of that. Two dissertations could proceed in parallel with zero shared falsification. Merging S03-C1 into N1 would reduce a verification calculus with its own benchmark and calibration program to a feature-engineering aim inside a control thesis, discarding most of its scientific content. The audit standard (one thesis, one architecture) fails for the merge; DISTINCT stands.

**Sharpened adjacency the proposal does not record:** D02-01's evidence-validity clock and S03-C1's currency dimension are the same underlying semantics (evidence expires; supersession relations) used for different purposes (timing beliefs versus judging claims). A shared temporal-validity formalism and a shared versioned-evidence corpus would serve both directions; this is a resource-and-formalism interface, not a merge argument.

**Confidence: HIGH.**

### N7: Measurement-Error-Aware Clinical NLP Evaluation (S03-C4)

**ROUND 1 VERDICT: ACCEPT** (distinct), with two missed relationships recorded.

1. Its object is the evaluation instrument itself; no other candidate's thesis concerns instrument error.
2. **Missed relationship (a): N7 as the portfolio's instrument layer.** N2's transition-aware metrics require exactly the hierarchical partial-credit and agreement machinery N7 builds; N4's regression detection (both halves) explicitly lists adjudicator uncertainty, judge drift, and label stochasticity in its own evaluation strategies, which is N7's subject matter as a component. These are producer-consumer interfaces, not merges.
3. **Missed relationship (b): N6 and N7** share expert-adjudication methodology (per-dimension labels, disagreement adjudication) at the protocol level only; the theses are unrelated.
4. **Confidence: HIGH.**

---

## C. Mandated attacks: summary of answers

- **N1:** representation and selective control remain one direction for S01-C1 + D02-01, because the state is the sufficient statistic the control thesis tests; S03-C3 does not belong as a full member, because its shift-dominance clause and extraction setting constitute a second thesis. SPLIT.
- **N4:** step-level attribution and version-level attribution are two theses with different intervention units, baselines, and statistics; keep as two directions in one family, with a conditional unified-formalism REDEFINE that only Day 2 evidence should trigger. SPLIT.
- **N6:** a separate direction with a real upstream interface to N1; merging would discard most of its scientific content. ACCEPT as DISTINCT.

## D. Missed or under-recorded relationships (beyond the audit notes above)

1. **N2 and N5 (S01-C2 and D02-02): PARTIAL at machinery level.** Constraint induction with applicability scopes could supply N2's transition model; Day 2 novelty searches for "temporal constraints over clinical structure" should be coordinated so the two directions do not duplicate or contradict each other's prior-art conclusions.
2. **N1 and N2 (D02-01 as the bridge candidate).** D02-01's belief-state maintenance over a longitudinal case sits between the two normalized directions: its transition-level evaluation of *agent beliefs* (justified preservation, warranted revision) is structurally N2's transition-fidelity evaluation applied to a different object (the agent's state rather than the record's state). Primary membership in N1 is correct because its thesis is control-centric; the affinity should be recorded because a Day 2 falsification of N2's representation claim would partly implicate D02-01's state semantics as well.
3. **N1 and N6 (temporal-validity semantics).** As in the N6 audit: one shared formalism (evidence-validity intervals, supersession) serves both; building it twice would be waste, and building it inconsistently would create false disagreement between streams.
4. **N4 and N7 (instrument error inside regression monitoring).** Change-attribution under noisy judges is partly a measurement-error problem; N7's decomposition machinery is the principled version of the adjudication-uncertainty handling N4 already lists.
5. **A recurring architecture worth naming without merging.** N1 (clinical beliefs), N3 (causal designs), and N6 (evidence adequacy) are three instantiations of one abstract pattern: represent validity explicitly in a typed structure, then act selectively on it, with refusal as a first-class output. This is a portfolio-level observation for the cross-review record. It must not be promoted to a merged umbrella direction; doing so would create exactly the fashionable-projects aggregation this review is required to reject.

## E. Independently recommended normalized candidate set

Eight normalized directions. Seven was not forced; neither was eight sought.

| ID | Normalized title | Constituents | Central scientific object | One-sentence scientific boundary |
|---|---|---|---|---|
| R1 | Evidence-state selective control for longitudinal clinical agents | S01-C1 + D02-01 (S03-C3's controller and workload-normalized evaluation folded in as variant machinery; its structural-signals-under-shift hypothesis preserved by name inside the signal-source aim) | Typed, provenance-linked, dual-clock evidence state; cost-sensitive multi-action controller; transition-level selective evaluation | Studies what an agent should do next given an explicit representation of its evidentiary situation; excludes judging evidence quality (R5) and excludes the evaluation instrument itself (R8) |
| R2 | Diagnostic-state trajectories from longitudinal clinical records | S01-C2 + S03-C2 | Trajectory representation with resolving events; temporal transition constraints; transition-aware metrics and benchmark; adjudication-fidelity validation | Studies what the record establishes about a patient's diagnostic state over time; excludes agent action policies (R1) |
| R3 | Machine-checkable causal data-fit contracts for EHR target-trial emulation | S01-C3 + D02-03 | Contract language and deterministic compiler mapping estimands to data support, with restricted-estimand and refusal outputs and audit traces | Studies whether a causal question is answerable from a given data-generating process; excludes generic agentic automation of analyses |
| R4a | Process-level failure attribution for clinical agent trajectories | S01-C4 | Failure ontology; critical-step localizer; counterfactual step replay; targeted intervention | Attributes one execution's failure to a step within it; excludes cross-version change attribution (R4b) |
| R4b | Change-attributed continual assurance for compound clinical AI systems | D02-04 | Versioned failure-surface model; paired component perturbation; budgeted sequential regression discovery | Attributes new failures to changed system components across versions; excludes within-trajectory step diagnosis (R4a). R4a/R4b form one family; a unified counterfactual-attribution formalism is a conditional Day 2 REDEFINE option |
| R5 | Adequacy-aware clinical evidence verification | S03-C1 | Per-dimension claim-evidence verification calculus (support, adequacy, currency, applicability); expert-annotated benchmark; calibrated verifier | Studies whether a clinical claim's evidence is good enough and still valid; upstream interface to R1's evidence state, not a component of it |
| R6 | Learned temporal clinical constraints and auditable representation repair | D02-02 | Probabilistic constraint induction with applicability scopes; proof-carrying minimal repair | Studies which constraints should govern clinical representations and how to repair violations safely; machinery interface to R2's transition model |
| R7 | Measurement-error-aware clinical NLP evaluation | S03-C4 | Error decomposition of the evaluation instrument; noise-aware ranking inference; validated corrected protocols | Studies the ruler, not the systems; serves R1/R2/R4 evaluation as an instrument layer without sharing their theses |

(Numbering note: R7 is listed eighth because R4 splits into R4a/R4b; the set contains eight directions across seven families.)

S03-C3 is the one Day 1 candidate that does not survive as an independent normalized direction: its content distributes into R1 (control layer, workload-normalized evaluation, the named shift-dominance hypothesis) and R5 (verification-derived failure signals), consistent with Stream 03's own frozen Day 1 diversity check, which recommended against carrying S03-C1 and S03-C3 forward separately.

## F. Disagreement ledger against the coordinator proposal

| # | Coordinator judgment | Stream 03 judgment | Exact reason | Consequence |
|---|---|---|---|---|
| 1 | N1 = strong convergence of three members | SPLIT: S01-C1 + D02-01 are SAME DIRECTION; S03-C3 is PARTIAL OVERLAP and dissolves into R1 + R5 | S03-C3's thesis-defining clause (task-structural signals dominate model-internal confidence under shift, in extraction pipelines, with statistical risk control) cannot be tested inside a belief-state control architecture without becoming a second thesis | N1's Day 2 novelty attack targets belief-state/POMDP/decision-theoretic prior art; the shift-dominance hypothesis is attacked separately against its own dangerous prior art; no aim in R1 inherits S03-C3's extraction setting silently |
| 2 | N4 = same direction at dissertation-family level | SPLIT into R4a and R4b (same family, two directions), conditional REDEFINE if a unified counterfactual-attribution formalism survives Day 2 | Two intervention units (trajectory step versus version component), two theses, disjoint baselines and statistics; a merged candidate would place two fashionable assurance projects beside one another | Prevents a normalized candidate that fails the one-thesis test on arrival; preserves the genuine unification as an explicit, evidence-gated option rather than an assumption |
| 3 | N5 = DISTINCT, no relationships noted | ACCEPT distinctness; add PARTIAL machinery relationship N5-N2 | S01-C2's transition model ("rules or learned constraints governing allowable state changes") is a special case of D02-02's constraint language | Coordinated Day 2 prior-art searches; interface named in both candidate definitions to avoid duplicated or contradictory novelty conclusions |
| 4 | N6 = distinct but adjacent to N1 via verifier-to-signal flow | ACCEPT, and add the shared temporal-validity semantics (D02-01's evidence-validity clock = S03-C1's currency axis) | The adjacency is deeper than signal flow: one formalism and one versioned-evidence corpus serve both | Shared-resource planning; prevents two streams building inconsistent supersession semantics that would later read as scientific disagreement when it is only engineering divergence |
| 5 | N7 = DISTINCT, no relationships noted | ACCEPT distinctness; add N7-N4 and N7-N2 instrument interfaces | N4's own evaluation strategies list adjudication uncertainty and judge drift, which are N7's subject matter; N2's transition metrics need N7's partial-credit machinery | N7 is recognized as the portfolio's instrument layer; its Day 2 scope-sizing question gains a concrete internal customer, without any merge |
| 6 | Seven-family structure | Eight directions across seven families | Consequence of ledger rows 1 and 2: N4 splits; N1 loses a member without losing content | The normalized set records where each Day 1 candidate's content went; no content is silently dropped, and no candidate was added |

## G. Umbrella-merge rejection statement

This review explicitly rejects, as violations of the one-thesis standard: any three-way merge of S01-C1 + D02-01 + S03-C3 that keeps S03-C3's extraction-and-shift clause; any merge of S01-C4 + D02-04 performed without the unified intervention formalism; any merge of S03-C1 into N1; and any future aggregation of N1 + N3 + N6 under a "typed validity state plus selective action" umbrella, which names a recurring architecture, not a dissertation. Each rejected merge would produce several attractive projects placed beside one another rather than different tests of one falsifiable dissertation thesis.

---

**STATUS: FROZEN — ROUND 2 INDEPENDENT NORMALIZATION REVIEW (2026-08-31). Produced without reading any other stream's Round 2 output. Later reconciliation with the coordinator and other streams belongs to the next stage, not to edits of this file.**
