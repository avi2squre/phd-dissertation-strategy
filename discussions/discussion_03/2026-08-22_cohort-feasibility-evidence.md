# What structured EHR data can and cannot establish for a rare-disease cohort: feasibility evidence

- **Period:** 2026-08-08 to 2026-08-22 (cohort work inside the institutional data enclave; internal report completed 2026-08-22)
- **Sources:** LIT-008, LIT-010, LIT-011, LIT-012 (disease definitions used to interpret the codes); LIT-003 (the extraction setting); LIT-006, LIT-007 (ontology)
- **Related:** `2026-08-20_diagnostic-state-trajectory-question.md`

## Why this is archived

This is the stream's only **empirical** evidence, and it bears on feasibility rather than on topic choice. It also archives how the analysis's errors were caught, which became project practice.

## Redaction note

All quantitative values (patient counts, proportions, interval statistics, corpus sizes, per-year distributions) are withheld from this public file because the data were accessed inside a secure environment with governed file transfer. The values are in the internal report. Statements below are qualitative and are labeled *empirical* only where they summarize a query result whose magnitude is withheld.

## Setting

Three diagnosis codes proposed by the clinical collaborator (ICD-10 Q61.5, Q77.2, Q04.3) were used to retrieve a candidate ciliopathy cohort from the institutional clinical data warehouse. Five permanent tables were materialized (diagnosis rows, cohort, note metadata, encounters, billing diagnoses) so that downstream queries run in seconds rather than tens of minutes.

## Findings (empirical, magnitudes withheld)

1. **The codes over-retrieve.** One code (Q04.3) is a heterogeneous category whose recorded diagnosis names include cortical malformations that are not ciliopathies alongside Joubert syndrome; a large share of its patients carry no informative name at all. Another (Q61.5) is dominated by medullary sponge kidney, a distinct condition that is not a ciliopathy (LIT-010). A further subgroup within Q61.5 carries only the legacy label "medullary cystic kidney," which historically covered both nephronophthisis and what is now classified as autosomal dominant tubulointerstitial kidney disease (LIT-011); these patients cannot be resolved from structured data. Within that code, sponge terminology and ciliopathy terminology never co-occur in the same patient.
2. **Only a small minority of code-retrieved patients carry an explicit ciliopathy name** (Joubert syndrome, nephronophthisis, Senior-Løken) in structured diagnosis text.
3. **Names are not diagnoses.** Per the clinical collaborator, recorded names are often suspicions under investigation (see the trajectory entry). The name-matched subgroup is therefore a name-match count, not a confirmed cohort, and the cohort has both false positives and false negatives, neither quantified.
4. **The interval between a patient's first available note and first ciliopathy code is typically long** (on the order of years, median withheld). A small fraction of intervals are negative, which is impossible if the two timestamps mean what was assumed; this establishes that the measure is an interval between two database timestamps, not a validated measure of diagnostic delay, and that timestamp semantics must be validated before any delay claim is made.
5. **The note corpus is large enough for extraction work, and only a small fraction of it mentions ciliopathy terminology.** The ratio neither proves nor disproves under-documentation; it shows how much documentation sits outside the terms.
6. **Data structure.** Encounters nest via a parent-encounter identifier, and a non-trivial share of ciliopathy-coded encounters sit beneath a parent encounter, so encounter-level joins must be nesting-aware. The original diagnosis-name text has systematic missingness concentrated in particular years; the cause was not established (an earlier "migration artifact" explanation was withdrawn as unsupported). One cohort patient has diagnosis rows but no encounters in the encounter table.

## The recommendation, and how it changed

Stream 03's first draft recommended narrowing the analytic cohort to the name-matched subgroup. An independent second reader identified this as verification bias: it selects the patients easiest to find in structured data and discards the atypical ones that narrative extraction exists to recover. The report was revised to keep four strata instead: code-retrieved, name-matched, unresolvable legacy terminology, and an adjudicated sample. Stream 03 agreed with the critique.

**Adjudication** means a clinician reads the longitudinal record and any genetic evidence and records a verdict; it is the only stratum that involves clinical judgment rather than a query, it is the only way to obtain ground truth that is not derived from the fields being evaluated, and it is expensive in clinician time. Annotation responsibilities are divided across sites in the project plan; what the local site is expected to adjudicate is unresolved.

## Environment constraints relevant to feasibility

- No internet inside the enclave; all transfers go through a governed file-transfer service. Hosted tools are disqualified; any language model used on notes must run locally.
- Large unindexed tables make ad hoc queries slow; the working pattern is to materialize once and query the materialized tables.
- GPU access is through a separate cluster with its own onboarding.
- These constraints match the least-tested configuration in LIT-002 (local models), which is a feasibility risk for any candidate that depends on frontier-model quality inside the enclave.

## How errors were caught (process, archived deliberately)

- **Additive distinct counts.** Summing distinct-patient counts across grouped rows overcounted patients; the correct count is at the patient level. Caught by the user tracing the query.
- **Inference stated as measurement.** Several early interpretations (a coding-era hypothesis, an under-coding claim, a billing-table interpretation) were presented as findings and were hypotheses. Caught by the user asking "how did we conclude this."
- **Independent second reader.** A separate model reviewed the draft report and found the cohort-narrowing recommendation and several wording errors. Adopted as practice: do not use the same model to verify its own output.
- **Rule adopted:** every figure is labeled as a query result, derived arithmetic, or inference; and for any non-trivial query or interpretation, the user is prompted to ask for a methodology walkthrough rather than being handed one, because a volunteered explanation reuses the reasoning that produced the result.

## Key excerpts

> **User:** "Cross-system involvement is present but under-coded." How did we conclude this exactly? From the data so far?

> **Stream 03:** We didn't. That was a hypothesis and I presented it as a conclusion — you're right to catch it.

> **User:** Can you confirm that all your code and interpretations so far have been accurate?

> **Stream 03:** No, I can't confirm that — and it would be worth little if I did, since I'm the one who made the errors.

> **Stream 03:** [count withheld] patients have a negative interval [...] That is not possible if the two timestamps mean what I have assumed, so it indicates that at least one endpoint reflects something other than the clinical event [...]. At [proportion withheld] this does not move the summary statistics, but it does establish that what I have measured is an interval between two database timestamps rather than a validated measure of diagnostic delay.

(Two figures in the last excerpt are bracketed out under the redaction note above.)

## Relevance to candidates and the feasibility gate

- **Feasibility gate ("plausible data/resources/infrastructure").** Data access exists and is working. Cohort definition is unresolved, and ground truth requires clinician time. Any candidate whose first paper depends on a validated rare-disease cohort carries this risk on its critical path.
- **Candidate 03 (causal / real-world evidence):** cohort definition is upstream of any real-world-evidence claim; this evidence is the concrete form of that risk.
- **Candidate 02 and 04:** the unresolvable subgroup is exactly where narrative extraction, verification, and diagnostic-state tracking would change the answer, which is a natural evaluation setting with a built-in comparison (structured data alone versus structured plus narrative).
- **Candidate 01:** the enclave constraints define what an agentic system would have to run on.
