# Current project state and next decisions

Updated: 2026-09-12. Authority: DEC-010 and DEC-011 in [`decisions/decision_log.md`](decisions/decision_log.md). These entries record the user's approval of clearer tool ownership, persistent workspaces, a lighter decision-oriented process, and open-ended topic discovery without removing existing directions.

## What is current

| Item | State |
|---|---|
| Existing research portfolio | Eight normalized directions, N1, N2, N3, N4a, N4b, N5, N6, N7; retained, not selected or ranked |
| Search space | Open to additional avenues; the historical eight are not exhaustive |
| Main analysis paths | `analysis/ChatGPT_disst/`, `analysis/Codex_disst/`, `analysis/Fable_disst/` |
| Historical identifiers | Stream 01/02/03, S01/S02/S03, D02, candidate IDs, and literature IDs retained |
| Original Day 1 file contents | Unchanged; path migration only |
| Three recovered Fable reviews | Imported unchanged as archival evidence; original commits/branches preserved |
| Common packet set | Draft 0.1 on its historical branch; not promoted or scientifically amended by this migration |
| Formal Phase 1 | Not launched; common-packet readiness gate remains if formal mode is invoked |
| Current authorized mode | Open-ended horizon scanning, concise evidence comparison, faculty feedback, and bounded pilot design |
| Current canonical ranking | None; `decisions/current_rankings.md` is a historical preliminary ranking, not the active eight-direction ranking |
| Repository visibility | Not changed; private-workspace separation remains a distinct access-control task |

## Decision-oriented workflow

Distinguish three decisions: what merits faculty discussion, what merits a bounded pilot, and what merits dissertation-level commitment. They require progressively stronger evidence. Do not spend dissertation-selection effort on a reversible meeting-preparation decision.

1. Retain the incumbent directions and discover additional avenues from research requirements, scientific bottlenecks, emerging data/resources, primary research, and credible translational evidence. New avenues are leads, not automatically approved dissertation candidates.
2. Use short, comparable evidence briefs: scientific question; nearest primary work; precise possible contribution; strongest objection; an informative first study; realistic resources/advising; capabilities the researcher would actually develop. Record findings, inferences, and unverified hypotheses separately.
3. Select a provisional discussion set on evidence, not document polish, novelty of terminology, or sunk preparation effort. Faculty input is part of investigation, not a reward after all reviews finish.
4. Obtain decision-relevant expert/resource input and run bounded studies. Stop or redirect when another analysis is unlikely to change the next action.

Do not add another full schema or audit cycle merely to operationalize these four steps.

## Scientific interpretation amendments

- Historical fidelity is not scientific validity. Preserve what was proposed; label a better scientific formulation as a new version or explicit amendment, never as mechanical reformatting.
- Report hypothesis results separately from research-direction disposition. A contradicted superiority hypothesis or informative null result does not automatically eliminate the broader research question.
- Coherence means a connected intellectual argument and compatible research questions; do not require every aim to support one preselected positive empirical outcome.
- Evaluate novelty by the actual contribution. Existing components do not prove novelty, but an application, measurement study, benchmark, or integration is not automatically scientifically trivial.
- Normally treat future-model resilience as scenario analysis rather than a confirmed fatal forecast.
- For diagnostic-state work, distinguish documented status, contemporaneously justified state, and retrospective disease truth. Reference-standard independence concerns circular labeling, model predictions, and leakage; it does not automatically require a different underlying document source.
- Preserve the historical N7 conjunction as history. Any future change to its mandatory ranking/conclusion-reversal condition must be an explicit scientific revision, not a silent edit to frozen packets.
- No ciliopathy, rare-disease, institutional-cohort, or specific method commitment is made by the current workflow.

These principles guide new work. They do not retroactively change the conclusions or statuses of frozen artifacts or certify any new avenue as novel.

## Independent review without repeated bureaucracy

Independent first passes and source-grounded disagreement remain valuable. Three agent opinions are not three independent empirical confirmations. Rotate complementary literature, methods, and synthesis responsibilities while permitting every reviewer to challenge a claim. Use one substantive review and a bounded rebuttal by default; additional rounds need a concrete decision-relevant unresolved issue.

The current ChatGPT thread has already seen other streams' historical reviews. Do not relabel it retrospectively as blind. Disclose exposure and use a fresh, appropriately scoped context when a new blind pass is required.

## Stable execution and ownership

- Confirm actual runtime and filesystem access before assuming a Mac path exists.
- Use a verified persistent repository as the anchor and separate persistent worktrees for concurrently active tasks. Prefer names `<Tool>_disst_<task>`; never have two agents switch branches or modify the same worktree concurrently.
- Record tool, model/version when known, role, base commit, output path, and durable preservation location. A recognizable folder name does not determine ownership of all files in a shared checkout.
- Preservation and approval are separate. Preserve completed public-safe work on an authorized remote branch, or in an approved private backup if the content is not public-safe. Do not auto-publish sensitive material. A preservation push does not authorize a merge.
- Before declaring completion, verify content against its recorded fingerprint at the durable destination. Do not rely only on temporary paths or agent memory.
- Use exact current repository-relative paths and actual absolute paths for materialized local outputs. A GitHub change does not automatically update Finder.
- Never rewrite old branches, delete archives, force-push, or silently replace scientific reasoning to make names consistent.

## Next checkpoint

Complete local workspace synchronization under the new names. Then conduct outside-in evidence exploration and compare a bounded subset of newcomers with incumbents. Existing packets and reviews remain available as research inputs, not a closed menu. Any specific scientific amendment, candidate selection, visibility change, or sensitive publication still requires an explicit decision.

## Navigation

- [Tool-owned analysis folders](analysis/README.md)
- [Path migration and archival source manifest](analysis/PATH_MAP.md)
- [Historical normalized candidate map](analysis/round3_normalization_reconciliation.md)
- [Accepted decisions](decisions/decision_log.md)
