# 2026-08-26 to 2026-08-30 — Multi-stream provenance and research governance

## Historical role

This entry reconstructs the evolution of the project from an informal idea for sharing conversations across analysis systems into a version-controlled, provider-neutral research-governance workflow.

The mature workflow did not exist at the beginning. It emerged through repeated corrections to earlier assumptions about synchronization, repository access, provenance, write discipline, and model independence.

## Initial shared-memory idea

The user proposed using GitHub so multiple analysis systems could read each other's dissertation recommendations and remain synchronized.

Stream 01's first major reframing was:

> GitHub should not merely be a shared transcript folder. It should be the canonical, version-controlled project state.

The proposed repository therefore separated:

- context and constraints;
- candidate programs;
- evidence;
- discussion archives;
- independent analyses;
- accepted decisions;
- scoring frameworks;
- current rankings;
- source records.

Raw discussions were treated as provenance rather than canonical conclusions.

## Preserve disagreement rather than force convergence

A central design principle emerged early:

**Independent analyses should not automatically converge.**

The value of multiple systems was argued to lie partly in disagreement. If two analyses rank a candidate very differently, the correct response is not to average the rankings mechanically. Instead, identify the assumptions or evidence causing the divergence and investigate those.

This produced working states such as:

- consensus;
- provisional consensus;
- open disagreement;
- unresolved evidence need.

Later, the workflow added an explicit rejected/undermined state for claims defeated by evidence or critique.

## Candidate-definition and decision-history discipline

The earlier advisor-ranking error directly influenced repository rules:

- do not silently change candidate definitions during scoring;
- create a new candidate when the scientific object materially changes;
- do not silently rewrite accepted decisions;
- record new evidence, challenge, replacement rationale, and status;
- preserve historical reasoning so later analyses can inspect why a weight or decision exists.

The repository therefore became not only a storage layer but an audit trail for research-strategy evolution.

## Neutral discussion streams

The repository adopted neutral numbered discussion and analysis streams so the public structure did not depend on a specific provider or tool.

The mapping between providers and stream numbers is intentionally kept outside the repository.

This made the architecture portable while also reducing the risk that later reviewers anchor on provider identity rather than reasoning quality.

## GitHub and portable internal strategy became separate layers

A second architectural distinction emerged:

- **GitHub:** canonical research state, evidence, provenance, decisions, analyses, disagreements, and eventual faculty-facing materials.
- **Portable internal strategy document:** compact cross-platform statement of broader private objectives and evaluation criteria.

The internal strategy document is context, not scientific evidence, and does not replace the reasoning history preserved in GitHub.

This separation supported the two-layer rule established in the faculty-meeting discussion: broad internal optimization may guide candidate selection, while faculty-facing materials remain primarily scientific.

## Why provenance became a first-class requirement

The user explicitly asked whether the methodology would preserve the series of discussions that led to conclusions.

Stream 01 then articulated four layers:

1. **Discussion archive** — arguments, objections, mistakes, and revisions.
2. **Independent analysis** — a manageable interpretation of the discussion and evidence.
3. **Decision log** — accepted project state and rationale.
4. **Evidence base** — sources that allow claims and decisions to be checked.

The key insight was that a decision such as "advisor-team advantage gets modest weight" is less useful without the argumentative path that produced it.

## Capability and repository-access corrections

The initial GitHub setup produced several incorrect or incomplete diagnoses about why a private repository was inaccessible. Tool permissions, account-level authorization, repository visibility, and connector installation were at first conflated.

The consequential lesson was not the click-by-click troubleshooting. It was:

> Claims about connected-system capabilities should be verified empirically rather than inferred from UI state or assumed authorization layers.

Once access was actually confirmed, Stream 01 initialized the repository directly.

This correction is preserved because it later influenced the stronger verification discipline used for branch state, commit SHAs, checksums, and post-write validation.

## Stream reconstruction exposed provenance failure modes

When another discussion stream was reconstructed, a dissertation concept labeled "Direction A / A1–A4" was initially supported only by fragmentary and secondhand traces. A conversation title had been transcribed from an embedded screenshot, and the full primary-source discussion was not initially available.

The original conversation was later recovered. That resolved the provenance gap and established the historical A1–A4 formulations directly.

### Governance lesson

This episode reinforced:

- screenshot fragments are useful provenance but may be incomplete;
- compressed summaries are not authority;
- exact historical claims should escalate to primary sources when disputed;
- retrospective synthesis must not rewrite another stream's original reasoning;
- another stream's critique should remain separate until the deliberate cross-review stage.

These ideas were later formalized in the operating protocol.

## Frontier-model efficiency protocol

Repeated large-corpus rereads and multi-agent extraction runs revealed a second problem: significant model computation could be spent remembering the project rather than advancing the research.

The project therefore adopted a provider-neutral operating protocol, later made canonical through DEC-008.

Its central principles included:

- progressive context retrieval;
- no full-repository reread by default;
- no routine rereading of raw historical exports once structured provenance is adequate;
- one strong reasoning process plus targeted retrieval by default;
- parallel agents only when methodological value justifies them;
- separate deep reasoning from deterministic execution;
- preserve stream independence;
- reuse source records without inheriting interpretations;
- escalate to primary sources when compression is insufficient or disputed;
- scale computation with decision consequence;
- stop when additional computation is unlikely to change the next scientific action, conclusion, confidence level, or identified uncertainty;
- require human checkpoints for consequential canonical changes.

The optimization target was summarized as:

**fewer tokens spent remembering the research; more frontier compute spent doing the research.**

## Write workflow matured through Stream 02/03 experience

The earliest repository work allowed direct writes to canonical state more readily.

The workflow later became stricter:

research/provenance reconstruction
→ isolated review branch or local candidate commit
→ deterministic validation
→ review artifact / diff inspection
→ explicit human approval
→ canonical integration
→ post-integration verification

This change is itself part of the provenance. The mature review-branch workflow should not be projected backward as though it existed from the beginning.

## Final three-stream intellectual workflow

By the end of this period, the intended brainstorming architecture was:

### 1. Neutral task specification

Formulate one bounded scientific question and give the same specification to each independent analysis stream.

### 2. Blind independent candidate generation

Each stream proposes a small number of coherent dissertation programs without first reading the other streams' conclusions.

A candidate should specify, where relevant:

- central scientific problem;
- falsifiable thesis;
- methodological contribution;
- why existing approaches are insufficient;
- coherent aims;
- required data/resources;
- evaluation strategy and baselines;
- closest literature and novelty risks;
- advisor/resource feasibility;
- plausible publication decomposition;
- generalizability.

### 3. Candidate normalization

Determine whether differently named proposals are genuinely distinct scientific programs or variants of the same underlying object. Merging candidates is itself a decision and should preserve provenance.

### 4. Adversarial falsification

Instead of asking systems to find support for a favored candidate, assign explicit attempts to defeat it, for example:

- find prior art that makes the novelty incremental;
- attack conceptual coherence;
- attack experimental tractability and reproducibility.

### 5. Evidence update and candidate revision

New literature or empirical evidence should modify candidates transparently rather than silently polishing them until they survive criticism.

### 6. Independent scoring after candidate freeze

Only stable candidate definitions should be scored. Large score disagreements should trigger investigation of assumptions, not arithmetic averaging.

### 7. Cross-review

After independent first-pass analyses are complete, each stream reads the others and identifies:

- the strongest argument it missed;
- the weakest external argument;
- whether its own conclusion should change and why.

### 8. Reconciliation

Important propositions may be classified as:

- consensus;
- provisional consensus;
- open disagreement;
- rejected/undermined.

Where disagreement depends on an empirical uncertainty, the preferred resolution is new evidence or an experiment, not more rhetoric.

### 9. Faculty as an additional epistemic layer

Faculty input is treated as new evidence about information that models may not possess reliably, including:

- unpublished or emerging lab work;
- realistic supervision interests;
- data and infrastructure access;
- collaborator constraints;
- funding context;
- local novelty judgments;
- what can realistically yield an early paper.

Faculty review is therefore not ceremonial approval of an AI-generated answer.

### 10. Minimum viable research probes

For the final few directions, small empirical prototypes should replace indefinite theoretical debate when possible. The objective is to test whether the central construct can be operationalized, whether useful signal exists, whether baselines are available, and whether the purported gap survives implementation.

## Orchestration versus epistemic authority

The project distinguished operational coordination from scientific authority.

One analysis system may coordinate task formulation, cross-review, repository discipline, and synthesis logistics, but it should not become the intellectual authority whose framing the other systems merely inherit.

The user remains the final decision-maker, with faculty judgment and empirical evidence capable of overriding any model recommendation.

## Stopping rule for multi-model analysis

A practical stopping rule was added to prevent analysis loops:

**three independent analyses → cross-review → unresolved disagreement → obtain new evidence, ask faculty, or run an experiment.**

The project should not respond to uncertainty by indefinitely adding prompts, rankings, and models that consume computation without changing the next scientific action.

## Status at the end of this episode

By 2026-08-30:

- the provider-neutral repository architecture was established;
- two other discussion streams had been reconstructed and marked complete enough for cross-stream analysis;
- the operating protocol and human-review workflow were in force;
- Stream 01 reconstruction was the remaining prerequisite before deliberate three-way cross-stream analysis.

The governance system is therefore itself a product of iterative correction rather than an initial fixed design.