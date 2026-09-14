# Analysis paths and historical provenance

Effective date: 2026-09-12. Authority: DEC-010 in `decisions/decision_log.md`.

## Current ownership map

| Historical directory / stream | Current directory | Tool identity |
|---|---|---|
| `analysis/analysis_01/`; Stream 01; S01 | [`analysis/ChatGPT_disst/`](ChatGPT_disst/) | ChatGPT |
| `analysis/analysis_02/`; Stream 02; S02; D02 | [`analysis/Codex_disst/`](Codex_disst/) | Codex |
| `analysis/analysis_03/`; Stream 03; S03 | [`analysis/Fable_disst/`](Fable_disst/) | Fable, the user's label for the Claude-based stream |

These names identify the originating tool stream, not an independent human author or a permanent model version. Record the actual tool/model version when known in new work; do not infer or rewrite the model version of historical work.

The six Day 1 files were moved without changing their contents. Historical stream identifiers, original paths, source dates, source identifiers, titles, and freeze notices remain unchanged inside them. Interpret unversioned old analysis paths using the table above. A historical citation pinned to a commit must still use the path that existed at that commit. The pre-migration main checkpoint is `8e5647c8391ea95dd7ae43f215137f923909ed9a`.

## Content-preservation manifest

The two Day 1 basenames are unchanged in every current directory.

| Current path | Unchanged Git blob identifier |
|---|---|
| `analysis/ChatGPT_disst/day1_candidate_generation.md` | `81c3de3603b8c9168c34c84501aa89ee93bb2af1` |
| `analysis/ChatGPT_disst/day1_candidate_generation_v2.md` | `cd3697120c679c1fb3668c6fff6ac9039cd035ba` |
| `analysis/Codex_disst/day1_candidate_generation.md` | `4505f3d24082ae055892f76c0dd86189d0b18444` |
| `analysis/Codex_disst/day1_candidate_generation_v2.md` | `47e38356b025c2cab49329744e93bf05ec439003` |
| `analysis/Fable_disst/day1_candidate_generation.md` | `67a61e06194cb80fa5ce140148f3e7ce6a37aab0` |
| `analysis/Fable_disst/day1_candidate_generation_v2.md` | `836f9cd2f6b72640339fbbdb98d264cede1116ae` |

## Recovered Fable reviews imported as archival evidence

Three already-public recovered reviews are copied here without changing their bytes. Their original branches and commit histories remain intact. This archival import does not adopt their judgments, approve packets, or launch scientific falsification. Importing file blobs is not a merge of their source commit histories.

| Current path | Original source commit and path | Git blob identifier |
|---|---|---|
| [`Fable_disst/round2_normalization_review.md`](Fable_disst/round2_normalization_review.md) | `66686c05134652aa17ceb31854581cb9aee87161:analysis/analysis_03/round2_normalization_review.md` | `00b0b61bc6b16936954b8a87ff256c4b7c139474` |
| [`Fable_disst/candidate_packet_fidelity_audit.md`](Fable_disst/candidate_packet_fidelity_audit.md) | `be73f0e68d14690a882dd48161165f716a33ab82:analysis/analysis_03/candidate_packet_fidelity_audit.md` | `0cffe33163797306dbd6386b4f1eabbe39e85de2` |
| [`Fable_disst/candidate_packet_reconciliation_audit.md`](Fable_disst/candidate_packet_reconciliation_audit.md) | `6e990866e1b11a5e841fa4f10b9a16b0e317ec52:analysis/analysis_03/candidate_packet_reconciliation_audit.md` | `75a7468e4bbcdbd1e09056a7d795c74bb3dc370c` |

## Preserved Codex reviews imported as archival evidence

Import date: 2026-09-14. Tool/model: Codex / GPT-6. Role: mechanical archival import. Base: `924eeb2cc3bda04fd9ea48c9e7c15ef155770d3e`.

These three already-public reviews are unchanged archival copies under `analysis/Codex_disst/`. Their original branches remain preserved at the source commits below. Titles, dates, historical stream identifiers, paths mentioned inside the documents, and freeze notices are unchanged. Copying these blobs does not merge their source histories, adopt their scientific conclusions, approve packets, or launch scientific analysis.

| Destination path | Original branch | Original source commit and path | Unchanged Git blob identifier | Verified SHA-256 |
|---|---|---|---|---|
| [`analysis/Codex_disst/round2_normalization_review.md`](Codex_disst/round2_normalization_review.md) | `codex/analysis02-round2-normalization-review` | [`21fd7d78d14c34d15e803ee6be01e3d7deb79bcd:analysis/analysis_02/round2_normalization_review.md`](https://github.com/avi2squre/phd-dissertation-strategy/blob/21fd7d78d14c34d15e803ee6be01e3d7deb79bcd/analysis/analysis_02/round2_normalization_review.md) | `440945d2bc3aa7afe3423d0c297df0e1bfa62e40` | `3c5eb5a5e7435db8cd4bf3f4fbbed9453200f4e0e9d621f8df3fb1d08aafd3c4` |
| [`analysis/Codex_disst/candidate_packet_fidelity_audit.md`](Codex_disst/candidate_packet_fidelity_audit.md) | `codex/analysis02-packet-fidelity-audit` | [`0458a99ea5c6ea14eff6f5cf8dfb247ec642cfb3:analysis/analysis_02/candidate_packet_fidelity_audit.md`](https://github.com/avi2squre/phd-dissertation-strategy/blob/0458a99ea5c6ea14eff6f5cf8dfb247ec642cfb3/analysis/analysis_02/candidate_packet_fidelity_audit.md) | `7c551541503f6fd4dd5c4f267cd2fafcdba29d38` | `e8fdf4791bf107b327c221b2d501df20024a38380a104828a3b6d49512414840` |
| [`analysis/Codex_disst/candidate_packet_reconciliation_audit.md`](Codex_disst/candidate_packet_reconciliation_audit.md) | `codex/analysis02-packet-reconciliation-audit` | [`57db21d29da4e99c621ce84ec555a44dcd193f22:analysis/analysis_02/candidate_packet_reconciliation_audit.md`](https://github.com/avi2squre/phd-dissertation-strategy/blob/57db21d29da4e99c621ce84ec555a44dcd193f22/analysis/analysis_02/candidate_packet_reconciliation_audit.md) | `0bcf89711d9173c9f378fd64eb58ee034be6d8ab` | `e12fc47eb800d8259e69c448128d3f79348ac2a216cca7b596bf22ff27394ea7` |

Other reviews may still exist only in separate branches or local workspaces. These tables are not a claim that all three streams' historical work has been integrated.

## Compatibility and future outputs

- Apply the ownership map to output-directory examples in older schemas and prompts. Do not create new numbered analysis directories merely because a historical template names them.
- Existing frozen file basenames and scientific bodies are unchanged. New standalone exports should include the tool prefix, for example `Fable_disst_2026-09-12_topic.md`, so a file remains identifiable outside its parent folder. Record the canonical path and content digest with an export.
- Shared protocols, schemas, literature, evidence, candidate packets, and coordinator decisions are not attributed to a single tool by a directory rename.
- `discussions/discussion_01/`, `discussion_02/`, and `discussion_03/` are historical provenance archives and are not renamed in this migration. They correspond to the same three streams.
- Preserved historical branches retain their old layouts. Do not rebase or rewrite them just to rename directories. Start new tasks from an explicitly verified current base; transfer a needed old artifact with recorded source provenance, not by silently mixing whole folders.

## Local worktrees are a separate layer

A local worktree name identifies the task owner, not the author of every file in its checkout. A Fable worktree may correctly contain all three tools' analysis directories because it is a checkout of the shared repository.

Prefer persistent worktree names such as `Fable_disst_<task>` and `Codex_disst_<task>`. Verify the runtime, repository identity, registered worktree, active task, and destination before moving anything. Use Git's worktree operations rather than dragging registered worktrees in Finder. Do not move the primary repository or unrelated sibling directories. See [Git worktree documentation](https://git-scm.com/docs/git-worktree).

The GitHub migration does not itself rename or synchronize folders on the user's Mac.
