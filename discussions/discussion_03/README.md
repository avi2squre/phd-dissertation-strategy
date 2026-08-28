# Discussion Stream 03

This directory archives the substantive reasoning from analysis stream 03 that bears on dissertation strategy. Per `discussions/README.md`, the platform behind this stream is not recorded here.

Raw discussion is supporting evidence, not canonical project state. Nothing in this directory changes an accepted decision. Where an entry disagrees with a file elsewhere in the repository, the disagreement is stated in the entry and left for the decision process.

## Provenance

All entries derive from one continuous conversation thread running from 2026-07-21 to 2026-08-28, plus the working documents produced in it (two journal-club decks, a rare-disease cohort report, and a proposal to insert verification into a phenotyping pipeline). Dates in filenames are the dates of the underlying exchanges, not the archiving date.

Entries contain two kinds of text:

- **Excerpts.** Verbatim passages from the thread, labeled `User:` and `Stream 03:`. Cuts are marked `[...]`. Excerpts preserve the original wording, including claims that were later retracted; retractions are archived alongside them.
- **Digest.** Stream 03's own summary of what the exchange established, written at archiving time. Digests are labeled by evidentiary status: *source-supported* (traceable to a `LIT-XXX` record), *empirical* (from the cohort work; see redaction note), *inference*, or *untested proposal*.

## Redaction policy for this public repository

Three things are deliberately withheld:

1. **Quantitative results from the institutional data enclave.** The cohort work was done inside a secure environment whose file-transfer rules govern what leaves it. Patient counts, proportions, and interval statistics are therefore described qualitatively here and live in the internal report. Restoring them is a separate decision that should be checked against the data-use terms first.
2. **Personal assessments of named individuals.** Faculty are referenced only by public role, appointment type, and documented project involvement.
3. **Platform identity of any analysis stream**, per the repository convention.

## Entries

| File | Period | What it archives | Bears on |
|---|---|---|---|
| `2026-07-23_kgarevion-verification-analysis.md` | 2026-07-21 to 07-23 | Close reading of LIT-001: the Review mechanism, the failed explanations for Revise, the determinism argument, and the limitations found | Candidate 02, Candidate 04, family 5 (KG + LLM reasoning) |
| `2026-07-23_rare-phenix-verification-proposal.md` | 2026-07-22 to 07-23 | The gap identified in LIT-003 and the proposal to insert graph verification into its standardization step, including the anchor constraint and the class-based verification design | Candidate 02, Candidate 04 |
| `2026-08-06_hegtkg-and-two-paper-synthesis.md` | 2026-08-03 to 08-06 | Close reading of LIT-002, comparison with LIT-004, and the verify-after versus supply-before synthesis of LIT-001 and LIT-002 | Candidate 02, Candidate 04 |
| `2026-08-20_neurosymbolic-framing-and-advisor-sequencing.md` | 2026-08-20 | Whether "neurosymbolic AI" is a dissertation direction; the narrower framing proposed; sequencing of direction versus advisor; a disagreement with `context/advisor_landscape.md` | Candidate 02, `current_rankings.md` rank 2, advisor landscape |
| `2026-08-20_diagnostic-state-trajectory-question.md` | 2026-08-20 | The research question that emerged from a clinical collaborator's input: diagnostic state as a trajectory across notes rather than a single extraction | Candidate 02, Candidate 01 (agentic systems), Candidate 04 |
| `2026-08-22_cohort-feasibility-evidence.md` | 2026-08-08 to 08-22 | Qualitative feasibility findings from the rare-disease cohort work: what structured data can and cannot establish, and what that implies for data-dependent candidates | Candidate 02, Candidate 03, feasibility gate |

## What this stream says about the current repository state

- `candidate_programs/02` and `04` are empty. Entries here supply material for their "core scientific problem," "candidate research questions," and "evidence" sections, but do not fill them; freezing a definition is a decision, not an archive action.
- `decisions/current_rankings.md` ranks six families with one-line rationales. This stream's material supports the caveat already in that file: families 2, 4, and 5 may be components of one program rather than alternatives. See the neurosymbolic entry.
- `context/advisor_landscape.md` lists four names. This stream's reasoning treats a fifth, not on that list, as the leading primary-advisor candidate. This is recorded as a disagreement to be resolved, not an edit.
- `literature/index.md` was empty when this stream was archived. The sources this stream relies on are registered as `LIT-001` through `LIT-014` in the same commit, with honest reading statuses.

## Not yet archived from this stream

A later brainstorm in a separate thread developed a candidate direction ("evaluation and assurance of clinical AI agents") with four instantiations. It is not in this directory because its source export has not been processed. It should be archived as its own entry before it is used in any candidate definition.
