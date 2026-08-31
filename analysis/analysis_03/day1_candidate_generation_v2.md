# Stream 03, Day 1: Candidate Dissertation Research Directions (Common Analysis Schema v2)

**FORMAT-NORMALIZED DERIVATIVE OF FROZEN BLIND FIRST PASS.**
**NO NEW SCIENTIFIC ANALYSIS PERFORMED.**

- **Original frozen artifact:** `analysis/analysis_03/day1_candidate_generation.md` (authoritative blind-first-pass scientific provenance; scientific content unchanged, metadata corrected on 2026-08-31).
- **Provenance chain (this branch, in order):**
  1. Original scientific freeze commit: `ec538e98fa0e1e2680a18d4bd5100c5f6141a6e6`
  2. Format-normalization commit (this derivative): `6d0ea960b1699756f4d2b673d1514fa66e51a541`
  3. Metadata-only provenance correction commit: `0c7d2f6ac1365a1755da765cf5c118b218baf428`
  4. Final provenance clarification: this commit (wording only).
- **Repository base SHA of the frozen analysis:** `86230f478b0a47a0198adbe325c42b0561fe8288`.
- **Derivation rule compliance:** sections 2, 21, and 22 of each candidate, and the matrix rows "falsifiability / discriminating experiment" and "time to uncertainty resolution," are populated only by extracting or faithfully compressing reasoning already present in the frozen artifact. No field required the marker NOT PRESENT IN ORIGINAL FROZEN ARTIFACT.

---

# Layer I — Executive navigation

## A. Analysis metadata

- **Date:** 2026-08-31 (frozen analysis); this derivative produced later the same day, 2026-08-31, with no content change.
- **METADATA-ONLY PROVENANCE CORRECTION (2026-08-31):** the frozen-analysis date and the advisor-profile fetch date were initially misrecorded as 2026-08-30 in both the frozen artifact and this derivative; corrected to 2026-08-31 per deterministic git and filesystem evidence (branch created 2026-08-31 14:39 US Central; freeze commit ec538e9 at 14:57; derivative commit 6d0ea96 at 16:02, all the same day). No candidate identity, scientific object, thesis, evidence interpretation, source, aim, advisor judgment, verdict, critical uncertainty, portfolio conclusion, or scientific reasoning changed.
- **Analysis-stream identifier:** Analysis Stream 03.
- **Repository SHA used:** `86230f478b0a47a0198adbe325c42b0561fe8288`.
- **Analysis status:** FROZEN — BLIND FIRST PASS (scientific content immutable; this file is a format normalization only).
- **Permitted repository inputs used:** `README.md`; `OPERATING_PROTOCOL.md`; `decisions/` (DEC-001 to DEC-008); `context/` files; structural READMEs; `literature/index.md` (ID/citation/identifier columns only) and Stream 03-authored records; Stream 03's own provenance (`discussions/discussion_03/`); public scientific literature independently retrieved for the task.
- **Deliberately excluded inputs:** `discussions/discussion_01/` and `discussions/discussion_02/` contents; literature records authored by other streams (LIT-024 to LIT-032 records); `candidate_programs/` file contents; `decisions/current_rankings.md` as an answer key; raw historical chat exports.
- **External-search scope:** four parallel retrieval agents (one per candidate area), roughly 38 distinct queries; primary pages fetched on arXiv, ACL Anthology, publisher DOI pages, PMC, and NCBI eutils. Source characterizations are abstract-level or page-level reads; full-text verification belongs to Days 2 to 3. Sources not in `literature/index.md` are cited inline with identifiers; registration deferred per the Day 1 write policy.
- **Independence disclosures (from the frozen artifact):** (1) while syncing, this analyst unavoidably saw the file names (not contents) of other streams' newly landed provenance; (2) from the shared index, only ID/citation/identifier columns were extracted for LIT-ID reuse; interpretive columns and other streams' records were not read; (3) during earlier provenance-reconstruction work (2026-08-28 to 08-30), this analyst was exposed to fragments of a later independent stream's critique of a Stream 03 proposal; none of its conclusions, citations, or interpretations were used as inputs, and all prior-art claims are grounded in sources retrieved independently on Day 1 or in Stream 03's archived provenance.
- **Advisor clarification (v1.1):** received before freezing and incorporated into each candidate's advisor section: named UMN IHI primary-advisor matches with Dr. Rui Zhang as external/complementary advisor, grounded in official institute profile pages fetched 2026-08-31 (staff pages for Melton-Meaux, Aliferis, Kummerfeld, Simon, Pakhomov); the full directory page returned 404 twice, so faculty coverage may be incomplete. All fit statements are inferences from public research descriptions; no willingness, availability, funding, or commitment is inferred.
- **Parallelism justification:** the four retrieval targets are scientifically disjoint; merging any two would halve dangerous-prior-art search depth in that area with no methodological benefit; only retrieval was delegated, and all scientific reasoning remained in one process.
- **Stopping condition:** reproduced as Layer III.E.

## B. Repository-convention declarations

1. **Question evaluated:** which 3 to 4 candidate dissertation research directions independently appear strongest now, specified deeply enough for Day 2 adversarial falsification.
2. **Evidence used:** canonical repository files; Stream 03's archived provenance; primary pages of independently retrieved 2024 to 2026 literature plus seminal anchors (identifiers inline).
3. **Key assumptions:** abstract-level and page-level source reads are treated as faithful pending full-text verification; Stream 03's archived provenance is treated as accurate as archived; the funded project's documented task assignments are treated as feasibility context only.
4. **Recommendation and uncertainty status:** four candidates specified; two ADVANCE, two ADVANCE WITH MAJOR UNCERTAINTY; per-candidate critical uncertainties named (section 22 of each).
5. **Other analyses consulted:** none; this is a blind first pass (see independence disclosures).
6. **Accepted decisions challenged or reconsidered:** none.

## C. Candidate overview table

This table is a map, not an ordinal ranking.

| ID | Candidate dissertation direction | Central scientific object | Day 1 verdict | Critical uncertainty / rejection trigger |
|---|---|---|---|---|
| C1 | Adequacy-aware verification of clinical AI claims | A claim-level verification formalism (support, adequacy, currency, patient applicability) with an expert-annotated benchmark and a calibrated verifier | ADVANCE | Whether LINS-class or commercial systems already implement per-claim adequacy/currency verification |
| C2 | Diagnostic-state trajectories from longitudinal clinical records | A patient-level state representation (states, transitions, resolving events) with an annotation scheme, transition-aware metrics, and a benchmark | ADVANCE | Whether clinician-adjudication access materializes for the decisive validation aim (and whether a trajectory formalism already exists) |
| C3 | Selective control for clinical language systems under asymmetric risk | Task-structural failure-prediction signals plus a cost-sensitive multi-action controller with risk control, and an evaluation methodology for selective behavior on extraction | ADVANCE WITH MAJOR UNCERTAINTY | Whether frontier self-verification matches structural signals under shift (MedAbstain and MedVAL full texts are the named targets) |
| C4 | Measurement error in clinical NLP evaluation | A measurement-error model of the evaluation instrument (artifact decomposition, noise-aware ranking inference, validated corrected protocols) | ADVANCE WITH MAJOR UNCERTAINTY | Whether artifact fractions are large enough to change conclusions, and whether the scope is dissertation-sized (cheap Aim 1 pilot resolves) |

---

# Layer II — Full candidate analysis

# Candidate C1: Adequacy-aware verification of clinical AI claims

### 1. Candidate identity

**Title:** Adequacy-aware claim verification: is this clinical claim supported by evidence that is methodologically adequate, still current, and applicable to this patient?

**One-sentence identity:** This direction studies verification of individual claims in clinical AI output along four separable dimensions (evidential support, methodological adequacy of the evidence, temporal currency of the evidence, and patient applicability), contributing the verification formalism, an expert-annotated benchmark, and a calibrated verifier, and measuring what each dimension buys over entailment-only support checking.

### 2. Central scientific object

A verification mechanism and evaluation instrument: a typed claim-evidence relation schema with quality and temporal-validity dimensions and composition rules; an expert-annotated per-dimension benchmark; a calibrated agentic verifier; and an evaluation methodology for verifiers themselves. (Extracted from the frozen artifact's section 8.)

### 3. Central scientific problem

Current attribution methods for generated medical text check whether a cited source *supports* a claim. Clinical epistemology requires more: evidence has a quality hierarchy (a case report is not a trial), evidence expires (guidelines are superseded; papers are retracted), and evidence is conditional on patient context. A claim can pass entailment-based citation checking while resting on retracted, superseded, methodologically weak, or inapplicable evidence. If clinical AI systems are to be audited rather than trusted, the verification layer must model these dimensions explicitly. The problem matters because unsupported and mis-supported output is prevalent at scale (section 5) and because human oversight demonstrably fails to catch machine errors (automation-bias evidence under C3).

### 4. Falsifiable dissertation thesis

**Proposed research hypothesis:** *A verifier that explicitly models evidence adequacy and currency detects clinically significant mis-supported claims that entailment-only support checking systematically misses, at rates high enough to change the measured reliability ranking of clinical QA/generation systems; and enforcing adequacy-aware verification at inference time improves clinically weighted reliability at acceptable coverage cost.*

Falsification conditions: if, on an expert-annotated benchmark, adequacy and currency violations are rare once entailment-support passes; or if entailment-only verifiers capture them incidentally; or if enforcing the verifier degrades coverage without reliability gain, the thesis fails. Coherence test: the aims are three tests of this one thesis (measure the phenomenon; build the mechanism; measure what enforcement buys), not adjacent projects.

### 5. Evidentiary basis

- **Claim:** LLM medical output is frequently unsupported by its own citations. → SourceCheckup, Wu et al. 2025, Nature Communications, DOI 10.1038/s41467-025-58551-6 (50 to 90 percent of LLM responses not fully supported across ~58,000 statement-source pairs). → *Source-supported finding (abstract-level read).*
- **Claim:** parametric model knowledge cannot handle retraction status. → Thelwall 2026, arXiv:2604.16872 (failure to recognize retracted articles 82 to 88 percent of the time). → *Source-supported finding.*
- **Claim:** models are weakest exactly where evidence synthesis and quality reasoning matter. → Wang and Chen 2026, Patterns, DOI 10.1016/j.patter.2026.101519 (about 90 percent on structured guidelines versus 50 to 60 percent on systematic reviews; confident answers when evidence is absent). → *Source-supported finding.*
- **Claim:** verification against an independent structured source measurably improves reliability, and supplying provenance eliminates identifier fabrication. → LIT-001 (about nine points from its Review step) and LIT-002 (100 percent versus 15.3 percent citation relevance), both READ in this stream. → *Source-supported findings (full-text reads archived in this stream's provenance).*
- **Claim:** support, adequacy, and currency are separable failure axes; systems covering one do not thereby cover the others. → *Cross-paper inference* from the observed division of labor: support checking (SourceCheckup; MedCite, LIT-024; ALCE, DOI 10.18653/v1/2023.emnlp-main.398), risk-of-bias automation as systematic-review tooling (ROBoto2, arXiv:2511.03048), retraction detection standalone (Pub-Guard-LLM, arXiv:2502.15429).
- Stream 03's archived two-paper synthesis (verify-after versus supply-before; supplying identifiers eliminates fabrication but not misattribution) supplies the architectural motivation. → *Cross-paper inference, archived 2026-08-28.*

### 6. Closest and dangerous prior work

- **MedCite** (LIT-024; ACL 2025.findings-acl.967): end-to-end citation generation and evaluation for medical tasks; support dimension only, per its page.
- **SourceCheckup** (DOI 10.1038/s41467-025-58551-6): automated claim-level support checking at scale, physician-validated.
- **ALCE** (2023.emnlp-main.398): the general-domain citation-quality metric frame.
- **DeepSciVerify** (arXiv:2605.27710): claim-citation alignment with evidence escalation; no currency dimension per abstract.
- **Dangerous prior art:** **LINS** (LIT-025; DOI 10.1038/s41467-025-64142-2), an end-to-end medical QA framework claiming evidence-traceable responses and explicitly claiming to address outdated knowledge and evidence validity; **Answered with Evidence** (arXiv:2507.02975), coupling generation with evidence-foundedness scoring; commercial evidence-grounded clinical QA products (surfaced, not fetched; a Day 2 obligation); **ROBoto2** (arXiv:2511.03048) for the adequacy component; **Pub-Guard-LLM** for the currency component; **αNeSy-CTM** (arXiv:2606.20895) for logic-based patient-applicability checking in trial matching.

### 7. Evidence-supported limitations of existing approaches

- Reported by sources: SourceCheckup notes pipeline error accumulation and 1-to-1 statement-source mapping limits; ALCE reports even best models lack complete support half the time on one dataset; Wang and Chen report confident-but-wrong behavior under absent evidence; Thelwall reports failure on retractions.
- **Inferred by this stream:** no surfaced system scores the *adequacy* of supporting evidence (study design, risk of bias) or its *currency* (supersession, retraction) as part of verifying generated claims; RoB automation exists only as systematic-review tooling on source papers, not as a verification dimension over generated text. LINS claims currency handling at the system level but its page describes no study-quality appraisal and no claim-level verification calculus. This inference is exactly what Day 2 must attack.

### 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION.** What appears unresolved: a claim-level verification formalism and expert-annotated benchmark in which each clinical claim-evidence pair is judged on support, adequacy, currency, and patient applicability as separable dimensions; a verifier that produces calibrated per-dimension verdicts; and empirical characterization of how frontier systems fail per dimension. Day 1 searches found the components separately but no unified treatment; the guideline-supersession component specifically returned no dedicated system (scout coverage note). Stated as "not surfaced in one day of targeted search," not as "no prior work exists."

### 9. Proposed methodological contribution

(a) A **verification formalism**: a typed claim-evidence relation schema with quality and temporal-validity dimensions and composition rules (when do two weak sources outweigh one strong outdated one), a genuine methodological object rather than an integration, because the composition and calibration questions have no existing answer; (b) an **expert-annotated benchmark** of clinical claim-evidence pairs labeled per dimension; (c) a **calibrated agentic verifier** (retrieve, appraise, date-check, judge) with per-dimension confidence; (d) an **evaluation methodology** for verifiers themselves (per-dimension error costs; detection of planted superseded-evidence citations). The symbolic half (evidence hierarchies, ontologies, temporal validity rules) makes this a concrete neuro-symbolic instance under the current medical NeSy framing (LIT-027, DOI 10.1038/s41551-026-01728-1) without using the umbrella as the topic.

### 10. Coherent dissertation aims

- **Aim 1 (measure).** Question: how often and where do frontier systems produce claims failing each dimension? → Method: build the schema and benchmark (public sources: guidelines with version histories, Cochrane reviews, retraction records); expert annotation. → Experiment: audit frontier and open systems. → Expected evidence: per-dimension failure rates; the adequacy/currency failure mass invisible to entailment-only checking (tests thesis clause 1).
- **Aim 2 (mechanism).** Question: can a verifier recover these failures with calibrated confidence? → Method: agentic verifier with per-dimension heads; appraisal via RoB-style signals; currency via versioned guideline and retraction lookups. → Experiment: against entailment-only and LLM-judge baselines, plus perturbation sets (planted superseded citations). → Expected evidence: detection gains attributable to the adequacy and currency machinery (ablations).
- **Aim 3 (consequence).** Question: what does enforcement buy downstream? → Method: gate a QA/generation system on the verifier; measure clinically weighted reliability versus coverage; rare-disease phenotyping instantiation connecting to the funded project's Aim 1 setting. → Expected evidence: risk-coverage improvement over confidence gating (tests thesis clause 2).

### 11. Publication decomposition

Benchmark and audit paper (Aim 1) → verifier method paper with ablations (Aim 2) → enforcement and clinical-instantiation paper (Aim 3), plus a plausible early resource note on the versioned-guideline corpus. If Aim 3 fails (enforcement buys little), Aims 1 and 2 still stand as a defensible dissertation on measurement plus mechanism with reusable artifacts (benchmark, verifier). No inflation: three core units.

### 12. Evaluation strategy

Datasets: constructed benchmark from public literature with version histories (Cochrane, guideline archives, PubMed retraction records; SourceCheckup-style question generation for coverage); existing attribution sets for comparability (ALCE-style metrics as baselines). Baselines: entailment-only citation checking (ALCE metrics, DeepSciVerify-style verifier), LLM-as-judge, frontier self-verification. Ablations: remove adequacy head; remove currency lookups; remove escalation. Metrics: per-dimension precision/recall against expert labels; calibration (ECE, selective risk); downstream risk-coverage curves. Robustness: temporal split (evidence published after model cutoff), planted-perturbation sets, specialty shift. Statistics: paired bootstrap over claims; annotator agreement with hierarchical/partial-credit handling. Human evaluation: expert adjudication on a stratified subsample and on disagreements.

### 13. Required resources and feasibility

Known available: public literature, guideline version archives, retraction records; this stream's archived close readings of LIT-001/002/004; local GPU access for open models (institutional cluster; archived provenance). Plausibly available: expert annotation hours through the research group's clinical collaborators (annotation is documented normal work in the group; no commitment inferred). Currently uncertain: affordable scale of expert annotation; access to versioned guideline text under licensing. The direction runs largely on **published literature rather than protected health data**, so the enclave and IRB path is not on the critical path until the Aim 3 clinical instantiation.

### 14. Novelty-collision risks

LINS is the sharpest collision: it claims outdated-knowledge handling and evidence validity at system level; if its mechanism (or a successor's) already implements per-claim adequacy/currency verification, the contribution shrinks to benchmark-plus-calibration. Commercial evidence-grounded products were not examined on Day 1 and could occupy the space without academic papers. Reviewer objections to anticipate: "adequacy equals GRADE automation, already studied in systematic-review tooling" (the answer must be the verification-calculus and calibration contribution, not the appraisal component); "another benchmark paper." Commoditization: frontier models with retrieval may absorb support checking; adequacy and currency depend on external state (versions, retractions) that parametric capability cannot absorb, which is the resilient core.

### 15. Advisor / expertise complementarity

**Required expertise:** clinical NLP; knowledge representation and terminologies; evidence-based-medicine appraisal methodology; benchmark and calibration methodology.

**Strongest plausible IHI primary-advisor match: Genevieve Melton-Meaux** (IHI core faculty; Professor of Surgery; Senior Associate Dean for Health Informatics and Data Science; directs the Center for Learning Health System Sciences, per her official profile; associate director of the NLP/IE group and co-PI on the NSF rare-disease award, per public project roles archived in this stream). She would contribute clinical knowledge representation and terminology expertise, clinical governance of expert annotation, and the learning-health-system deployment framing in which an evidence-auditing verifier earns clinical meaning. **Dr. Zhang contributes** the biomedical knowledge-graph and LLM/IE methodology, the lab's graph substrate, and its verification-adjacent research line. **Why complementary:** the verification calculus needs both a clinical-epistemology half (what makes evidence adequate and current clinically) and a computational half (retrieval, entailment, calibration); the two profiles divide exactly there rather than duplicating on NLP systems work. **Alternative framing match: Constantin Aliferis** (IHI Director; Professor of Medicine; CTSI Chief Research Informatics Officer, per his official profile) if the direction is framed as rigorous evaluation methodology for clinical AI. **Remaining expertise gap:** formal EBM/biostatistics appraisal depth, likely from outside IHI core. Fit statements are inferences from public profiles; no willingness or availability is inferred.

### 16. Foundation-model resilience

High. Stronger base models increase the volume and fluency of confidently cited output, raising the value of independent adequacy/currency auditing; the currency dimension is anchored in external world-state a frozen model cannot know (Thelwall's result is the empirical demonstration). The benchmark and formalism remain scientific contributions even if verifier engineering commoditizes.

### 17. Publication and execution risk

Novelty bar: moderate to high in the crowded attribution space; the per-dimension framing must be defended against LINS-class systems on Day 2. Time to first publishable unit: moderate (benchmark plus audit achievable early). Single-point risk: expert annotation throughput. Ground truth: difficult but tractable (expert labels with adjudication). Reproducibility: high (public data, open verifier). Overtaking risk: real; three of the closest papers are 2025 to 2026.

### 18. Generalizability

Healthcare-specific: the evidence hierarchy, guideline dynamics, and clinical claim types are integral, not a testbed veneer. Transferable: the typed claim-evidence calculus, calibration of multi-dimension verifiers, and versioned-evidence evaluation methodology transfer to scientific claim verification generally (law and policy analogs plausible).

### 19. Strongest reason to reject the direction

The space is the most crowded of the four candidates: two Nature-family end-to-end systems (LIT-025; SourceCheckup) and an active ACL line already occupy adjacent territory, and unexamined commercial systems may already do adequacy-aware verification internally; the direction could reduce to "a better benchmark for a race already being run by better-resourced groups."

### 20. Evidence that would change the recommendation

Strengthen: Day 2 confirmation that no system (academic or commercial) verifies adequacy or currency per claim; expert annotators confirming high prevalence of adequacy/currency violations in frontier output. Weaken: LINS full text or successors implementing per-claim quality appraisal; evidence that currency violations are rare in practice. Kill: an existing expert-annotated multi-dimension claim-evidence benchmark with a calibrated verifier (precisely the artifact this direction proposes).

### 21. Day 1 verdict and verdict rationale

**ADVANCE.** The problem is quantified at scale by 2025 to 2026 sources, the proposed object is specific and falsifiable, the components demonstrably exist only separately, the data path avoids the enclave critical path, and the direction sits on this stream's deepest verified reading. The collision with LINS-class systems is the named Day 2 target.

### 22. Critical uncertainty / rejection trigger

Whether LINS-class academic systems or unexamined commercial products already implement per-claim adequacy/currency verification; the kill condition is an existing expert-annotated multi-dimension claim-evidence benchmark with a calibrated verifier. (Compressed from sections 14, 19, and 20.)

---

# Candidate C2: Diagnostic-state trajectories from longitudinal clinical records

### 1. Candidate identity

**Title:** Diagnostic-state trajectories: modeling when a suspected diagnosis becomes confirmed or excluded across a patient's longitudinal record.

**One-sentence identity:** This direction studies the patient-level diagnostic state (suspected, working, confirmed, excluded, historical) and its transitions over time as a first-class extraction and representation object, contributing a task formalism, an annotated benchmark, transition-aware models and metrics, and an application to rare-disease cohort ground truth.

### 2. Central scientific object

A representation: the diagnostic-state trajectory (typed states, transitions, resolving-event links anchored on a clinical timeline), together with an annotation scheme, a benchmark, transition-aware evaluation metrics, and state-carrying longitudinal models. (Extracted from the frozen artifact's section 8.)

### 3. Central scientific problem

A diagnosis mention in a note is often a hypothesis under investigation, not a fact; the resolving event (genetic testing, biopsy, specialist adjudication) arrives months later or never. Mention-level assertion classification (the canonical i2b2 2010 formulation) captures certainty at one point in one note; it does not model the patient-level state or its resolution. The consequences are concrete: code-based rare-disease cohorts carry double-digit error rates and coding-granularity limits (Yadaw et al. 2025, DOI 10.1101/2025.05.02.25325348), diagnostic delay is measured today by retrospective surveys (Faye et al. 2024, DOI 10.1038/s41431-024-01604-z: mean 4.7 years across 6,507 European patients), and cohort validation requires expensive clinician chart review. Stream 03's archived cohort work (empirical, magnitudes internal) found a subgroup carrying only legacy labels that structured data cannot resolve at all; notes are the only route.

### 4. Falsifiable dissertation thesis

**Proposed research hypothesis:** *Patient-level diagnostic state and its transitions are recoverable from longitudinal notes with fidelity sufficient to reproduce expert chart-review verdicts on diagnosis status; and models that represent the trajectory explicitly outperform per-mention assertion classification aggregated across notes, by margins that grow with record length and diagnostic complexity.*

Falsification: if per-mention assertion plus simple aggregation matches trajectory-aware modeling, the representational claim dies; if neither approach approaches adjudication fidelity, the application claim dies. Coherence test: the aims are three tests of the one thesis (formalize and measure; model; deploy against the ground-truth problem).

### 5. Evidentiary basis

- **Claim:** mention-level certainty is a solved-task foundation, not a patient-level solution. → i2b2 2010 (Uzuner et al., DOI 10.1136/amiajnl-2011-000203; assertion F1 0.936 at mention level); LLM-era successors at mention level (Ji et al. 2024, DOI 10.1109/ichi61247.2024.00039; Kocaman et al. 2025, arXiv:2503.17425). → *Source-supported findings.*
- **Claim:** patient-level timeline construction from notes is an open, hard task. → ChemoTimelines shared task (2024.clinicalnlp-1.53: cross-document treatment timelines; fine-tuned small models beat LLM prompting; "more sophisticated techniques necessary"). → *Source-supported finding.*
- **Claim:** code-based cohort definition has quantified error and granularity limits for rare disease. → Yadaw et al. 2025 (11.6 percent false-positive mapped codes; ICD-10 granularity limits). → *Source-supported finding.*
- **Claim:** the diagnostic odyssey is long and currently measured by survey recall. → Faye et al. 2024. → *Source-supported finding.*
- **Claim:** clinicians treat recorded rare-disease names as suspicions pending genetic resolution, and code-defined cohorts have both false positives and false negatives. → Stream 03 archived provenance (trajectory-question entry, 2026-08-20; collaborator-attributed, documented). → *Source-supported (documented domain-expert input), archived.*
- **Claim:** temporal substrate tasks exist and are mature enough to build on. → THYME (TACL Q14-1012), i2b2 2012 (DOI 10.1136/AMIAJNL-2013-001628). → *Source-supported findings.*

### 6. Closest and dangerous prior work

- **Wang et al. 2025** (AMIA; PMID 41726535): LLM pipeline distinguishing newly diagnosed versus suspected versus historical multiple myeloma and dating the earliest diagnosis; the closest single system; one disease pair, status classes without a general trajectory formalism.
- **KEEPER** (Schuemie et al. 2025, DOI 10.1038/s41746-025-01433-4): LLM case adjudication against structured-data profiles, concluded viable versus manual review for ten diseases; dangerous because it attacks the same ground-truth problem from structured data.
- **Dickerson et al. 2026** (DOI 10.64898/2026.03.23.26349012): whole-chart longitudinal oncology abstraction at 91 to 100 percent concordance, including recurrence status (a time-varying state).
- **Paverd et al. 2026** (DOI 10.64898/2026.02.10.26345124): open-LLM longitudinal trajectory reconstruction in liver disease at scale.
- **ChemoTimelines 2024** as the task-formulation precedent for cross-document timelines.
- **LIT-015** (Faviez et al. 2024): partner-site ML detection of the target disease family from EHRs; must be read before any novelty claim in the rare-disease instantiation (flagged in this stream's provenance).

### 7. Evidence-supported limitations of existing approaches

- Reported: KEEPER's authors state context windows prevent processing complete charts, performance is disease-dependent, and the study still required 1,828 manual reviews; ChemoTimelines organizers state LLM prompting underperforms; Yadaw et al. state code granularity limits; Wang et al. state single-site, single-disease scope without external validation.
- **Inferred by this stream:** the 2025 to 2026 systems are per-disease pipelines or whole-chart abstraction demonstrations; none surfaced on Day 1 defines diagnostic state and its transition dynamics as a general, disease-agnostic task with an annotation scheme, transition-aware metrics, and a public benchmark; and none evaluates whether trajectory structure (as opposed to strong per-document extraction plus aggregation) carries the fidelity. That representational question is the scientific core, untested as far as the Day 1 search shows.

### 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION.** What appears unresolved: (a) a general formalism and annotated corpus for patient-level diagnostic-state trajectories (states, resolving events, transition triggers) spanning multiple conditions; (b) transition-aware evaluation metrics (state-at-time fidelity, resolution-event detection, earliest-suspicion dating) rather than mention F1; (c) a controlled answer to whether explicit trajectory modeling beats assertion-plus-aggregation; (d) validated use as cohort ground truth against clinician adjudication in the rare-disease setting where structured data provably cannot resolve membership. Wang et al. 2025 and Dickerson et al. 2026 are the nearest neighbors and define the bar.

### 9. Proposed methodological contribution

A **representation** (the diagnostic-state trajectory: typed states, transitions, resolving-event links anchored on a THYME-style timeline), an **annotation scheme and benchmark** operationalizing it across diseases, **transition-aware metrics** (a new evaluation methodology; mention F1 is the wrong loss for state dynamics), and **models** that read longitudinally with explicit state (the modeling novelty is the state-carrying formulation, testable against aggregation baselines). The integration question (assertion plus temporal relations plus cross-document fusion) is posed as a representational hypothesis with a falsifiable answer, not as engineering.

### 10. Coherent dissertation aims

- **Aim 1 (formalize and measure).** Question: can diagnostic state be annotated reliably, and where do snapshot methods fail? → Method: annotation scheme; corpus on public longitudinal sources (MIMIC-family notes) plus, where authorized, institutional rare-disease records; inter-annotator agreement with partial-credit handling. → Experiment: run mention-level assertion SOTA per note, aggregate, score against trajectory labels. → Expected evidence: characterized failure modes of snapshot aggregation.
- **Aim 2 (model).** Question: does explicit trajectory modeling improve state-at-time and resolution detection? → Method: longitudinal readers with state (windowed LLM with state summary passing; structured-state decoding), against aggregation baselines and whole-chart prompting. → Experiment: ablate the state channel; vary record length. → Expected evidence: margins that grow with length/complexity (thesis clause 2).
- **Aim 3 (deploy on the ground-truth problem).** Question: does trajectory extraction reproduce expert adjudication of cohort membership where codes cannot? → Method: apply to a rare-disease cohort with an adjudicated sample (the setting this stream's archived cohort work established, including its four-strata design); compare against code-based and name-based definitions and a KEEPER-style structured-data adjudicator. → Expected evidence: fidelity versus clinician verdicts; corrected diagnostic-interval estimates versus survey-based figures (thesis clause 1).

### 11. Publication decomposition

Formalism, corpus, and snapshot-failure audit (Aim 1) → modeling paper with ablations (Aim 2) → clinical validation and cohort-science paper (Aim 3, informatics venue), plus a plausible early short paper on the annotation scheme. Failure of Aim 3 (fidelity insufficient for adjudication replacement) still leaves a defensible dissertation: the formalism, benchmark, metrics, and the negative result about how far narrative data can go, itself an evaluation finding this stream's provenance anticipated.

### 12. Evaluation strategy

Datasets: public longitudinal notes (MIMIC-family) for the open benchmark; institutional rare-disease cohort for Aim 3 (enclave-governed); ChemoTimelines as an external transfer test of the temporal machinery. Baselines: assertion SOTA plus aggregation rules; whole-chart LLM prompting; retrieval-augmented per-question chart QA; KEEPER-style structured adjudication for Aim 3. Ablations: remove state passing; remove temporal normalization; per-note versus cross-document. Metrics: state-at-time accuracy, transition/resolution-event F1 with time tolerance, earliest-suspicion dating error, cohort-level sensitivity/specificity versus adjudication. Statistics: patient-level bootstrap; agreement with hierarchical partial credit. Human evaluation: clinician adjudication on the Aim 3 sample (the only non-derived ground truth, per this stream's archived analysis).

### 13. Required resources and feasibility

Known available: public corpora (i2b2/THYME lineage under DUAs; MIMIC-family), the institutional data-shelter cohort with materialized tables and a large note corpus (archived, magnitudes internal), local model constraint honored (cloud APIs excluded on protected data), GPU cluster path identified. Plausibly available: clinician adjudication time via the funded project's collaborators (annotation is normal group work; site assignment for annotation was an open question flagged in this stream's provenance; no commitment inferred). Currently uncertain: whether protected note text may move to the GPU node (open governance question, archived); annotation budget for the public benchmark; institutional authorization timelines.

### 14. Novelty-collision risks

Closest overlaps: Wang et al. 2025 (status classes plus dating, one disease), Dickerson et al. 2026 (whole-chart abstraction concordance), Paverd et al. 2026 (longitudinal reconstruction), KEEPER (adjudication replacement), and the unread partner-site precedent LIT-015. Reviewer objections to anticipate: "assertion classification plus temporal relation extraction, re-packaged" (the answer must be the controlled representation experiment and the transition-aware metrics); "single-institution clinical validation." Commoditization risk: long-context frontier models may make whole-chart prompting strong enough that explicit state buys little; that outcome is a legitimate falsification of thesis clause 2, and the benchmark plus fidelity-versus-adjudication result (clause 1) survives it.

### 15. Advisor / expertise complementarity

**Required expertise:** temporal clinical NLP and assertion modeling; EHR secondary-use and phenotyping methodology; observational cohort-science methods; clinical adjudication access (nephrology/genetics for the rare-disease instantiation).

**Plausible IHI primary-advisor matches, depending on framing.** For the clinical-NLP-forward framing: **Genevieve Melton-Meaux** (IHI core; clinical NLP and terminology work with deep EHR documentation expertise per her official profile and the institute's NLP publications; Center for Learning Health System Sciences director). She contributes clinical-documentation and terminology depth plus clinical governance of the adjudication study; Dr. Zhang contributes LLM/IE modeling and the rare-disease project's infrastructure; complementary because the decisive Aim 3 is a clinical-validation study needing exactly the clinical-informatics oversight that the external advisor's methods focus does not duplicate. For the cohort-science framing: **Gyorgy Simon** (IHI faculty; PhD in computer science with a statistics minor and a clinical data-mining record at Mayo Clinic, per his official profile). He contributes statistical phenotyping and EHR data-mining methodology for the fidelity-versus-adjudication design; Dr. Zhang again supplies the NLP/LLM half; complementary because the pairing separates representation learning (external) from validation methodology (primary). **Remaining expertise gap:** clinical domain adjudicators (nephrology/genetics) beyond the informatics committee. The direction runs inside the funded project's documented US-site task assignments (feasibility statement only). Fit statements are inferences from public profiles; no willingness or availability is inferred.

### 16. Foundation-model resilience

Moderate to high. Better base models improve per-document reading, which strengthens Aim 1's baselines and may narrow Aim 2's margins (acknowledged falsification path). The durable contributions are the formalism, the benchmark, the transition-aware evaluation methodology, and the validated ground-truth instrument; the need to establish diagnostic state against later resolving events is a property of the clinical record, not of model capability.

### 17. Publication and execution risk

Novelty bar: moderate; the formalism-and-benchmark route is defensible but the 2026 neighbors are close. Time to first unit: moderate (Aim 1 needs annotation before anything publishes). Single-point risk: clinician adjudication access for Aim 3; mitigated because Aims 1 and 2 run on public data. Ground truth: hard by construction (that is the point); the resolving-event anchor (genetic testing) gives a natural label. Reproducibility: high for public aims, low for the enclave aim (institutional data cannot be released; mitigate with released code and the public benchmark). Overtaking risk: moderate to high; chart-abstraction work is moving fast.

### 18. Generalizability

Healthcare-specific: diagnostic sociology (suspicion, work-up, resolution) and the clinical record's structure are integral; this is not a testbed framing. Transferable: state-trajectory extraction from longitudinal document streams generalizes to legal matters, incident investigations, and any domain where entity status resolves over a document series; the transition-aware evaluation methodology is domain-general.

### 19. Strongest reason to reject the direction

Its decisive experiment (Aim 3) sits behind institutional data governance and clinician time, the two resources this stream's own feasibility evidence identifies as the binding constraints; if adjudication access stalls, the dissertation's clinical anchor weakens to a public-data methods contribution in a space where strong groups are already demonstrating near-expert whole-chart abstraction.

### 20. Evidence that would change the recommendation

Strengthen: confirmation that no general trajectory formalism/benchmark exists (Day 2); a pilot showing snapshot aggregation fails badly on even a small trajectory sample; resolution of the annotation-assignment question in the funded project. Weaken: LIT-015 or ChemoTimelines-successor work turning out to cover diagnostic-state dynamics; long-context models matching trajectory models in a pilot. Kill: an existing multi-disease diagnostic-state benchmark with transition metrics, or institutional denial of the adjudicated-sample path with no public substitute.

### 21. Day 1 verdict and verdict rationale

**ADVANCE.** It is the most distinct direction in this portfolio, it attacks a problem whose importance is quantified independently of any system fashion, this stream holds unique empirical grounding for it, and its representational core question is cleanly falsifiable. The governance-gated decisive experiment is the named risk.

### 22. Critical uncertainty / rejection trigger

Whether the clinician-adjudication path for the decisive Aim 3 materializes (governance and clinician time), and whether Day 2 reading of LIT-015 and the 2026 neighbors reveals an existing diagnostic-state formalism; the kill conditions are an existing multi-disease trajectory benchmark or institutional denial of the adjudicated sample with no public substitute. (Compressed from sections 14, 19, and 20.)

---

# Candidate C3: Selective control for clinical language systems under asymmetric risk

### 1. Candidate identity

**Title:** Selective control beyond multiple choice: predicting failure and choosing among answer, retrieve, flag, and defer for clinical extraction and generation.

**One-sentence identity:** This direction studies when a clinical language system should not act on its own output, contributing failure-predictive signals derived from task structure (retrieval agreement, ontology consistency, evidence-state features), a decision layer that chooses among actions under clinically asymmetric costs, and an evaluation methodology for selective behavior on extraction and generation tasks rather than multiple-choice QA.

### 2. Central scientific object

A controller: a failure-prediction representation over task-structural signals, a cost-sensitive multi-action decision layer (answer, retrieve, flag, defer) extending learning-to-defer with conformal risk control at document and cohort level, and an evaluation methodology for selective behavior on extraction. (Extracted from the frozen artifact's section 8.)

### 3. Central scientific problem

Clinical deployment requires knowing which outputs to trust, and the burden cannot rest on human vigilance: a randomized trial found physicians exposed to deliberately erroneous LLM suggestions dropped 14 percentage points in diagnostic accuracy despite AI-literacy training and full autonomy (Qazi et al. 2025, medRxiv 10.1101/2025.08.23.25334280, abstract-level). LLMs almost never abstain under medical uncertainty (LIT-026, MedQAbstain), hallucination prevalence is high and clinician-perceived harm is real (Kim et al. 2025, arXiv:2503.05777), and dynamic stress-testing collapses static-benchmark performance (LIT-032: 94 percent of previously correct answers failed under dynamic robustness testing, per its preprint arXiv:2508.00923). The open problem is a principled, clinically costed control layer for the tasks that actually run in pipelines (extraction, normalization, generation), where the action space is richer than answer-or-abstain.

### 4. Falsifiable dissertation thesis

**Proposed research hypothesis:** *For clinical extraction and generation, failure-predictive signals computed from task structure (candidate-set agreement, ontology-consistency checks, evidence-state features) support risk-coverage tradeoffs that dominate model-internal confidence, self-consistency, and frontier self-verification, under site and distribution shift; and a cost-sensitive controller using them chooses among answer, retrieve, flag, and defer so as to reduce clinically weighted risk at fixed human workload.*

Falsification: if frontier self-estimates match or beat structural signals under shift, the thesis core dies; if richer action spaces buy nothing over binary abstention, the control claim dies. Coherence test: the aims test signal validity, control value, and clinical transfer of the same thesis.

### 5. Evidentiary basis

- **Claim:** models systematically overcommit on medical QA. → LIT-026 (ACL 2026.acl-long.1365). → *Source-supported finding.*
- **Claim:** human oversight fails under erroneous suggestions. → Qazi et al. 2025 RCT. → *Source-supported finding (abstract-level; published version not read).*
- **Claim:** static accuracy is a poor reliability estimate. → LIT-032 / arXiv:2508.00923. → *Source-supported finding.*
- **Claim:** sycophancy is a conversation-level property with large per-question variance. → Ping et al. 2026, arXiv:2608.01017. → *Source-supported finding.*
- **Claim:** conformal and deferral machinery exists and is being applied to medical MCQA. → Ke et al. 2025 (arXiv:2503.05505); MedAbstain (arXiv:2601.12471); CIC (arXiv:2607.04430); Bary et al. (arXiv:2509.12573); Mozannar and Sontag 2020 (arXiv:2006.01862). → *Source-supported findings.*
- **Claim:** structural verification signals carry information that model confidence does not, in the clinical extraction setting. → *Preliminary gap hypothesis grounded in this stream's archived proposal (family-scoped verification counts as flag signals, keep-and-flag design, 2026-07-23) and LIT-001's verification gains; untested as a selective-prediction signal.*

### 6. Closest and dangerous prior work

- **MedAbstain** (arXiv:2601.12471, EACL 2026): unifies conformal prediction, perturbations, and abstention on medical MCQA; the most dangerous single item, claiming its discrete-choice setting "generalizes to agentic action selection."
- **MedQAbstain** (LIT-026): abstention benchmark, MCQA.
- **CIC** (arXiv:2607.04430): guaranteed selective answering, general QA.
- **Conformal deferral without learning** (arXiv:2509.12573).
- **MedVAL** (arXiv:2507.03152): trained evaluator LMs judging factual consistency of medical text, reported statistically non-inferior to a single expert; dangerous as an already-strong learned verifier for generation.
- **Know Your Limits** survey (DOI 10.1162/tacl_a_00754): the field map any contribution must be positioned in.

### 7. Evidence-supported limitations of existing approaches

- Reported: MedQAbstain and MedAbstain both find overcommitment robust to prompting and scale; Ke et al. note conformal guarantees are marginal (average-case); the survey motivates abstention as an underdeveloped meta-capability; LIT-030 (DOI 10.1038/s41746-026-02443-6) reports agentic scaffolding did not substantially reduce hallucinations.
- **Inferred by this stream:** the abstention literature surfaced on Day 1 is MCQA-centric; selective prediction for clinical extraction pipelines (span plus normalization outputs, thousands of decisions per document, ontology structure available as a signal) and for generation with clinically weighted costs appears far less developed; deferral work is classification-centric; no surfaced work uses external verification structure (knowledge-graph or ontology consistency) as the failure-predictive signal in this setting. MedVAL is the nearest generation-side verifier and must be treated as a baseline, not ignored.

### 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION.** What appears unresolved: selective prediction with statistical risk control for clinical extraction and generation (not MCQA), using task-structural failure predictors, evaluated under site/language shift with clinically asymmetric costs and a beyond-binary action space, together with the finding of when structural signals beat model-internal ones. MedAbstain's generalization claim and MedVAL's verifier strength are the two claims most likely to preempt parts of this; both are explicit Day 2 targets.

### 9. Proposed methodological contribution

A **failure-prediction representation** (structural signals: retrieval-candidate agreement, ontology-consistency features, verification-count features in the spirit of this stream's archived keep-and-flag design), a **cost-sensitive controller** (a learning objective extending learning-to-defer to multi-action clinical settings with conformal risk control at the document and cohort level, not per-question), and an **evaluation methodology** for selective behavior on extraction (risk-coverage under shift, workload-normalized comparisons). The control layer is metacognitive in the literal sense: a model of the system's own reliability, learned from task structure.

### 10. Coherent dissertation aims

- **Aim 1.** Question: which signals predict extraction/generation failure, and do structural signals beat internal confidence under shift? → Method: instrument a phenotyping pipeline (LIT-003-style) and a generation task; train failure predictors per signal family. → Experiment: cross-site and cross-language evaluation; compare against self-verification and MedVAL-style judges. → Expected evidence: AUROC/risk-coverage by signal family and shift condition.
- **Aim 2.** Question: does a multi-action controller beat binary abstention at fixed workload? → Method: cost-sensitive controller with conformal risk control; actions answer/retrieve/flag/defer. → Experiment: clinically weighted cost matrices (elicited with clinical collaborators); workload-matched comparisons. → Expected evidence: dominated risk-coverage curves, or a falsifying null.
- **Aim 3.** Question: does the controller hold up in the rare-disease setting where stakes and sparsity are extreme? → Method: instantiate on the funded project's extraction setting under enclave constraints (local models). → Expected evidence: transfer of the risk-control guarantees to a real cohort pipeline.

### 11. Publication decomposition

Signal study and shift benchmark (Aim 1) → controller method paper (Aim 2) → clinical instantiation (Aim 3). Early unit: the instrumented shift benchmark alone. If Aim 2's null falsifies the action-space claim, Aim 1's signal findings and benchmark still publish and still inform the field's baseline choices; the dissertation survives as measurement plus a negative control result, though weakened.

### 12. Evaluation strategy

Datasets: public clinical IE corpora with site splits; multilingual phenotyping data where authorized; MedQAbstain/MedAbstain for comparability on the QA slice. Baselines: max-probability and entropy confidence, self-consistency, frontier self-verification, MedVAL-style learned judge, conformal MCQA adaptations. Ablations: each signal family removed; conformal on/off; binary versus multi-action. Metrics: risk-coverage curves and AURC, violation rates of risk guarantees, workload-normalized clinical cost. Statistics: patient-level bootstrap; guarantee-violation tests. Human evaluation: clinician utility elicitation for the cost matrix and review of deferred cases.

### 13. Required resources and feasibility

Known available: public IE corpora; local GPU path; the instrumented pipeline setting from the funded project's task assignments. Plausibly available: cross-site or cross-language splits via the project's collaboration (policy-gated; the international component is constrained per archived guidance, so language shift may need public French corpora instead). Currently uncertain: clinical cost-elicitation time; whether guarantees survive realistic shift (a scientific risk, not a resource one).

### 14. Novelty-collision risks

MedAbstain (conformal plus abstention plus perturbations, with a generalization claim), CIC (guaranteed selective answering), Bary et al. (conformal deferral), and MedVAL (strong learned verifier) together box in much of the space; the surviving territory is the extraction setting, structural signals, and multi-action control, which a skeptical reviewer could call "conformal risk control plus feature engineering." The strongest defense is the shift result (if structural signals genuinely dominate under shift, that is a scientific finding); if they do not, the direction collapses to incremental engineering. Commoditization risk is the highest of the four candidates: frontier self-verification is improving on exactly this axis, and the field's own survey frames abstention as a capability labs are optimizing directly.

### 15. Advisor / expertise complementarity

**Required expertise:** statistical learning theory (conformal methods, decision theory, learning-to-defer); clinical NLP systems; clinical collaborators for cost elicitation.

**Plausible IHI primary-advisor matches:** **Erich Kummerfeld** (IHI faculty; official profile states his primary research interest is statistical and machine-learning methods, with a focus on causal discovery and latent-variable models), the closest IHI match to the statistical-methodology core this direction needs; or **Constantin Aliferis** (IHI Director; ML methodology and research-rigor leadership via CTSI, per his official profile) if the direction is framed as reliability methodology for clinical AI. Either contributes the statistical-theory half (validity of guarantees, method soundness); **Dr. Zhang contributes** the clinical NLP/LLM systems and tasks the controller governs, plus the group's agent-evaluation context (LIT-014). **Why complementary:** the pairing separates guarantee methodology (primary) from the systems being controlled (external) with no duplicated territory. **Remaining expertise gap / caution** (archived previously in this stream and repeated): whether these methodologists have LLM-adjacent interests is not established by their profiles; this is a fit inference only, and this direction's advisor risk is accordingly higher than C1/C2's. No willingness or availability is inferred.

### 16. Foundation-model resilience

The weakest of the four. The thesis explicitly bets that structural signals beat model-internal ones; if frontier self-verification closes that gap, the core finding inverts. The residue that survives (risk-control methodology, workload-normalized evaluation, cost elicitation) is real but thinner. This is penalized in the verdict.

### 17. Publication and execution risk

Novelty bar: high; the space is dense and fast (four of the closest items are 2025 to 2026). Time to first unit: fast (Aim 1 is executable on public data quickly). Single-point risk: the central comparative claim could resolve against the thesis early (informative but strategically costly). Ground truth: moderate (extraction gold standards exist; their own noise interacts with C4). Reproducibility: high on public aims. Overtaking risk: the highest in this portfolio.

### 18. Generalizability

Healthcare-specific: cost asymmetries and the deployment context are integral to the evaluation design. Transferable: selective prediction for structured-output NLP, multi-action risk control, and shift-robust failure prediction transfer to any high-stakes extraction domain.

### 19. Strongest reason to reject the direction

Its central bet sits directly in the blast radius of frontier-lab optimization: abstention and self-verification are capabilities the model builders measure and train for, several 2026 systems already unify the key machinery on adjacent tasks, and a dissertation could spend three years establishing a comparison whose answer changes with each model release.

### 20. Evidence that would change the recommendation

Strengthen: a pilot showing structural signals clearly dominate internal confidence under site shift; Day 2 confirmation that extraction-setting selective prediction is genuinely unoccupied. Weaken: MedAbstain's full text covering structured/agentic outputs; frontier self-verification matching structural signals in the pilot. Kill: a published demonstration that model-internal uncertainty suffices for clinical extraction risk control under shift.

### 21. Day 1 verdict and verdict rationale

**ADVANCE WITH MAJOR UNCERTAINTY.** The problem's importance is exceptionally well evidenced (an RCT on oversight failure; systematic overcommitment findings), and the extraction-setting gap looks real today; but the field's velocity, the density of 2026 prior art, and the direct dependence of the thesis on a moving frontier make this the riskiest advance. Day 2 must test MedAbstain and MedVAL hard before this direction is allowed near finalist status.

### 22. Critical uncertainty / rejection trigger

Whether frontier self-verification (and MedAbstain's claimed generalization beyond MCQA) already matches or will shortly match task-structural failure signals under shift; the kill condition is a published demonstration that model-internal uncertainty suffices for clinical extraction risk control under shift. (Compressed from sections 14, 16, 19, and 20.)

---

# Candidate C4: Measurement error in clinical NLP evaluation

### 1. Candidate identity

**Title:** How much of reported clinical NLP error is measurement artifact? A measurement-error methodology for clinical language evaluation.

**One-sentence identity:** This direction studies the evaluation instrument itself, contributing a decomposition of reported system error into scoring artifact (surface-form matching, ontology granularity, label noise, judge bias) versus true error, noise-aware ranking inference, and corrected evaluation protocols for clinical extraction and normalization.

### 2. Central scientific object

An evaluation instrument in the metrology sense: a measurement model for clinical IE evaluation (error decomposition with estimators per artifact source), a noise-aware ranking-inference procedure, and a validated corrected-evaluation protocol and toolkit. (Extracted from the frozen artifact's section 8.)

### 3. Central scientific problem

Clinical NLP conclusions rest on benchmark scores, but multiple independent results indicate the scores partly measure the scoring method: exact-match agreement on clinical concept normalization was 52.4 percent between expert annotators while hierarchical agreement was 78.2 percent (CUILESS2016, DOI 10.1186/s13326-017-0173-6); automated metrics anti-correlate with human rankings in medical summarization (Wang et al., ACL 2023.acl-long.549); token- versus span-based scoring flips clinical NER leaderboard rankings (Abdul et al., arXiv:2410.05046); 3.3 percent test-label error destabilizes benchmark rankings in general ML (Northcutt et al., arXiv:2103.14749); LLM judges discriminate poorly and disagree with clinicians on reasons even when verdicts agree (DeLucia et al., arXiv:2604.16383). Stream 03's own archived cross-paper inference (two independent papers whose dominant false negatives were linguistic variation, not extraction failure) is the same phenomenon. If artifact fractions are large, method comparisons, clinical-readiness claims, and the field's error analyses are partly artifacts of the ruler.

### 4. Falsifiable dissertation thesis

**Proposed research hypothesis:** *A substantial and quantifiable fraction of reported error in standard clinical extraction and normalization evaluations is measurement artifact rather than system error; correcting for it with semantically valid, noise-aware evaluation changes system rankings and at least one accepted substantive conclusion; and artifact-corrected evaluation is itself measurable for validity (agreement with expert adjudication) rather than merely different.*

Falsification: if expert re-adjudication shows artifact fractions are small; or if corrected metrics reshuffle nothing; or if "corrected" evaluation agrees with experts no better than exact match, the thesis fails. Coherence test: the aims are three tests of one thesis (quantify the artifact; build the corrected instrument; show conclusions change and validate the instrument).

### 5. Evidentiary basis

Each item in section 3 is a *source-supported finding* from a primary page read on Day 1, with identifiers as listed. Additional basis: Groza et al. 2024 (DOI 10.1186/s12911-024-02439-w) anchors current phenotype-CR evaluation practice and reports run-to-run non-determinism as an evaluation problem; Köhler et al. 2009 (DOI 10.1016/j.ajhg.2009.09.003) establishes the ontology semantic-similarity machinery a corrected instrument builds on; the LLM-as-judge scoping analysis (arXiv:2605.25273) reports judge reliability "varies substantially across tasks." **Cross-paper inference (this stream):** these results, from disjoint subfields, are the same phenomenon (the instrument contributing variance and bias), and no surfaced work unifies them into a decomposition methodology for clinical NLP; the retrieval agent's coverage note records that no source directly decomposing clinical-IE error into artifact versus true error was found on Day 1.

### 6. Closest and dangerous prior work

- **Alaa et al. 2025** (arXiv:2503.10694): position paper arguing medical LLM benchmarks should prioritize construct validity, with proof-of-concept experiments; the conceptual frame exists, the systematic instrument does not (per abstract).
- **Northcutt et al. 2021**: the general-ML label-error anchor and confident-learning machinery.
- **CUILESS2016**: the sharpest clinical quantification of exact-versus-hierarchical agreement.
- **Abdul et al. 2024**: metric-choice rank flips in clinical NER.
- **Dangerous prior art:** **Labbe et al. 2026** (ACL 2026.bionlp-1.5) explicitly introduces a hierarchy-aware evaluation framework beyond exact-match metrics for HPO phenotype linking; **Köhler 2009** and the HPO semantic-similarity tradition already provide ontology-aware scoring; Wang et al. 2023 already demonstrates metric-human anti-correlation in one clinical task. Any novelty claim must be positioned as the *decomposition and inference methodology across artifact sources*, not as "score with the ontology," which exists.

### 7. Evidence-supported limitations of existing approaches

- Reported: CUILESS2016 reports the agreement gap but stops at annotation; Abdul et al. report rank flips but propose no corrected inference; Alaa et al. call for construct validity but present proof-of-concept only; DeLucia et al. report judge unreliability without a correction method; Groza et al. report evaluation instability without decomposition.
- **Inferred by this stream:** the field lacks (a) estimates of artifact fractions on the benchmarks that drive clinical NLP conclusions, (b) an inference procedure that propagates label noise and scoring uncertainty into ranking confidence (Northcutt-style confident learning has not, per the Day 1 search, been applied to clinical IE), and (c) validated semantic-equivalence adjudication protocols cheaper than full expert re-annotation.

### 8. Preliminary research gap

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION.** What appears unresolved: a measurement-error methodology for clinical NLP evaluation that (a) decomposes reported error into surface-form artifact, granularity artifact, label noise, and judge bias with uncertainty estimates; (b) provides noise-aware ranking inference (does system A really beat system B given instrument error?); and (c) validates corrected metrics against expert adjudication. Hierarchy-aware scoring alone is *not* the gap (Labbe 2026, Köhler 2009 occupy it); the decomposition-and-inference layer is.

### 9. Proposed methodological contribution

A **measurement model** for clinical IE evaluation (an error decomposition with estimators for each artifact source: paraphrase-equivalence via adjudicated semantic matching, granularity via ontology-distance-aware credit, label noise via confident-learning adapted to structured clinical outputs, judge bias via clinician-anchored calibration), a **ranking-inference procedure** (uncertainty-aware benchmark conclusions), a **corrected-evaluation protocol and toolkit**, and **re-evaluations** of published systems demonstrating which conclusions survive. This is evaluation methodology in the metrology sense: the contribution is the instrument science, and it must itself be validated (Aim 3), which elevates it above a critique paper.

### 10. Coherent dissertation aims

- **Aim 1 (quantify).** Question: what are the artifact fractions on the benchmarks behind current clinical extraction and normalization claims? → Method: stratified expert re-adjudication of system-versus-gold disagreements on public corpora (phenotype CR, clinical NER/normalization); classify each disagreement as artifact type or true error. → Expected evidence: artifact-fraction estimates with confidence intervals; the first direct decomposition (per the Day 1 search).
- **Aim 2 (correct and infer).** Question: can corrected metrics and noise-aware inference change conclusions without merely being different? → Method: build the estimators and ranking-inference procedure; re-score published leaderboards and canonical comparisons. → Expected evidence: which rankings and claims survive; quantified conclusion fragility.
- **Aim 3 (validate the instrument).** Question: do corrected metrics agree with expert judgment better than standard ones, at what cost? → Method: blinded expert preference and adjudication studies; cost accounting for the adjudication protocol. → Expected evidence: validity gain per annotation dollar; a deployable protocol.

### 11. Publication decomposition

Artifact-fraction audit (Aim 1, strong standalone paper) → decomposition and inference methodology with re-evaluations (Aim 2) → validation and protocol/toolkit paper (Aim 3). Early unit: the Aim 1 audit on one task. If Aim 2's corrections do not change conclusions, the result is still publishable and important (benchmarks are robust; artifact fears overstated), and the toolkit and audit remain reusable artifacts; the dissertation survives with a deflationary but defensible thesis resolution.

### 12. Evaluation strategy

Datasets: public phenotype-CR corpora (the Groza et al. suite), clinical NER/normalization benchmarks (Abdul et al. suite), the CUILESS lineage, medical summarization sets with human facets (Wang et al. 2023). Baselines: exact match, span/token variants, existing semantic and hierarchy-aware metrics (Köhler-style similarity, Labbe 2026's framework as a direct comparator), LLM judges. Ablations: each estimator removed; adjudication-protocol depth varied. Metrics: artifact fractions with CIs; ranking stability (rank correlation under correction); agreement with expert adjudication (the validity criterion). Statistics: hierarchical bootstrap over documents and annotators; noise-propagating significance tests for system comparisons. Human evaluation: central and unavoidable (expert adjudication is the ground truth of the instrument study); design must budget it explicitly.

### 13. Required resources and feasibility

Known available: public corpora and published system outputs (many with released code per Day 1 pages); ontologies (LIT-006/007); no protected data required anywhere in the core aims. Plausibly available: expert adjudication hours (smaller than a de novo annotation effort because only disagreements are adjudicated; the design's cost lever). Currently uncertain: whether published system outputs are recoverable for re-scoring at sufficient scale (mitigation: re-run open systems); adjudicator recruitment beyond the immediate collaboration.

### 14. Novelty-collision risks

Labbe 2026 and the semantic-similarity tradition own "score with the hierarchy"; Alaa et al. own the construct-validity framing; Northcutt owns label-noise machinery. The direction collapses into incremental territory if it amounts to applying each existing tool to one more dataset; the defense is the unified decomposition with validated inference, which no surfaced work provides. Reviewer objections to anticipate: "meta-research, not methods" (answer: the estimators and inference procedure are methods, and Aim 3 makes validity itself measurable); "cherry-picked artifact examples" (answer: stratified sampling with pre-registered protocols). A subtler risk: the field may not reward instrument science at dissertation scale in NLP venues; venue fit needs Day 2 attention (the ACL evaluation/metrics track and JAMIA methodological papers are the plausible homes).

### 15. Advisor / expertise complementarity

**Required expertise:** clinical NLP evaluation practice; ontologies and terminologies; measurement modeling / biostatistics; clinician adjudicators.

**Plausible IHI primary-advisor matches:** **Genevieve Melton-Meaux** (IHI core; terminology and clinical-NLP evaluation practice per her official profile and the institute's NLP portfolio) for the clinical-instrument framing: she contributes the terminology/equivalence expertise at the heart of the granularity and paraphrase estimators, plus adjudication governance. **Constantin Aliferis** (IHI Director; CTSI research-informatics leadership) for the research-rigor framing: his official profile's methods-and-rigor orientation matches an instrument-science dissertation. **Dr. Zhang contributes** the NLP systems, benchmarks, and evaluation practice being audited, plus the venue reach for the re-evaluation studies; the combination is complementary because the primary owns the measurement/clinical-semantics side while the external owns the systems side, and neither profile duplicates the other's role in an instrument study. **Remaining expertise gap:** formal measurement/psychometrics or biostatistics depth, plausibly from outside IHI core. Fit statements are inferences from public profiles; no willingness or availability is inferred.

### 16. Foundation-model resilience

The highest of the four. Stronger models make evaluation the binding constraint of the field: as system error shrinks toward instrument error, artifact-dominated benchmarks become useless precisely when the stakes are highest, and every capability claim (including the frontier labs' own clinical claims) depends on instruments this direction studies. Nothing here competes with model capability.

### 17. Publication and execution risk

Novelty bar: moderate (the unified methodology appears open, but each component has an owner; the synthesis must be argued as a contribution, a real rhetorical risk). Time to first unit: fast (the Aim 1 audit needs modest adjudication on existing corpora). Single-point risk: low (no experiment is existential; even null artifact fractions publish). Ground truth: the study's own subject, handled by design. Reproducibility: highest of the four (all public). Overtaking risk: low to moderate; the area is active (2025 to 2026 position papers) but no group surfaced on Day 1 is building the decomposition instrument.

### 18. Generalizability

Healthcare-specific: ontology structure, clinical equivalence judgments, and clinician adjudication are integral to the estimators. Transferable: the decomposition methodology, noise-aware ranking inference, and validity-audit protocol transfer to any structured-output NLP evaluation; the general-domain version is itself a publishable extension.

### 19. Strongest reason to reject the direction

It is a dissertation about the ruler rather than the phenomenon: it produces no clinical capability, its committee-facing narrative ("your benchmarks are partly artifact") wins arguments but not necessarily allies, and if Aim 1 finds modest artifact fractions the remaining aims deflate to careful confirmation of the status quo; a risk-averse reading says this is one strong paper wearing a dissertation's clothes.

### 20. Evidence that would change the recommendation

Strengthen: an Aim 1 pilot on one corpus showing artifact fractions above, say, a quarter of reported error; Day 2 confirmation that no decomposition methodology exists; evidence that clinical-readiness claims in the literature rest on artifact-heavy benchmarks. Weaken: pilot artifact fractions small; discovery of an existing noise-aware evaluation line in clinical NLP. Kill: a published clinical-IE error decomposition with validated corrected metrics (this direction's core artifact).

### 21. Day 1 verdict and verdict rationale

**ADVANCE WITH MAJOR UNCERTAINTY.** The evidence that the problem is real is unusually convergent and quantitative, feasibility and resilience are the best in the portfolio, and this stream's own provenance independently observed the phenomenon twice; the uncertainty is scope-sizing (dissertation versus strong paper) and the density of component-level prior art. A cheap Aim 1 pilot is the designated uncertainty-resolver.

### 22. Critical uncertainty / rejection trigger

Whether artifact fractions are large enough to change conclusions and whether the direction is dissertation-sized rather than one strong paper; the designated resolver is a cheap Aim 1 pilot, and the kill condition is an existing published clinical-IE error decomposition with validated corrected metrics. (Compressed from sections 19 and 20.)

---

# Layer III — Portfolio-level analysis

## A. Candidate diversity check

These are four distinct falsifiable theses about four distinct objects: a verification calculus over claim-evidence pairs (C1), a longitudinal state representation (C2), a control policy over system actions (C3), and a measurement model of the evaluation instrument (C4). They are not variants of one thesis. However, honesty requires naming the family resemblance: C1, C3, and C4 all descend from one architectural principle this stream has held since July (generation cannot verify itself; checking requires an independent instrument), applied to evidence, to actions, and to evaluation respectively. C2 is the most independent, organized around a representational claim about the clinical record. There is also a designed synergy rather than an overlap: C4's corrected metrics would be the right scoring for C2's benchmark and C3's risk estimates; C1's verifier could supply C3's structural signals. A finalist portfolio should probably not carry both C1 and C3 forward as separate directions; if both survive Day 2, merging C3 into C1's Aim 3 (verification-driven selective control) is the coherent combination.

## B. Qualitative scientific comparison matrix

| Dimension | C1 verification | C2 trajectories | C3 selective control | C4 measurement |
|---|---|---|---|---|
| Scientific importance | High (auditability of clinical AI) | High (ground truth for cohort science; odyssey measurement) | High (safety layer; oversight demonstrably fails) | High (validity of the field's conclusions) |
| Methodological depth | Formalism + calibration + benchmark | Representation + metrics + corpus | Decision theory + risk control | Measurement modeling + inference |
| Falsifiability / discriminating experiment | Aim 1 audit: does an adequacy/currency failure mass exist beyond entailment support? (explicit falsification conditions stated) | Aim 1/2 controlled comparison: trajectory modeling versus assertion-plus-aggregation; Aim 3 fidelity versus adjudication | Aim 1 pilot: structural signals versus internal confidence and self-verification under shift | Aim 1 pilot: artifact-fraction estimate with expert re-adjudication |
| Preliminary novelty headroom | Moderate (crowded; per-dimension calculus open) | Moderate-high (formalism open; neighbors close) | Low-moderate (dense 2026 art; extraction slice open) | Moderate (components owned; decomposition open) |
| Publication tractability | Good; early benchmark unit | Moderate; annotation before first unit | Fast first unit; venue competition fierce | Fast first unit; venue fit needs care |
| Empirical feasibility | High (public data core) | Split (public aims + governed decisive aim) | High (public core; clinical aim governed) | Highest (all public) |
| Time to uncertainty resolution | Fast (the critical uncertainty is a Day 2 literature/product check) | Slow (governance and annotation precede the decisive evidence) | Fast to moderate (the central comparison could resolve early, per the risk analysis) | Fast (cheap Aim 1 pilot is the designated resolver) |
| Artifact/reuse potential | Benchmark + verifier | Corpus + formalism + instrument | Benchmark + controller | Toolkit + protocol (field-serving) |
| Foundation-model resilience | High (external world-state) | Moderate-high (record property; margins may shrink) | Lowest (bets against frontier self-verification) | Highest (instrument science) |
| IHI advisor/resource feasibility | Strong local fit (named matches); EBM methodology to add | Strongest empirical grounding in-stream; governance-gated; named matches by framing | Local fit via methodological faculty; LLM-adjacency of matches unverified | Local fit (named matches); measurement/biostat depth to add |
| Transferable technical depth | Calibration, verification systems | Longitudinal IE, evaluation design | Risk control, selective prediction | Metrology, inference under noise |
| Largest unresolved uncertainty | LINS-class and commercial preemption | Adjudication access; long-context commoditization of Aim 2 | Frontier self-verification closing the gap | Artifact fractions unknown; scope-sizing |

## C. Missing-direction check

Directions considered and deliberately not carried forward on Day 1, with reasons: **evidence-substrate construction** (building the temporally versioned, provenance-tiered rare-disease knowledge base that C1 consumes) collides frontally with LIT-004's territory and reads as resource engineering unless a methodological problem is isolated; **federated/multilingual evaluation under privacy constraints** is scientifically live but sits behind the international-collaboration policy risk this stream has documented, disqualifying for a dissertation spine on current evidence; **causal inference over real-world evidence** is a strong family this blind pass could not responsibly develop because this stream's provenance and Day 1 searches give it no independent grounding (named explicitly: its absence reflects this stream's search allocation, not an assessment of weakness; cross-review should treat it as a genuine candidate blind spot); **human-AI teaming evaluation** (measuring clinician-plus-system performance rather than system performance, anchored by the automation-bias RCT) emerged on Day 1 as a serious adjacent direction and is flagged for cross-review rather than developed, since one day's search cannot establish its landscape.

## D. Intellectual-interest note

The user's stated interests in neuro-symbolic AI and artificial metacognition are treated as tie-break signals only. C1 is a concrete neuro-symbolic instance under the current medical NeSy framing (symbolic evidence structures constraining neural generation; LIT-027), and C3 is literal machine metacognition (a model of the system's own reliability governing action). Both connections are noted after each direction's scientific case was made on evidence, and neither would rescue its direction if Day 2 falsifies the gap: C3 in particular carries the portfolio's weakest resilience despite being the best metacognition fit, and its verdict reflects the science, not the interest.

## E. Stopping-condition statement

Four directions are specified to the required schema with primary-page-verified sources, dangerous prior art named per direction, and Day 2 falsification targets identified (LINS full text and commercial systems for C1; LIT-015, ChemoTimelines successors, and long-context abstraction for C2; MedAbstain and MedVAL full texts for C3; Labbe 2026 and any decomposition line for C4). Additional Day 1 search is unlikely to change which directions deserve adversarial review. No global novelty claim is made or implied for any direction.

---

**Provenance restated:** this file is a format-normalized derivative of the frozen blind first pass at `analysis/analysis_03/day1_candidate_generation.md` (scientific freeze commit `ec538e9`; that file's scientific content is unchanged since the freeze, with metadata corrected on 2026-08-31 in commit `0c7d2f6`). Scientific content, candidate identities, theses, aims, evidence interpretations, verdicts, and portfolio conclusions are unchanged. No new sources, searches, or scientific reasoning were introduced. Chain: scientific freeze → format-normalized derivative → metadata-only correction → final provenance clarification.
