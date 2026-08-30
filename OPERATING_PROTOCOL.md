# Operating Protocol for Analysis Systems

Provider-neutral rules for how any AI analysis system should allocate its computation in this repository. The goal is not to reduce reasoning quality or discourage frontier-model use; it is to maximize the fraction of frontier compute spent doing the research (scientific reasoning, methodological criticism, hypothesis generation, experiment design, novelty assessment, adversarial review, synthesis, difficult judgment) and to minimize the fraction spent remembering the research (reconstructing historical context, rereading processed exports, redundant repository scans, repeated ingestion, unnecessary multi-agent decomposition, mechanical version-control operations).

This protocol governs process only. It changes no scientific decision, scoring criterion, ranking, or provenance record, and it is subordinate to the analytical-independence rules in `README.md` and DEC-005.

## 1. Progressive context retrieval

Start with the smallest authoritative context sufficient for the task, and widen only when a concrete dependency is discovered:

current task specification
→ `decisions/` (canonical project state)
→ relevant `candidate_programs/` or `analysis/` files
→ relevant `evidence/` records
→ relevant `discussions/` provenance
→ relevant `literature/records/`
→ the original paper or source
→ raw historical chat exports, last.

Do not reread large historical exports merely to reacquire context already represented faithfully in structured repository files. Escalate toward primary or raw material when: provenance is insufficient; a claim is disputed; exact wording matters; a source record is incomplete; independent verification is required; or a conclusion depends on information lost during compression.

## 2. No full-repository reread by default

Identify the smallest dependency set first. Do not recursively read the entire repository before every task. Broaden retrieval only when a concrete missing dependency appears.

## 3. No raw-history reread by default

Once a discussion stream is marked COMPLETE ENOUGH FOR CROSS-STREAM ANALYSIS, its structured provenance archive substitutes for the historical conversation exports in routine work. Raw exports remain primary provenance and may be reopened under the escalation triggers in rule 1, never as a routine context-loading mechanism.

## 4. Single reasoning process by default

Default to one strong reasoning process plus targeted retrieval. Parallel agents are justified when: workstreams are genuinely separable; independent replication materially increases confidence; adversarial perspectives are intentionally required; the corpus exceeds reliable single-context processing; or parallel literature searches cover meaningfully different hypotheses. Task size alone justifies nothing. Before launching more than three parallel agents, state in the execution plan (rule 14) why the additional parallelism provides methodological value.

## 5. Reasoning and execution are different work

Use frontier reasoning for scientific decisions, methodological choices, interpretation, criticism, synthesis, and uncertainty resolution. Use deterministic tooling for file creation and renaming, formatting, checksum generation, version-control operations, routine validation, and reproducible scripts. Once the intended change is fully specified, do not re-invoke expensive independent reasoning to execute it.

## 6. Stream independence

During independent analysis, a stream must not read another stream's conclusions before producing its own first-pass analysis, unless the process has explicitly entered the cross-review stage. Shared factual sources, literature records, canonical decisions, and repository conventions may always be read. Historical provenance reconstruction for one stream must never import another stream's retrospective critique into that stream's historical record.

## 7. Source reuse without claim inheritance

Reuse existing LIT IDs and literature records rather than rediscovering or duplicating sources. Reusing a source never obliges accepting another stream's interpretation of it. Each independent analysis may challenge a source's interpretation, relevance, methodological implications, novelty implications, and evidentiary strength.

## 8. Cache expensive ingestion

When a large source has been processed into a sufficiently complete structured representation whose provenance and scope are documented, use that representation for routine downstream work; primary-source escalation under rules 1 and 11 still applies whenever stronger verification is needed. Repeat the ingestion only when the representation is incomplete, the downstream question requires information omitted from it, source verification is necessary, or the representation is disputed.

## 9. Stopping rule

Before additional retrieval, analysis, or agent spawning, ask: is this computation reasonably likely to change the next scientific action, a conclusion, a confidence level, or an identified uncertainty? If not, stop. Do not pursue marginal certainty for its own sake.

## 10. Compute scales with decision consequence

Low-consequence or reversible tasks: minimal context and analysis. Moderate scientific decisions: targeted literature and reasoning. High-consequence or hard-to-reverse decisions justify deep, independent frontier-model analysis: dissertation-program selection, the central hypothesis, advisor configuration, major methodological commitments, candidate-definition freezes, and any interpretation that could invalidate novelty.

## 11. Compression is not authority

When a structured record and a primary source conflict, or when exact scientific claims matter, return to the primary source. Never propagate a compressed statement merely because it already exists in the repository.

## 12. Measure output, not compute

The objective is not to minimize tokens or agent calls; it is to maximize useful scientific output per unit of researcher attention and model computation. Expensive computation is correct whenever it materially improves scientific validity, novelty assessment, methodological rigor, reproducibility, or decision quality.

## 13. Human checkpoints

Stop for user review before: changing a canonical decision; freezing a candidate definition; any write that could move a private or internal criterion into this public repository; acting on conflicting evidence that would materially change a ranking; proceeding past provenance that cannot be resolved; any write that would erase or reinterpret historical reasoning; materially changing `OPERATING_PROTOCOL.md` itself; and anything implicating institutional or privacy constraints.

## 14. Execution plan for expensive tasks

Before a computationally expensive task, state briefly: the objective; the files and sources required; the files and sources deliberately excluded; whether external research is required; whether parallel agents are justified (rule 4); the expected artifact; and the stopping condition. Do not impose this on trivial tasks.

## 15. Efficiency must not suppress intellectual independence

This protocol never licenses an arrangement in which one system reasons and the others merely execute. For the high-consequence decisions in rule 10, every participating analysis stream conducts genuinely independent reasoning, per DEC-005 and the independence rules above.

The optimization target, in one line: fewer tokens spent remembering the research; more frontier compute spent doing the research.
