# Diagnostic state as a trajectory: the research question that verification does not answer

- **Period:** 2026-08-20 (following a group meeting in which the clinical collaborator responded to the cohort work)
- **Sources:** LIT-001, LIT-002 (what verification handles); LIT-003 (the pipeline setting); LIT-006, LIT-007 (ontology)
- **Related:** `2026-07-23_rare-phenix-verification-proposal.md`, `2026-08-22_cohort-feasibility-evidence.md`

## Why this is archived

A domain expert's methodological point, made in a meeting, converted the cohort work's main problem into a research question that the examined papers do not address. Stream 03 judged it the best candidate direction to come out of the week. It is archived as an **inference and untested question**, with the expert's contribution attributed.

## The collaborator's input (attributed; from the 2026-08-20 meeting)

Dr. Xiaoyi Chen (clinical collaborator on the CIL-FLARE project) made two points about the cohort work:

1. Disease names in clinical notes are frequently suspicions under investigation rather than confirmed diagnoses, and genetic testing may later rule them out. A count of patients with a matching disease name is therefore a name-match count, not a confirmed cohort.
2. The reverse error also exists: a patient with the disease may be coded only for its downstream consequences and never carry the disease code. The cohort has false positives and false negatives, and neither was quantified.

She also noted that the current diagnostic classification (ICD-10) has limited coverage of rare-disease names, which its successor improves but which is not yet in clinical use.

## Digest

**Inference (stream 03).**

- Verification as implemented in LIT-001 checks whether a claim is consistent with a knowledge graph (is this phenotype a documented feature of this disease). LIT-002 attaches provenance and time anchors to each claim. Both address whether a claim is true of the world.
- The collaborator's problem is different in kind. A note that says "under investigation for [disease]" yields a correct extraction, a correct ontology mapping, and a true claim (the patient is under investigation). What is uncertain is whether the patient has the disease, and no knowledge graph contains that. It is a fact about the patient's diagnostic state, not about biology.
- This is the July finding in a new form: verification checks truth of the world, never whether the note asserts it; here the note asserts a hypothesis rather than a fact. The distinction between possible, confirmed, and ruled-out is modality, and it lives in the note's language rather than in any ontology. It is also one of the context dimensions the collaborator had named earlier in the project (uncertainty).
- The mechanism that resolves the hypothesis is usually a later event (genetic testing). A patient's diagnostic state is therefore not a single extraction but a **trajectory across notes**: a suspicion at one time becomes confirmed or excluded at a later time. The unit of analysis is the patient timeline, and the question is when and whether the hypothesis resolved.
- The data available to the user has the structure to support this: timestamped notes, timestamped diagnosis codes, and laboratory and genetic result tables not yet examined (see the feasibility entry).

**The research question, as stated in the stream:**

> Can we determine, from longitudinal clinical notes, whether a rare disease mentioned as a suspicion was ultimately confirmed or excluded, and does that resolve the cohort-definition problem that codes and name mentions cannot?

**Shape.** Neural extraction of mentions and their modality; symbolic representation of diagnostic state and its transitions over time. This is neurosymbolic in shape without needing the label, and it is a problem a domain expert handed over rather than one selected from a trend.

**What it would change.** If it works, ground truth for rare-disease phenotyping could be established from the record itself rather than requiring clinician adjudication of every patient, which the feasibility entry identifies as the binding cost. If it does not, the failure would still characterize how far structured plus narrative data can go, which is itself an evaluation result.

## Key excerpts

> **User:** "if neither codes nor name mentions establish who has the disease, notes are the only remaining source." Can this potentially be tackled using knowledge graphs and the methods proposed in any [of] the papers we have read so far?

> **Stream 03:** Partly, and being precise about which part is where the interesting research question sits. What the papers do handle. [LIT-001]'s Review checks whether a claim is consistent with a knowledge graph [...]. [LIT-002] attaches provenance and temporal anchors to each claim. Both address is this claim true of the world. What [the collaborator's] problem is. A note says "under investigation for nephronophthisis." The extraction is correct. The mapping is correct. The claim is even true — the patient is under investigation. What's uncertain is whether the patient has the disease, and no knowledge graph contains that. It's a fact about this patient's diagnostic state, not about biology.

> **Stream 03:** So a patient's diagnostic state isn't a single extraction — it's a trajectory across notes, where a suspicion at month 3 becomes confirmed or excluded at month 8. That means the unit isn't a note. It's a patient timeline, and the question is when and whether the hypothesis resolved.

## Status

Untested question. No literature search has been done on modality and diagnostic-state extraction (assertion classification, temporal reasoning over clinical narratives, hypothesis resolution). Novelty is **not** established by this entry and should not be inferred from it; the relevant literature must be examined and registered before this becomes a candidate research question.

## Relevance to candidates

- **Candidate 02:** the neural-modality plus symbolic-state design is a direct instance.
- **Candidate 01 (trustworthy agentic AI):** an agent tracking a patient's diagnostic state over time is a longitudinal belief-revision problem. A brainstorm in a separate thread of this stream three weeks *earlier* (2026-07-28, since archived as `2026-07-28_evaluation-and-assurance-brainstorm.md`, instantiation A1) had already formulated longitudinal belief revision as an evaluation question; this entry's trajectory question is its clinically grounded counterpart, arrived at from the collaborator's input without citing that session. The original cross-reference here called the brainstorm "later" before its export was processed; the corrected chronology is as stated, and the connection between the two is an archival observation.
- **Candidate 04:** whether a system's belief about diagnostic state tracks the record's resolution is an evaluable property with a natural ground truth (the later test result).
- **Candidate 03 (causal / real-world evidence):** cohort definition is upstream of any real-world-evidence claim; this question is the cohort-definition problem stated precisely.
