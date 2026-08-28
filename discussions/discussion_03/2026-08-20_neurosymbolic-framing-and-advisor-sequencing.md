# "Neurosymbolic AI" as a direction: umbrella versus research question, and the order of direction and advisor

- **Period:** 2026-08-20
- **Sources:** LIT-001, LIT-002, LIT-003 (as instances); official IHI faculty directory (institutional source, not literature); LIT-014 (BioML-bench, discovered only)
- **Related:** `decisions/current_rankings.md` (family 2), `candidate_programs/02_neurosymbolic_metacognitive_ai.md`, `context/advisor_landscape.md`

## Why this is archived

The user asked whether neurosymbolic AI could be a dissertation direction, and separately obtained an answer from another analysis stream. This entry records stream 03's independent answer, where it agreed with the other stream, where it pushed back, and a disagreement with the current advisor-landscape file. It also records the advice on sequencing (direction before advisor) that shaped the following weeks.

## Digest

**Inference (stream 03).**

1. **Not a new direction; a name for existing work.** LIT-001 is neural generation plus symbolic verification. LIT-002 is neural synthesis plus a provenance-anchored graph. The July proposal (`2026-07-23_rare-phenix-verification-proposal.md`) inserts symbolic verification into a neural extraction pipeline. Mapping extracted phenotypes to an ontology is itself a neurosymbolic operation. Two presentations and a report already exist as evidence of work in this pattern.
2. **Umbrella, not a question.** As a dissertation framing, "neurosymbolic AI in healthcare" names a technology family. The stronger version is a specific question in which neurosymbolic methods are the means: verification of LLM-generated clinical output against structured knowledge, or trustworthy phenotype extraction.
3. **Narrow version proposed:** verification of LLM-generated clinical output against structured knowledge, as one contribution. Causal reasoning and agentic execution can be later aims if they earn their place; they do not need to be in the title.
4. **Vocabulary mismatch.** The institute's faculty directory filters research areas by labels such as Artificial Intelligence, Causal Analytics, and Natural Language Processing; "neurosymbolic" is not among them. Faculty doing ontology-grounded clinical NLP or causal analytics are doing structured-reasoning work under other names. Searching for a "neurosymbolic person" is the wrong search.

**Agreement with the other stream.** Both streams concluded independently that "neurosymbolic AI" should not be proposed as the topic. The other stream added faculty analysis from directory profiles that stream 03 could not do without the directory: one core faculty member's doctoral training is in logic and computation, and another works on ontologies for clinical knowledge modeling and secondary use of EHR data, which is the symbolic half of the user's work under a different name.

**Pushback on the other stream (preserved as disagreement).**

- Faculty rankings derived from directory profiles are inferences about fit, not verified interest in this kind of work. That is checkable and should be checked before a proposal is built around a name.
- The other stream's flagship framing combined four areas (neuro-symbolic, agentic, causal, longitudinal data). Stream 03's view: that is a lab's agenda, not a dissertation; four-way novelty means four ways to fail, and a first-year proposal that broad is usually narrowed by the committee anyway.

**Sequencing (inference, adopted by the user).** Approval from a core faculty member is not needed to decide a direction. The order is: form a view; refine it with the research mentor and the clinical collaborator; then approach a core faculty member with something concrete. Arriving with one clear preference and two alternatives reads as a decision; arriving with four equally weighted options reads as not having decided.

**Consistency with DEC-006.** The stream advised that any document shared with faculty rank directions on research grounds (novelty, feasibility with available data, fit with lab strengths, venue), with career criteria informing the ranking privately. This matches the accepted two-layer rule.

## Disagreement with `context/advisor_landscape.md`

That file lists four names under discussion. Stream 03's reasoning treats a fifth, not on the list, as the leading primary-advisor candidate, on public grounds: core IHI faculty; associate director of the NLP/IE group; co-principal investigator with the research mentor on the NSF award that funds the CIL-FLARE project the user works on. One of the four listed names already serves on the user's monitoring committee, which is an existing relationship. This is recorded as a disagreement for the decision process; the context file was not edited.

## Signal from the research mentor (institutional, not literature)

In the 2026-08-20 group meeting the research mentor shared an agent-evaluation benchmark (LIT-014, unexamined) with the group. Stream 03 read this as a signal that "how do we verify what clinical AI agents produce" sits closer to current lab interest than "neurosymbolic AI." This is an inference from one action and should not be over-weighted.

## Key excerpts

> **Stream 03:** Neurosymbolic AI is a broad umbrella, not a research question. As a dissertation framing it risks sounding like you picked a trendy term rather than a problem. The stronger version is a specific question — verification of clinical AI output, or trustworthy phenotype extraction — where neurosymbolic is the method, not the topic.

> **Stream 03:** You've already done this work. KGArevion is neural generation plus symbolic verification. HEG-TKG is neural synthesis plus a provenance-anchored knowledge graph. Your own July 23 proposal was inserting symbolic verification into a neural extraction pipeline. So you're not choosing a new direction. You're naming one you've been building for two months, with two talks and a report as evidence.

> **Stream 03:** The narrow version I'd actually propose: verification of LLM-generated clinical output against structured knowledge. That's one contribution, it's what you've already read deeply, it's measurable, and it sits inside what [the research mentor] was signaling [...]. Causal reasoning and agentic execution can be Aim 2 or Aim 3 if they earn their place. They don't need to be in the title.

> **Stream 03:** The strongest opening, given what you've actually done: "Both papers I presented this summer are verification architectures — generate with a model, check against structured knowledge. My RARE-PHENIX proposal was the same pattern. I'd like to build the dissertation around that: how do we verify what clinical AI produces, and what does verification actually buy?"

## Errors and corrections preserved

- Stream 03 first said it could not read the faculty directory; it could, after a search, and did. The correction is that institutional pages should be fetched rather than inferred from memory.
- Stream 03 initially named faculty from memory with a caution; the directory superseded that list.

## Relevance to candidates and rankings

- **Family 2 (rank 2 in `current_rankings.md`):** this entry argues the family's one-line rationale ("highly differentiated and durable") holds only if the candidate is defined as a specific verification question rather than as the technology family. This bears directly on the candidate-definition rule.
- **Families 2, 4, and 5:** the material here treats them as components of one program (verification method; evaluation of what verification buys; knowledge graph as substrate), consistent with the caveat already in `current_rankings.md`.
