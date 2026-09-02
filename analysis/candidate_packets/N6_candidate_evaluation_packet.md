# N6 Candidate Evaluation Packet

- **Candidate identifier:** N6
- **Candidate title:** Adequacy- and Currency-Aware Clinical Claim Verification
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifact and section:** `analysis/analysis_03/day1_candidate_generation_v2.md` C1
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N6 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **typed, claim-level clinical evidence-verification calculus** that distinguishes at least four dimensions:

- evidential support;
- methodological adequacy or quality of the supporting evidence;
- temporal currency, including supersession and retraction;
- applicability to the relevant patient, population, or clinical context.

The dissertation object also includes an expert-annotated multidimensional benchmark, a calibrated verifier that produces dimension-specific judgments, and an evaluation method for determining whether these judgments change measured system reliability and inference-time behavior.

## 2. Exact falsifiable thesis

> A verifier that explicitly models evidence adequacy and temporal currency, alongside support and patient applicability, will detect clinically significant mis-supported claims that entailment-only support checking systematically misses at rates large enough to change the measured reliability ranking of clinical question-answering or generation systems; enforcing multidimensional verification at inference time will improve clinically weighted reliability at an acceptable coverage or action-cost penalty.

The thesis is defeated or materially weakened if:

- adequacy and currency failures are rare once entailment support passes;
- entailment-only or generic language-model verifiers capture the same failures incidentally;
- experts cannot label the dimensions reproducibly;
- study-quality or patient-applicability judgments cannot be operationalized at claim level;
- enforcement reduces coverage or increases cost without clinically meaningful reliability gain;
- an existing academic or commercial system already provides an expert-validated multidimensional claim-evidence benchmark and calibrated verifier with comparable enforcement evaluation.

## 3. Included scientific scope

The common Phase 1 target includes:

1. Claim-level decomposition of clinical artificial-intelligence output and its supporting evidence.
2. Separate judgments for support, methodological adequacy, temporal currency, and patient/population applicability.
3. Explicit representation of evidence hierarchy, study design or risk-of-bias signals, retraction/supersession, versioned guidance, and context constraints where feasible.
4. Composition rules for situations involving multiple sources, conflicting evidence, weak evidence, or outdated evidence.
5. An expert-annotated benchmark with per-dimension labels, uncertainty, and adjudication.
6. A calibrated verifier whose errors can be analyzed by dimension.
7. Comparison with entailment-only citation checking, generic language-model judging, retrieval/citation pipelines, and dimension-specific tools.
8. Perturbation tests using planted unsupported, weak, superseded, retracted, or inapplicable evidence.
9. Evaluation of whether verifier enforcement changes reliability, coverage, rankings, or clinically weighted risk.
10. Publicly reproducible core resources where licensing and redistribution permit.

## 4. Explicitly excluded scientific scope

The following are not part of N6's mandatory identity:

- A general controller choosing among answer, retrieve, ask, revise, or defer; that is N1, although N6 outputs may serve as N1 signals.
- Generic retrieval-augmented generation or citation generation without multidimensional evidence appraisal.
- A claim that one evidence hierarchy applies uniformly to all clinical questions.
- Automated systematic-review production as the primary task.
- A requirement to solve every risk-of-bias instrument or clinical-guideline domain.
- A guarantee that evidence appraisal alone establishes clinical truth or treatment appropriateness.
- Measurement-error science as the primary thesis; that is N7, though N7 methods may audit this benchmark.
- A product comparison or commercial-system survey as a substitute for methodological novelty.
- Merely combining existing support checker, retraction detector, and risk-of-bias classifier without new formalization, calibration, or evaluation.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S03-C1 — Adequacy-Aware Verification of Clinical Artificial-Intelligence Claims | Four-dimensional claim-evidence relation; expert benchmark; calibrated verifier; inference-time enforcement; neuro-symbolic evidence structures | Complete scientific source for the normalized singleton | One particular medical question-answering system, evidence repository, rare-disease application, or agent architecture |

N6 is distinct from N1. Its verifier can supply N1 with evidence-state signals, and its currency dimension may share temporal-validity semantics with N1, but N6 has an independently testable formalism, benchmark, and verification thesis.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Formalize and measure multidimensional evidence failure | How often do apparently supported clinical claims fail adequacy, currency, or applicability, and can experts label those dimensions reliably? | Define relation schema, composition rules, annotation protocol, benchmark, and perturbation sets | Important failure mass exists beyond entailment support and is measurable | Per-dimension prevalence, agreement, construct validity, and evidence that rankings or conclusions change when dimensions are considered |
| Aim 2 — Build and calibrate the verifier | Can an automated or agentic verifier detect the multidimensional failures beyond entailment-only and generic judge baselines? | Retrieve/appraise/date-check/applicability pipeline or unified model; dimension-specific calibration and ablation | Explicit adequacy/currency/applicability machinery adds detection value | Better per-dimension detection and calibration, robustness to planted failures, and ablation evidence isolating each component |
| Aim 3 — Evaluate enforcement consequences | Does gating or revising generation using the verifier improve clinically weighted reliability at acceptable coverage, latency, and workload? | Inference-time enforcement policy and controlled downstream evaluation | Multidimensional verification produces operational benefit rather than only new labels | Improved risk-coverage or reliability trade-offs and changed system rankings, with explicit cost and failure analysis |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a clinical claim paired with one or more cited or retrieved evidence sources and expert multidimensional labels.
- **Strongest comparator:** a strong entailment/support verifier, generic language-model judge, and an end-to-end evidence-grounded medical question-answering system with equivalent source access.
- **Primary thesis-relevant outcomes:** adequacy/currency/applicability failure prevalence after support passes, per-dimension discrimination and calibration, system-ranking stability, clinically weighted reliability, and coverage/action cost under enforcement.
- **Supporting result pattern:** a substantial and reproducible failure mass remains invisible to support-only checking; the proposed verifier detects it with useful calibration; and enforcement changes reliability or rankings at acceptable cost.
- **Defeating result pattern:** additional dimensions are rare, irreproducible, or captured by support-only/generic baselines; an existing system already provides the full contribution; or enforcement yields no practical reliability benefit.

## 8. Inherited dangerous prior art

These sources were identified during Day 1 and must be independently inspected during Phase 1.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| `LIT-024` | Wang et al., *MedCite*, Findings of ACL 2025, DOI `10.18653/v1/2025.findings-acl.967` | End-to-end medical citation generation and evaluation | SCREENED | Does it evaluate only support/citation quality or also adequacy, currency, and applicability per claim? |
| `LIT-025` | Wang et al., *LINS*, Nature Communications 2025, DOI `10.1038/s41467-025-64142-2` | Claims evidence-traceable responses, timeliness, and evidence validity; closest end-to-end academic threat | SCREENED | Does it already implement claim-level quality/currency appraisal and calibrated multidimensional verification? |
| Unregistered, DOI `10.1038/s41467-025-58551-6` | Wu et al., *SourceCheckup* | Large-scale physician-validated claim-level support checking | Day 1 abstract/page characterization | Does its pipeline or error taxonomy already extend beyond support into evidence adequacy? |
| Unregistered, ACL `2023.emnlp-main.398` | *ALCE* | General-domain citation-quality evaluation framework | Day 1 source characterization | Does its metric decomposition subsume the proposed relation schema? |
| Unregistered, arXiv `2605.27710` | *DeepSciVerify* | Claim-citation alignment with evidence escalation | Day 1 abstract characterization | Does escalation include evidence quality and temporal validity or only support? |
| Unregistered, arXiv `2507.02975` | *Answered with Evidence* | Couples generation with evidence-foundedness scoring | Day 1 abstract characterization | Does it implement a comparable multidimensional verifier and enforcement study? |
| Unregistered, arXiv `2511.03048` | *ROBoto2* | Automates risk-of-bias or evidence-quality assessment | Day 1 abstract/page characterization | Can its adequacy machinery be directly repurposed at claim level, reducing N6 to integration? |
| Unregistered, arXiv `2502.15429` | *Pub-Guard-LLM* | Retraction/currency detection | Day 1 abstract characterization | Does it already provide a general currency/supersession verifier for generated claims? |
| Unregistered, arXiv `2606.20895` | AlphaNeSy-CTM | Logic-based patient applicability in clinical-trial matching | Day 1 abstract characterization | Does its applicability formalism transfer directly to claim-evidence verification? |
| Unregistered | Commercial evidence-grounded clinical question-answering systems | May already implement practical versions not described fully in papers | Surfaced but not inspected on Day 1 | Is the academic method novel despite commercial implementation, and is sufficient technical evidence accessible? |
| `LIT-001` / `LIT-002` | KGARevion and HEG-TKG or related provenance-grounded verification sources | Demonstrate structured-source verification, revision, and citation/provenance gains | READ in prior Stream 03 work | Do they already cover the proposed verification object beyond support and provenance? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether LINS-class or commercial systems already implement per-claim adequacy and currency verification | KT1 | Could directly preempt the central method and benchmark | Named Day 1 kill target; full technical comparison unresolved |
| Whether adequacy, currency, and applicability are separable, reliable claim-level constructs | KT3 | Poor construct validity would defeat the benchmark and verifier | Proposed formalism only; expert agreement unknown |
| Whether the additional failure mass is large enough to change conclusions or system rankings | KT3/ST1 | A small phenomenon could reduce the direction to one careful study | Unresolved; designated early measurement task |
| Whether a composed pipeline adds methodological science beyond existing component tools | KT1/KT4 | Could be viewed as integration engineering | Composition, calibration, and evaluation are proposed novelty; not yet validated |
| Whether entailment-only or generic judge baselines are practically equivalent | KT4 | Equivalent simpler systems would remove necessity | Unresolved |
| Whether inference-time enforcement improves reliability without unacceptable coverage/workload loss | KT4 | Required by the second thesis clause | Proposed experiment only |
| Whether evidence rules transfer across specialties, question types, and evolving guidance | KT6/ST2 | Could be narrow and brittle | Unresolved; explicit boundary conditions may be necessary |

## 10. Feasibility assumptions inherited from Day 1

- Public sources with version histories, retraction records, guidelines, reviews, and cited medical answers can support an initial benchmark.
- Expert annotation is obtainable at a bounded scale for relation labels and adjudication; no commitment is inferred.
- Risk-of-bias, retraction, evidence-retrieval, and citation-checking tools can serve as components and baselines.
- Public or synthetic perturbations can create known unsupported, outdated, weak, or inapplicable evidence conditions.
- The core benchmark and verifier can be developed without protected clinical records.
- A downstream rare-disease or clinical use case may strengthen evaluation but is optional rather than the sole scientific path.

## 11. Packet provenance and change control

### Direct compressions

- The scientific object, exact thesis, four dimensions, aims, falsification conditions, inherited sources, and critical uncertainty are compressed from S03-C1.
- The distinction between support and adequacy/currency/applicability is preserved directly.

### Reconciled formulations

- The packet treats a substantial failure mass and changed reliability/rankings as necessary evidence so that merely adding labels cannot satisfy the thesis.
- The boundary with N1 preserves verifier-to-controller reuse without collapsing the two directions.

### Unresolved candidate-definition tension

The original formulation emphasizes adequacy and currency most strongly while also including patient applicability and support. Fidelity reviewers should determine whether all four dimensions are mandatory to the common thesis or whether support/applicability should be treated as baseline/context dimensions. Any change must preserve the multidimensional verification identity.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
