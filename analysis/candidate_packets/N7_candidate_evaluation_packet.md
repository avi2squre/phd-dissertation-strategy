# N7 Candidate Evaluation Packet

- **Candidate identifier:** N7
- **Candidate title:** Measurement-Error-Aware Clinical Natural Language Processing Evaluation
- **Packet version:** Draft 0.1
- **Packet-set version:** Draft 0.1
- **Packet status:** **DRAFT — FIDELITY REVIEW REQUIRED**
- **Date drafted:** 2026-09-01
- **Scientific source/base repository commit:** `5bbbdcbb10c6c810fc6bd2c4203e9dd2fc0e54fa`
- **Packet drafting base commit:** `8e5647c8391ea95dd7ae43f215137f923909ed9a`
- **Source normalization artifact:** [`analysis/round3_normalization_reconciliation.md`](../round3_normalization_reconciliation.md)
- **Constituent Day 1 artifact and section:** `analysis/analysis_03/day1_candidate_generation_v2.md` C4
- **Approval record:** Pending independent packet-fidelity audits and user approval
- **Packet fingerprint location:** packet-set manifest

This packet defines the common N7 target for later Phase 1 review. It performs no new external research and makes no scientific-survival judgment.

## 1. Central scientific object

A **measurement-error model and corrected inference framework for clinical natural-language-processing evaluation**, comprising:

- decomposition of reported error into true system error and measurement artifacts;
- estimators for artifact sources such as surface-form mismatch, ontology granularity, label noise, span/token scoring, and judge bias;
- uncertainty-aware inference about system comparisons or rankings;
- a corrected evaluation protocol and toolkit;
- validation of the corrected instrument against expert adjudication.

The primary scientific phenomenon is error in the evaluation instrument—the ruler—not the clinical system being measured.

## 2. Exact falsifiable thesis

> A substantial and quantifiable fraction of reported error in standard clinical extraction and normalization evaluations is measurement artifact rather than true system error; a semantically valid, noise-aware evaluation methodology that estimates and propagates those artifacts will change at least some system rankings or accepted substantive conclusions while agreeing with expert adjudication better than standard metrics at a defensible cost.

The thesis is defeated or materially weakened if:

- artifact fractions are too small to alter conclusions of practical interest;
- proposed corrections do not improve agreement with expert adjudication;
- corrected rankings are unstable, arbitrary, or more biased than standard metrics;
- a published clinical evaluation framework already performs the same multi-source error decomposition, uncertainty propagation, and validation;
- the work reduces to ontology-aware matching or relabeling rather than a general measurement/inference contribution;
- the scientifically defensible scope supports only one audit paper and no coherent dissertation-scale extension.

## 3. Included scientific scope

The common Phase 1 target includes:

1. Clinical extraction, normalization, linking, summarization, or other structured-output tasks where the evaluation instrument can misclassify semantically acceptable outputs.
2. Explicit decomposition of at least several measurement-artifact sources, including surface form, boundary/tokenization, ontology granularity, label error, and human or language-model judge bias where applicable.
3. Estimation of artifact fractions and uncertainty rather than merely listing error examples.
4. Noise-aware or measurement-error-aware inference for system comparisons, significance, uncertainty, and ranking stability.
5. Corrected metrics or protocols whose validity is tested against blinded expert adjudication rather than assumed.
6. Re-evaluation of existing systems or benchmark conclusions to determine what changes and what remains robust.
7. Comparison with exact match, token/span alternatives, hierarchy-aware or semantic metrics, label-error correction, and language-model judging.
8. Analysis of annotation burden, validity gain, and reproducibility.
9. Transfer to more than one clinical task or explicit boundary conditions explaining where the instrument applies.

## 4. Explicitly excluded scientific scope

The following are not part of N7's mandatory identity:

- Building a new clinical prediction, extraction, or generation model as the primary contribution.
- Generic benchmark criticism without an estimable measurement model and validated correction.
- Ontology-aware or semantic matching alone.
- Label cleaning alone.
- Language-model judge evaluation alone.
- Correcting one dataset's labels without a transferable methodology.
- Process-level agent failure attribution; that is N4a.
- Versioned continual assurance; that is N4b, although N7 methods may address judge drift or measurement noise within it.
- Diagnostic trajectory modeling; that is N2, although N7 methods may improve N2's metrics.
- A requirement that every corrected metric change leaderboards; a robust null result may remain scientifically informative but could weaken dissertation-scale scope.
- A claim that expert adjudication is error-free.

## 5. Constituent Day 1 formulations and relationship

| Constituent candidate | Contribution retained | Role in normalized target | Contribution not made mandatory |
|---|---|---|---|
| S03-C4 — Measurement Error in Clinical Natural Language Processing Evaluation | Artifact decomposition; noise-aware ranking inference; corrected protocol/toolkit; expert validation; re-evaluation of published conclusions | Complete scientific source for the normalized singleton | One specific phenotype corpus, named metric, or error fraction threshold as a universal requirement |

N7 interfaces with N2 and N4 because they need valid evaluation instruments, but it remains distinct because measurement error is the primary phenomenon and thesis.

## 6. Provisional coherent aims

| Aim | Scientific question | Methodological function | Thesis clause tested | Expected evidence |
|---|---|---|---|---|
| Aim 1 — Quantify measurement artifacts | What fraction of apparent system error on representative clinical natural-language-processing benchmarks is attributable to surface form, granularity, label noise, boundary/scoring choice, or judge bias? | Stratified expert re-adjudication, artifact taxonomy, sampling design, and uncertainty estimation | A material, measurable artifact fraction exists | Artifact-fraction estimates with confidence intervals; task-specific patterns; evidence about whether standard scores misrepresent performance |
| Aim 2 — Correct evaluation and propagate uncertainty | Can corrected metrics and measurement-error-aware inference improve system comparison and reveal which rankings or claims are robust? | Develop estimators, semantic/hierarchical credit, noise propagation, and ranking-confidence methods | Correction changes or strengthens substantive conclusions in a principled way | Validated corrected scores, ranking stability/fragility estimates, and re-analysis of canonical comparisons with uncertainty |
| Aim 3 — Validate the instrument and its cost | Do corrected evaluations agree with blinded expert judgment better than standard metrics, and at what annotation or computational cost? | Independent adjudication, preference/validity studies, and cost-performance analysis | The new instrument is more valid rather than merely different | Higher expert agreement or construct validity at a defensible burden, plus explicit failure boundaries across tasks |

## 7. Decisive or discriminating experiment

- **Experimental unit:** a stratified sample of system-output versus reference-label disagreements from one or more public clinical extraction/normalization benchmarks.
- **Strongest comparator:** standard exact match or canonical task score, plus the strongest existing semantic/hierarchy-aware metric and label-error correction available for that task.
- **Primary thesis-relevant outcomes:** estimated artifact fraction with uncertainty, change in system comparisons/rankings, agreement with blinded expert adjudication, and validity gain per annotation/computation cost.
- **Supporting result pattern:** a material fraction of apparent errors are measurement artifacts; corrected evaluation changes at least one consequential conclusion or substantially improves confidence in robust conclusions; and expert agreement improves over strong existing metrics.
- **Defeating result pattern:** artifact fractions are small or immaterial; existing hierarchy-aware/semantic methods already solve the problem; corrected methods do not improve expert agreement; or the work cannot extend coherently beyond one audit.

## 8. Inherited dangerous prior art

These sources are inherited starting points and require independent Phase 1 inspection.

| Source identifier | Source | Why dangerous | Prior inspection depth | Exact unresolved collision question |
|---|---|---|---|---|
| Unregistered, DOI `10.1186/s13326-017-0173-6` | CUILESS2016 | Quantifies disagreement between exact and hierarchical concept-normalization judgments | Day 1 source/abstract characterization | Does it already provide a general artifact-decomposition or only document agreement differences? |
| Unregistered, ACL `2023.acl-long.549` | Wang et al. 2023, medical-summarization metric evaluation | Reports disagreement or anti-correlation between automated metrics and human judgments | Day 1 source characterization | Does it contain a correction/inference methodology that generalizes beyond summarization? |
| Unregistered, arXiv `2410.05046` | Abdul et al. 2024, token-versus-span clinical named-entity-recognition scoring | Demonstrates metric-choice rank reversals | Day 1 abstract/page characterization | Does it already formulate measurement error and ranking uncertainty at dissertation-relevant depth? |
| Unregistered, arXiv `2103.14749` | Northcutt et al., benchmark label errors/confident learning | General machine-learning foundation for label-error effects on rankings | Day 1 source characterization | Can established confident-learning machinery directly solve the clinical structured-output problem? |
| Unregistered, arXiv `2604.16383` | DeLucia et al. 2026, language-model judges versus clinicians | Direct evidence of judge unreliability and reason disagreement | Day 1 abstract/page characterization | Does it already provide a validated correction or only characterize failure? |
| Unregistered, arXiv `2503.10694` | Alaa et al. 2025, construct validity in medical language-model benchmarks | Conceptual framing and proof-of-concept for benchmark validity | Day 1 abstract characterization | Does the framework already subsume N7's proposed instrument science? |
| Unregistered, ACL `2026.bionlp-1.5` | Labbe et al. 2026, hierarchy-aware phenotype-linking evaluation | Direct clinical hierarchy-aware scoring framework | Day 1 page/abstract characterization | Is N7 novel beyond adding several known corrections to this framework? |
| Unregistered | Köhler et al. 2009 and Human Phenotype Ontology semantic-similarity tradition | Mature ontology-aware evaluation machinery | Day 1 source-family characterization | Does semantic similarity already solve the granularity component sufficiently? |
| Unregistered | Groza et al. phenotype concept-recognition evaluation suite | Reported evaluation instability and error-pattern observations | Prior Stream 03 analysis | Does the source already contain the proposed decomposition or supply only motivating observations? |
| Source family | Measurement-error models, psychometrics, metrology, latent-class models, noisy-label inference, annotator models, benchmark statistics | Parent disciplines may already provide the central decomposition and corrected-ranking methods | Not comprehensively searched on Day 1 | Is N7 a clinical packaging of mature measurement methodology without an independent contribution? |

## 9. Known critical uncertainties

| Uncertainty | Relevant kill test | Why decision-relevant | Current evidence state |
|---|---|---|---|
| Whether a published clinical evaluation methodology already combines multi-source artifact decomposition, uncertainty-aware ranking, and expert validation | KT1 | Could directly preempt the central object | Day 1 search found components but was not saturated |
| Whether artifact fractions are large enough to change meaningful conclusions | KT3/ST1 | A small phenomenon could reduce the direction to one audit paper | Central designated early pilot; unresolved |
| Whether expert adjudication supplies a sufficiently valid reference standard | KT3 | The new ruler must itself be measured | Unresolved; blinded and multi-rater design is proposed |
| Whether strong semantic/hierarchy-aware metrics are practically equivalent | KT4 | Equivalent simpler methods would remove need for a complex framework | Unresolved |
| Whether the decomposition can identify artifact sources rather than simply relabel disagreements | KT3 | Latent true error may be unidentifiable | Requires explicit sampling and adjudication model |
| Whether the direction is dissertation-sized rather than one strong methods paper | ST1/KT2 | The most prominent Day 1 rejection argument | Unresolved; cross-task transfer and instrument validation are proposed extensions |
| Whether the method generalizes beyond one task and ontology | ST2 | Narrowness could make it application-bound | Proposed but untested |
| Whether clinicians and reviewers value instrument science sufficiently for coherent execution and validation | KT5 | Expert time and methodological support are required | Plausible but no commitment inferred |

## 10. Feasibility assumptions inherited from Day 1

- Public clinical extraction, normalization, phenotype-linking, and summarization benchmarks provide system outputs and reference labels suitable for retrospective audit.
- A stratified expert-adjudication sample can be obtained at a bounded scale; no individual commitment is inferred.
- Existing semantic, ontology-aware, noisy-label, and language-model-judge methods can be implemented or reused as strong baselines.
- The first artifact-fraction audit can be conducted without protected clinical data.
- Hierarchical bootstrap or related uncertainty methods are computationally feasible.
- Re-evaluation across at least two task types is plausible, but dissertation-scale breadth remains to be tested.

## 11. Packet provenance and change control

### Direct compressions

- The scientific object, exact thesis, artifact categories, aims, decisive pilot, dangerous sources, rejection case, and critical uncertainty are compressed from S03-C4.
- The distinction between studying the evaluation instrument and studying the system is preserved directly.

### Reconciled formulations

- The packet requires both changed conclusions and improved expert validity so that a merely different score cannot satisfy the thesis.
- It avoids treating any provisional one-quarter artifact threshold from Day 1 as a universal requirement; Phase 1 must justify practical significance prospectively.

### Unresolved candidate-definition tension

The original thesis contains both `a substantial artifact fraction` and `changes at least one accepted substantive conclusion`. Fidelity reviewers should determine whether both are mandatory or whether either could independently sustain the dissertation. They should also assess whether clinical summarization belongs in the common scope or should remain an optional transfer task.

### Change control

This draft may be revised only during packet-fidelity review. Once approved and Phase 1 begins, material changes require user approval, a new packet-set version, and a comparability assessment for completed scans.
