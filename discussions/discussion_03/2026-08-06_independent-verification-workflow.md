# Independent verification as working method: from paper principle to project practice

- **Period:** 2026-08-05 to 2026-08-06
- **Sources:** LIT-001, LIT-002 (the papers whose shared principle was operationalized)
- **Related:** `2026-08-06_hegtkg-and-two-paper-synthesis.md` (which archives the audit event itself), `2026-08-22_cohort-feasibility-evidence.md` (where the practice caught the cohort-narrowing error), DEC-005

## Why this is archived

The repository's multi-stream architecture exists because of the reasoning archived here. On 2026-08-05 the user deliberately applied the principle both examined papers argue (a generator cannot verify its own output) to the project's own workflow, by having an independent second reader audit this stream's consolidated report. The audit caught four real errors this stream had missed, and itself contained at least two unverified claims presented as fact. The next day the user generalized the experiment into a standing working method. Per the stream convention, the platform identity of the second reader is not recorded.

## Digest

**Empirical (about the project's own process).** The audit confirmed four errors in this stream's report, all of the same class: the stream found a table, treated it as the table, and stopped searching (a search-completeness failure). The critique also made the same class of error it identified, in two places. Resolving those required going back to the paper. The conclusion the user adopted: critique findings are candidates, not verdicts; the decisive step is verification against the source, done by the user.

**Inference (stream 03), adopted as method.**

1. **Why an independent reader works.** Not greater capability: the second reader has not already committed to the claim. Once this stream had written a claim, it became a premise it built on rather than a claim it rechecked.
2. **The phase structure.** Explore (one stream, iteratively, where the user's pushback does the work); Consolidate (same stream produces the artifact); Audit (second stream, one shot, given the source, the original instructions, and the output, asked specifically about instruction-following and factual accuracy); Verify (the user, against the source; non-negotiable); Revise (original stream folds in what survived verification). A single-pass audit with a well-posed question avoids the endless back-and-forth cycle; the framing of the audit, not tooling, is what makes it work.
3. **For code, the loop is three-way.** Implementer, execution, auditor, with execution first: tests, type checkers, and running the code catch most of what a reviewer would, so the auditor is pointed at what execution cannot verify (wrong approach to the right problem, unhandled edge cases, silent failure modes, passing tests for the wrong reason, misreading the spec). Implementer-first always; both models drafting produces two drafts, not a better one. Give the auditor the failing case, not just the code.
4. **Test case chosen.** The user's existing graph-explorer project (already built and committed to a public repository) was selected as the pilot for the implementer/auditor loop, because an existing codebase tests the audit loop rather than the build loop, and correctness questions about its graph operations have checkable answers.

## Key excerpts

> **User (2026-08-06):** it has made me consider that I should adopt this strategy for all future uses. I would probably get better results if I used both of you in conjunction on the same project, for something like understanding a research paper, coding, brainstorming research directions etc.

> **Stream 03 (2026-08-06):** So the pattern isn't "second model adjudicates" — it's "second reading surfaces candidates, you verify against the source." [...] And note that resolving both of those took me going back to the paper.

> **User (2026-08-06):** my primary goal is to use 2 models for projects that involve not just reasoning and brainstorming research ideas, but also implement them using code. So if I use 1 as an implementer and the other as a reviewer/ auditor, that can help.

> **Stream 03 (2026-08-06):** Code has a ground truth that documents don't: it runs. [...] Implementer-first, always.

## Status

Adopted as practice and applied since (the cohort report's independent review on 2026-08-22 followed this method and reversed a recommendation; see the feasibility entry). The tooling and formalization of the setup were left open ("I will try to figure out this month how to properly build a work setup"), and the pilot on the graph-explorer project had not run by the time of archiving. This method is also the reason the repository maintains independent discussion and analysis streams rather than one merged record (DEC-005).

## Relevance to candidates

- **Candidate 04 (evaluation, verification, safety):** the method is a lived instance of the candidate's core claim, that generation and verification must be separated; the project's own workflow is now evidence the user can point to when arguing the research direction.
- **Candidate 01 (trustworthy agentic AI):** the implementer/execution/auditor decomposition is an agent-workflow design pattern arrived at from practice.
