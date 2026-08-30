# Restricted Data and Public-Private Boundaries

- **Historical date:** 2026-07-30
- **Archived:** 2026-08-30
- **Primary provenance:** Stream 02 archival PDF, exchanges 6, 8, 9, and 10
- **Nature of record:** public, redacted historical reconstruction
- **Canonical effect:** none

## Why the boundary affected research feasibility

The dissertation strategy depended on producing public methods, reproducible software, and independently inspectable artifacts while some possible validation work would occur in a restricted institutional environment. The archive therefore treated privacy and release constraints as part of scientific feasibility, not as an afterthought.

## Three distinct evidence layers

**Stream 02 recommendation.** Maintain three physically and conceptually separate collections:

1. **Public portfolio:** public code, papers, posters, slides, synthetic demonstrations, and permitted documentation.
2. **Private evidence vault:** training records, original correspondence, feedback, authorship confirmations, submissions, invitations, and internal progress documentation.
3. **Restricted research environment:** PHI, protected datasets, sensitive outputs, restricted code, and any material controlled by institutional policy.

The public repository must not contain PHI, clinical screenshots, patient-level output, rare combinations, small-cell counts, exact protected distributions, restricted schema details, credentials, or sensitive error logs.

## Synthetic-data interface contract

**User-stated proposal.** The user suggested describing permitted formats and abstract schemas so that fictional data could be generated outside the restricted environment for code development.

**Stream 02 recommendation.** This was accepted with an interface-contract workflow:

1. confirm what schema metadata, aggregates, and code may leave the restricted environment;
2. describe permitted structure abstractly rather than copying data dictionaries, screenshots, queries, or patient examples;
3. generate entirely fictional records and edge cases outside the environment;
4. develop schema validation, integrity checks, tests, and pipeline code against the synthetic interface;
5. move only approved code into the restricted environment;
6. run real-data validation there;
7. return only permitted, nonsensitive failure descriptions or interface changes;
8. reproduce the abstract failure condition synthetically without recreating a patient.

Synthetic fixtures could cover negation, experiencer, uncertainty, anatomy, temporality, missingness behavior, relational integrity, and expected model outputs without encoding real prevalence or cases.

## Limits of the synthetic path

**Later correction or qualification.** Synthetic data could validate software correctness, schemas, edge handling, and experimental plumbing. It could not establish clinical performance, subgroup fairness, real prevalence, realistic missingness, or generalizability. Final empirical claims would still require approved real-data analyses or independently validated public data.

Exact protected cohort characteristics were treated as potentially sensitive even if no direct identifier was present.

## Public/private strategic boundary

The historical discussion included private career, immigration, and commercialization motivations. Those details are not reproduced. The public causal summary is limited to the following:

> Internal strategic objectives favored methodological work capable of producing independently recognized research contributions, transferable technical skills, external adoption, and strong publication artifacts.

This explains the emphasis on a public benchmark, reusable evaluation infrastructure, publication-quality methodology, and independent adoption without disclosing the private objective function.

Faculty discussion is similarly limited to public roles, official adviser eligibility, methodological fit, and whether an advising commitment had actually been confirmed. Private assessments of named individuals are excluded.

## Durable provenance workflow

The archive recognized that long conversations are lossy and should not be the sole project memory. It recommended multiple focused workstreams with durable files for decisions, current state, evidence, experiments, failures, open questions, and next actions, with Git history preserving dated milestones.

For Stream 02 reconstruction, the consequence is:

- the source archive remains primary provenance;
- the structured entries record the reasoning that affects dissertation strategy;
- provider/platform identities are not recorded;
- operational UI instructions and the request to generate the PDF do not need separate substantive entries;
- raw screenshots remain outside the repository;
- structured provenance does not become canonical merely because it is easier to retrieve.

## Unresolved questions

1. Which schema details and aggregate statistics were permitted outside the restricted environment?
2. Which code and derived artifacts could be released publicly?
3. Could a public-data benchmark approximate the important clinical failure modes sufficiently to support early methods work?
4. How would external users validate or adopt a system whose strongest clinical results might remain restricted?
5. Which private evidence needed long-term preservation outside the public repository?

No restricted data or quantitative enclave result is included in this stream.
