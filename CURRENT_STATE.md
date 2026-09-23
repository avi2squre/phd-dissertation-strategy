# Current project state and next decisions

Updated: 2026-09-23. Authority: DEC-010 through DEC-016 in [`decisions/decision_log.md`](decisions/decision_log.md). These entries record the user's approval of clearer tool ownership, persistent workspaces, a lighter decision-oriented process, open-ended topic discovery without removing existing directions, the project-wide communication preference, the sustainable preparation workflow, the active/archive artifact lifecycle, and the Chat/Codex/Work allocation strategy described below.

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
| Faculty / independent-study coordination | Erich Kummerfeld scheduled a Zoom meeting with Avi for Thursday, 2026-09-24, 1:15–2:00 PM CDT. The meeting will assess HINF 8492 supervision/permission and substantive research overlap. A 2-credit independent study remains a possibility, not an approved arrangement. |
| Grammar/writing corrections in this project | Disabled by default across all chats unless the user explicitly asks to resume them |
| Preparation workflow | Bounded, outcome-based preparation is the default for meetings, classes, presentations, tests, and deadlines. Protect sleep and preserve regular time for exercise, meals, chores, social life, and personal downtime; reduce scope rather than letting preparation expand indefinitely. |
| Active working workbooks | Keep a deliberately small active set: `PhD_Preparation_Guidelines_and_Templates.xlsx`, the current Kummerfeld meeting reference workbook, and `IHI_Fellowship_Progress_Tracker_Sep2026_CURRENT_v3.xlsx` in the NLP Library Active folder. A compact Kummerfeld replacement is pending; do not treat the earlier larger draft as the final reference once the replacement is verified. |
| Archive lifecycle | Completed task workbooks are distilled for current relevance and preserved under the NLP Library Archive hierarchy. Historical artifacts remain retrievable and do not stay active merely because they contain useful background. |
| Tool allocation | Chat is the default for non-coding work and straightforward coding; Codex is reserved preferentially for complex/repository-scale software work; Work is reserved for autonomous multi-step browser/desktop/repetitive delegated workflows. |

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

## Active / archive artifact lifecycle

Use DEC-014 for task-specific working artifacts.

- Keep the active set small and tied to immediate execution.
- Before archiving a completed task workbook, extract only information that still changes a current decision, short-term action, or reusable process.
- Preserve the full historical workbook in Archive for later retrieval; do not keep it active as a substitute for current state.
- Use the general preparation workbook as a reusable template. Derive bounded task-specific workbooks from it rather than rebuilding a large permanent dossier for every meeting.
- Current Library structure includes `/NLP/Active/`, `/NLP/Archive/Meetings/2026-09_Gyorgy_Simon/`, and `/NLP/Archive/Fellowship_Tracker_Versions/`.
- The available file-management tool cannot move/detach Project attachments themselves. Archive copies therefore coexist with any older attachments that may remain visible on the Project surface; this is a product-surface limitation, not an indication that those files remain operationally active.

## Sustainable preparation workflow

Use DEC-013 as the default planning rule for PhD preparation.

- Define the actual performance objective before deciding how much preparation is needed.
- Set a bounded preparation budget and explicit readiness/stop criteria before starting.
- Separate must-know or must-produce work from useful extras and optional perfectionism.
- If time is tighter than initially expected, compress scope to the highest-value work rather than automatically extending work into the night.
- Protect sleep by default and preserve recurring space for exercise, meals, chores, social activity, and personal downtime.
- Evaluate preparation by whether the user can perform the required task, not by the number of hours spent.
- Exact hour caps remain task-specific and may be revised from experience; they are not yet globally fixed.

## Chat / Codex / Work allocation

Use DEC-015 as the default tool-selection rule.

- Prefer Chat for research discussion, source/file work, planning, analysis, writing, spreadsheets, meetings, and straightforward coding.
- Prefer Codex when repository-scale implementation, testing, debugging, refactoring, or substantial software engineering is the main task.
- Prefer Work when autonomy, browser/desktop interaction, repetitive multi-step execution, or a long delegated workflow is the main source of value.
- Do not use Work merely because a task is intellectually difficult, and do not use Codex merely because a task contains code.
- Short-term capacity objective: before 2026-10-03, use one deliberate high-value Work run and one deliberate high-value Codex run so the user's reported remaining reset is not wasted.

## Meeting preparation artifact policy

Use DEC-016 for ordinary professor/advisor meetings.

- Chat is the primary collaborative preparation environment.
- The spreadsheet is a quick-reference aid, not the main study environment.
- Default to roughly 3–4 tabs: meeting brief/readiness, faculty + research overlap, prioritized/anticipated questions, and notes/next actions.
- Keep readings and background bounded to what can change the meeting outcome.
- Do not create a Simon-scale multi-tab dossier unless the stakes or complexity clearly require it.
- The compact Kummerfeld workbook is pending completion/verification; archive or supersede the earlier larger draft only after the replacement exists.

## Project communication preference

Grammar, spelling, punctuation, fluency, and writing-correction sections are disabled by default across all chats in this project. Do not add a `Writing check` or equivalent unless the user explicitly asks to resume or requests writing/grammar feedback for a specific message.

## Next checkpoint

Complete local workspace synchronization under the new names. Then conduct outside-in evidence exploration and compare a bounded subset of newcomers with incumbents. Existing packets and reviews remain available as research inputs, not a closed menu. Any specific scientific amendment, candidate selection, visibility change, or sensitive publication still requires an explicit decision.

Near-term faculty coordination: prepare for the scheduled Erich Kummerfeld Zoom meeting on Thursday, 2026-09-24, 1:15–2:00 PM CDT. Use the bounded DEC-013 workflow and the task-specific Kummerfeld workbook. The meeting should resolve whether Erich can supervise/authorize two credits of HINF 8492 and identify a scientifically useful first step if there is substantive overlap. No independent-study arrangement has yet been approved.

## Navigation

- [Tool-owned analysis folders](analysis/README.md)
- [Path migration and archival source manifest](analysis/PATH_MAP.md)
- [Historical normalized candidate map](analysis/round3_normalization_reconciliation.md)
- [Accepted decisions](decisions/decision_log.md)
