# Common Analysis Schema v2

## Purpose

This document standardizes the structure of independent dissertation-direction analysis artifacts so that different analysis streams remain scientifically independent while producing outputs that are directly comparable.

The schema standardizes **presentation, evidentiary labeling, triage terminology, and required fields**. It does **not** require agreement among streams, prescribe scientific conclusions, impose canonical rankings, or replace `OPERATING_PROTOCOL.md`, `decisions/`, or the candidate-definition rules.

A stream may disagree strongly with every other stream while still conforming to this schema.

## Terminology

Use the following terms consistently:

- **Dissertation research direction**: the primary scientific unit being generated and compared.
- **Candidate dissertation direction**: a direction still under consideration.
- **Finalist dissertation direction**: one of the eventual directions selected for faculty discussion.
- **Research family**: a broader methodological area from which multiple dissertation directions may arise.
- **Dissertation topic**: acceptable shorthand.
- **PhD program**: reserved for an academic degree/program at a university.

Do not use **research program** to mean a dissertation direction.

## Version history and Day 1 provenance

- **v1.0**: original Day 1 common specification frozen before blind candidate generation.
- **v1.1 clarification**: made the existing canonical advisor constraint explicit: a plausible University of Minnesota IHI primary advisor plus Dr. Rui Zhang as a complementary/external advisor. This clarification changed no scientific selection criterion.
- **v1.2 clarification**: standardized the four Day 1 verdict meanings. This clarification changed no scientific selection criterion.
- **v2**: standardizes the common presentation schema using useful structural features observed across the three independently produced Day 1 artifacts. v2 is a **format normalization**, not a license to revise frozen Day 1 analyses.

When a previously frozen artifact is reformatted into v2, its scientific content, candidate definitions, claims, evidence interpretation, aims, verdicts, and portfolio conclusions must remain unchanged. Any post-freeze analytical reconsideration belongs in a new cross-review or later-round artifact.

---

# Layer I — Executive navigation

Every analysis artifact should begin with the following metadata.

## A. Analysis metadata

Record:

- date;
- analysis-stream identifier;
- repository SHA used;
- analysis status;
- permitted repository inputs;
- deliberately excluded inputs;
- external-search scope;
- independence disclosures;
- use of parallelism, if any, and its methodological justification;
- stopping condition.

For blind first-pass work, use the status:

**FROZEN — BLIND FIRST PASS**

Once frozen, the scientific content of that first pass is immutable. Later reconsideration belongs in a separate artifact.

## B. Repository-convention declarations

State briefly:

1. the question evaluated;
2. evidence used;
3. key assumptions;
4. recommendation and uncertainty status;
5. whether other analyses were consulted;
6. whether any accepted decision is being challenged or reconsidered.

## C. Candidate overview table

Before the detailed analyses, provide a compact navigation table:

| ID | Candidate dissertation direction | Central scientific object | Day 1 verdict | Critical uncertainty / rejection trigger |
|---|---|---|---|---|

This table is a **map**, not an ordinal ranking.

Do not rank candidates first/second/third during blind Day 1 analysis.

---

# Layer II — Full candidate analysis

Each candidate dissertation direction must contain the following 22 sections in this order.

## Scientific definition

### 1. Candidate identity

Provide:

- a concise descriptive title;
- a one-sentence identity explaining exactly what the direction studies.

Avoid umbrella-only labels such as `neuro-symbolic AI`, `agentic AI`, or `trustworthy AI` without a specific scientific object.

### 2. Central scientific object

Name the principal methodological object the dissertation would contribute or study, such as:

- representation;
- controller;
- algorithm;
- inference framework;
- learning objective;
- formal contract;
- evaluation instrument;
- benchmark methodology;
- causal method;
- verification mechanism.

This section is intended to expose directions whose novelty rests only on combining fashionable technologies.

### 3. Central scientific problem

State the unresolved methodological/scientific problem and explain why it matters.

### 4. Falsifiable dissertation thesis

State one central thesis that could, in principle, be shown wrong.

Apply the coherence test:

> Are the proposed aims different tests of one thesis, or several attractive projects placed beside one another?

## Evidence and novelty

### 5. Evidentiary basis

For important premises, use:

`claim -> source(s) -> evidentiary status`

Prefer explicit labels such as:

- **Source-supported finding**
- **Cross-paper inference**
- **Preliminary gap hypothesis**
- **Proposed research hypothesis**
- **Unverified assumption**

Maintain the inferential chain:

`published finding -> observed limitation -> inferred gap -> proposed hypothesis`

Do not make a citation appear to prove a gap or hypothesis that the source itself does not establish.

### 6. Closest and dangerous prior work

Identify the work most likely to overlap with or invalidate the proposed novelty. Include dangerous prior art, not only supportive sources.

### 7. Evidence-supported limitations of existing approaches

Separate:

- limitations explicitly reported by sources;
- limitations inferred by the analysis stream.

### 8. Preliminary research gap

Label explicitly:

**PRELIMINARY GAP HYPOTHESIS — REQUIRES ADVERSARIAL NOVELTY VERIFICATION**

State precisely what appears unresolved. Avoid field-wide absence claims unless a suitably comprehensive search supports them.

## Proposed science

### 9. Proposed methodological contribution

State the new methodological/scientific contribution. Merely integrating existing technologies is insufficient unless the integration itself poses and solves a genuine methodological problem.

### 10. Coherent dissertation aims

Normally propose 2–3 aims. For each aim state:

`question -> method -> experiment -> expected evidence`

The aims should test different aspects of the same central thesis.

### 11. Publication decomposition

Explain how the direction could naturally produce multiple coherent publications, for example:

`measurement/benchmark -> core method -> external validation/generalization`

Do not inflate paper count. State whether failure of a later aim could still leave a defensible dissertation and meaningful publications/artifacts.

### 12. Evaluation strategy

Specify, where applicable:

- datasets or experimental environments;
- strongest meaningful baselines;
- ablations;
- primary metrics;
- robustness/generalization tests;
- appropriate statistical comparisons;
- human evaluation.

## Execution

### 13. Required resources and feasibility

Identify requirements for data, annotations, compute, software infrastructure, collaborators, domain expertise, and restricted versus public resources.

Separate:

- **known available**;
- **plausibly available**;
- **currently uncertain**.

### 14. Novelty-collision risks

Act as the candidate's first skeptic. Identify:

- closest overlapping work;
- likely reviewer objections;
- ways the contribution could collapse into incremental engineering;
- components likely to be commoditized by stronger foundation models.

### 15. Advisor / expertise complementarity

First identify the methodological expertise required by the direction.

Then identify the strongest plausible **University of Minnesota IHI primary-advisor match(es)** using current official public information where appropriate. Dr. Rui Zhang should be treated as the external/complementary advisor.

For each named IHI match, briefly explain:

- what expertise the IHI faculty member contributes;
- what Dr. Zhang contributes;
- why the combination is complementary for this direction;
- any important expertise gap that remains.

More than one plausible IHI primary-advisor option may be listed when the best choice depends on the direction's final framing.

Do not infer willingness, availability, funding, commitment, data access, or final advising eligibility from methodological fit.

### 16. Foundation-model resilience

Assume frontier foundation models become dramatically more capable during the PhD. State what scientific contribution remains. Penalize directions that become uninteresting if base-model reasoning improves routinely.

### 17. Publication and execution risk

Assess qualitatively:

- novelty bar;
- time to first credible publishable unit;
- dependence on one risky experiment;
- ground-truth difficulty;
- reproducibility;
- risk of rapidly moving prior art.

Avoid false numerical precision.

### 18. Generalizability

Distinguish:

- healthcare-specific contributions;
- methodologically transferable contributions.

Do not call healthcare merely a testbed when healthcare-specific structure is integral to the method.

## Falsification and triage

### 19. Strongest reason to reject the direction

Give the strongest substantive argument for not pursuing it. This section should be adversarial, not ceremonial.

### 20. Evidence that would change the recommendation

Specify what evidence would:

- substantially strengthen the direction;
- substantially weaken the direction;
- kill the direction outright.

### 21. Day 1 verdict and verdict rationale

Choose exactly one standardized verdict from the definitions below, then provide a **2–4 sentence verdict rationale** explaining why the current evidence warrants that status.

### 22. Critical uncertainty / rejection trigger

Provide one concise statement identifying the single unresolved issue most capable of changing the verdict or causing the direction to be rejected.

This field should directly inform the next adversarial research task.

---

# Standardized verdict definitions

## ADVANCE

**Definition:** Current evidence clearly justifies substantial next-round adversarial investigation. No presently identified scientific, novelty, feasibility, coherence, or execution problem makes the direction obviously unsuitable.

Operational meaning: **worthy of serious next-round scrutiny**.

`ADVANCE` does not mean selected dissertation direction, finalist, proven novel, faculty recommendation, or ordinal rank.

## ADVANCE WITH MAJOR UNCERTAINTY

**Definition:** The direction is sufficiently promising to justify next-round adversarial investigation, but at least one identified uncertainty could materially weaken or eliminate it.

The critical uncertainty must be named explicitly.

Operational meaning: **investigate this direction, but attack the named weak point first**.

## HOLD

**Definition:** The direction remains scientifically plausible and worth preserving, but current evidence does not justify allocating it equal next-round effort unless cross-stream evidence or targeted research materially strengthens it.

Operational meaning: **preserve, but do not prioritize yet**.

`HOLD` is not rejection.

## DO NOT ADVANCE

**Definition:** A substantive scientific, novelty, feasibility, coherence, or execution problem currently makes further routine investigation unjustified. Reopening requires materially new evidence rather than another favorable opinion.

Operational meaning: **stop routine investment unless genuinely new evidence changes the state**.

---

# Layer III — Portfolio-level analysis

After all candidate directions, provide the following.

## A. Candidate diversity check

State whether the candidates are genuinely distinct scientific directions. If two are variants of the same thesis, say so.

## B. Qualitative scientific comparison matrix

Use a table with candidates as columns and at least these dimensions as rows:

- scientific importance;
- methodological depth;
- falsifiability / discriminating experiment;
- preliminary novelty headroom;
- publication tractability;
- empirical feasibility;
- time to uncertainty resolution;
- artifact/reuse potential;
- foundation-model resilience;
- IHI advisor/resource feasibility;
- transferable technical depth;
- largest unresolved uncertainty.

Use qualitative judgments. Do not impose ordinal ranking or false numerical precision during blind first-pass analysis.

## C. Missing-direction check

Ask:

> What strong scientific direction might this analysis have overlooked because of anchoring on historical repository discussions or the search allocation used in this pass?

Omission is not evidence of weakness. Name serious blind spots explicitly.

## D. Intellectual-interest note

Personal intellectual interests may be treated as positive tie-break signals, but they must not rescue weak science or displace substantially stronger directions.

## E. Stopping-condition statement

State why additional work in the current round is unlikely to change which directions deserve the next stage of investigation.

---

# Scientific matrix versus private strategic matrix

The Layer III comparison above is a **scientific/research-viability matrix**.

Broader private strategic criteria belong in a separate internal analysis layer after scientific viability has been established sufficiently. Examples may include publication/citation upside, reusable-artifact adoption potential, transferable skill development, broader labor-market portability, commercialization potential, externally visible independent contribution potential, and other private strategic considerations permitted by DEC-006.

Do not silently mix the private strategic matrix into the scientific comparison matrix.

---

# Reformatting frozen artifacts into v2

When an existing frozen analysis is normalized to this schema:

1. Preserve the original frozen artifact or its commit/hash as provenance.
2. Do not perform new literature searches or new scientific reasoning.
3. Do not change candidate identity, thesis, aims, evidence interpretation, verdict, or portfolio conclusions.
4. Reorder or relabel existing material only where necessary to match v2.
5. Populate `Central scientific object`, `Verdict rationale`, and `Critical uncertainty / rejection trigger` only by extracting or faithfully compressing reasoning already present in the frozen artifact. Do not invent new analysis.
6. If a required v2 field is genuinely absent from the original artifact and cannot be derived without new reasoning, mark it **NOT PRESENT IN ORIGINAL FROZEN ARTIFACT** rather than filling the gap analytically.
7. Record that the v2 artifact is a **format-normalized derivative** and cite the original frozen artifact/hash/commit.
8. Never overwrite the original Day 1 scientific provenance silently.

The purpose of normalization is structural comparability, not retrospective convergence.
