# Inserting verification into a phenotyping pipeline: the gap, the anchor problem, and the class-based design

- **Period:** 2026-07-22 to 2026-07-23 (developed for the 2026-07-23 presentation; revisited 2026-08-05)
- **Sources:** LIT-003 (RARE-PHENIX), LIT-001 (KGARevion), LIT-006 and LIT-007 (Human Phenotype Ontology)
- **Related:** `2026-07-23_kgarevion-verification-analysis.md`, `2026-08-20_diagnostic-state-trajectory-question.md`

## Why this is archived

This is the stream's first proposed research program element. It survived several rounds of the user dismantling it and changed materially each time. The final form is an **untested proposal**, and it is archived as such.

## The gap in LIT-003

**Source-supported.** LIT-003 is a three-module pipeline: (1) a fine-tuned LLM extracts free-text phenotype mentions; (2) for each string, retrieval-augmented standardization embeds the string, retrieves the ten nearest Human Phenotype Ontology terms, and an LLM picks one; (3) a supervised learning-to-rank model orders the patient's terms by diagnostic informativeness and takes the top k. The authors' own error analysis attributes false positives primarily to ontology granularity (a parent term chosen over the more specific child) and finds that the large majority of false negatives were not extraction failures but arose from how phenotypes are documented, with the model sometimes extracting a semantically related or higher-level concept.

**Inference.** Module 2 makes an irreversible commitment, and the only thing judging that commitment is the model that made it. Module 3 cannot repair it: it can only reorder terms that exist, and a term recorded too generally scores low on rarity and falls below the cutoff. A single granularity error therefore produces a false positive (the parent) and a false negative (the missing child) at once, so fixing granularity would improve precision and recall together, which the top-k curve normally trades against each other.

## The proposal, in its final form

Insert a Review-style verification step (LIT-001) into Module 2 so that the mapping is checked against a disease knowledge graph before the LLM selects, with selection restricted to survivors and cosine similarity as tiebreaker.

**The constraint that reshaped it.** Review needs both slots of a triplet to resolve to graph nodes. The head (a candidate HPO term) is fine. The tail is the problem: a triplet such as (phenotype, present in, disease) needs a disease, and an undiagnosed patient does not have one. The population LIT-003 was built on is undiagnosed by definition.

Four tail candidates were considered:

| Option | Tail | Verdict in stream |
|---|---|---|
| A. Scope to confirmed-diagnosis patients | The known disease | Honest but a retreat; verification becomes a development tool, not a screening tool |
| B. Anchor to the patient's own high-confidence phenotypes | Diseases implicated by the intersection of unambiguous findings | Defensible in principle; bootstraps off phenotypes assumed correct; output is graded rather than binary |
| C. Anchor to the disease family | A class-level node | Cheap to check; class-level annotations may be too sparse to verify anything |
| D. Rank diseases instead of filtering phenotypes | Every disease | A different system (differential diagnosis); does not answer the mapping question |

**The user's proposal, adopted as the stronger design.** Test each candidate term against every disease in a bounded class (for the CIL-FLARE setting, the ciliopathies). Threshold on how many diseases in the class verify:

| Verifies against | Reading |
|---|---|
| none | Flagged: no support anywhere in the family |
| a few | Highly discriminating |
| most | True but non-informative (the "fatigue" case) |

Two properties follow. The count is a within-family inverse document frequency, sharper than the global informativeness signal Module 3 uses. And flagged terms are **kept and marked rather than deleted**, because knowledge-graph coverage of rare disease is sparse and a flag may mean a novel manifestation rather than a wrong mapping. This converts a silent degradation (verification quietly stops working for unmappable entities) into a visible one.

**Cost.** Ten candidates times about twenty diseases per extracted string is a large number of verification calls across a note corpus; mitigation is to precompute the term-by-disease verification matrix once per disease class.

**Circularity, stated concretely.** Verification against a disease anchor presupposes the thing extraction is meant to establish. The class-based design reduces this (the anchor is a family, not a diagnosis) but does not remove it: it still assumes the patient's disease is in the class. Both annotation regimes (literal versus propagated ontology annotations) were traced and gave the right answer in the running example, which is one example, not evidence.

## The complementary thread: context identification (2026-07-23, archived 2026-08-28)

The same night produced design principles for the context-identification direction (the clinical collaborator's five dimensions), which verification cannot supply:

- **Context detection must run upstream of standardization, because standardization is lossy.** By the time Module 2 sees the string, the negation cue is gone. (Inference.)
- **Label negated findings; do not delete them.** An explicitly absent finding is diagnostically valuable. Review cannot verify polarity: negation is a fact about the note, not about biology. (Inference.)
- **Hedged assertions need a data-structure extension.** A triplet has three slots and nowhere to put the clinician's certainty; LIT-002 attaches confidence to edges, but to the evidence supporting a claim, not to the clinician's certainty in asserting it. Related problem, different object. (Inference; pointed to as where a real contribution could sit.)
- **Correction preserved:** the stream first suggested the graph schema's phenotype-absent relation as a slot for negation, then corrected itself: that relation likely encodes disease-level biological absence, not note-level negation.

This thread also created a new dependency the stream named at the time: the composed design now rests on context detection being accurate, which is itself unverified. It is the bridge from this entry to the trajectory entry's modality argument.

## Key excerpts

> **Stream 03:** The constraint, stated precisely: Review needs both slots of a triplet to resolve to graph nodes. The head is fine — it's an HPO term. The problem is only ever the tail. So the brainstorm is really: what else could go in the tail slot?

> **Stream 03:** Your proposal is stronger than mine, and tracing it shows why. [...] Earlier I objected that falling back to cosine rank reduces to "take the top retrieval hit, no KG needed." Here it doesn't, because the KG eliminates candidates on evidence first and cosine only breaks ties among survivors. Filtering then ranking is not the same as ranking alone.

> **Stream 03:** Keep them, marked. Don't delete — KG coverage is sparse for rare disease, so "flagged" may mean novel manifestation rather than wrong mapping, and deleting would systematically prevent you from ever discovering new phenotypic features.

> **User:** Then why exactly are we even adding the [review and re-visit] sections in module 2? I still am unclear about how [it helps].

> **Stream 03:** You've found the real problem, and it's fatal to the granularity claim. [...]

(The last exchange refers to an earlier version of the proposal in which verification ran after selection; the user's objection led to the reordering, verification before selection, that the final form uses.)

## Errors and corrections preserved

- Stream 03 initially claimed the 97% false-negative finding in LIT-003 was an extraction (Module 1) problem that verification could not touch. The paper says the opposite, and the user caught it; corrected to a Module 2 granularity problem, which strengthens the proposal.
- Stream 03 described Review as "fixing" the soft-constraint hole in an early slide; retracted as overstatement (the unmappable entity is retained in the verified set, per the paper).
- Stream 03 initially placed verification after the LLM's selection; the user showed this verifies one term rather than the candidate pool, and the ordering was reversed.
- Stream 03 used "adjacent," "specificity," and "annotation table" without definition; each was later defined, and "specificity" was found to carry three distinct meanings in the material.

## Status

Untested proposal. No implementation, no data run. The design questions still open: whether literal or propagated annotations are used; how to distinguish "wrong mapping" from "poorly annotated ultra-rare disease" among flagged terms; and whether the precomputed matrix reduces to a lookup, which it does not, because Review scores structural position rather than literal edges (the lookup-versus-Review comparison itself was identified as a missing ablation the paper never runs, and remains an open empirical question).

One further open question, added 2026-08-06 when the user's challenge strengthened the proposal's case: of LIT-003's linguistic-variation false negatives, what fraction had the correct term present in Module 2's retrieved top-ten candidates? That single number sets the ceiling on what any verification step inserted at Module 2 can recover, and it is answerable with the paper's released code.

## Relevance to candidates

- **Candidate 02:** this is the concrete neural-plus-symbolic instance the stream keeps returning to; the ontology is the symbolic half.
- **Candidate 04:** the keep-and-flag design is an evaluation and assurance mechanism (surfacing unverifiable output) rather than an accuracy mechanism.
