# KGARevion: what verification buys, and what the paper does not explain

- **Period:** 2026-07-21 to 2026-07-23 (preparation of a journal-club presentation given 2026-07-23)
- **Source:** LIT-001 (Su et al., ICLR 2025)
- **Related:** `2026-07-23_rare-phenix-verification-proposal.md`, LIT-005 (PrimeKG, the graph used)

## Why this is archived

This was the first close reading in the stream and it produced the architectural principle that later entries build on: let a model generate freely, then check its output against an independent structured source. It also produced a worked example of the stream's failure mode (constructing mechanisms the paper does not supply) and the user's method for catching it (tracing the mechanics step by step and refusing to accept a conclusion that the mechanics do not support).

## Digest

**Source-supported (LIT-001).**

- The agent has four actions: Generate produces candidate triplets from the question (one per answer option in the choice-aware setting); Review maps each triplet's entities to pretrained structural embeddings of a knowledge graph, fuses them with a fixed textual description of the relation, and a LoRA-fine-tuned model emits True or False; Revise takes a False triplet, swaps its head or tail, and resubmits it, up to k rounds; Answer reasons only over the verified set.
- Review is fine-tuned once, offline, on triplet-completion data from the graph. Structural embeddings are frozen. Relation descriptions come from a fixed template table. Nothing updates at inference time.
- Reported effects: removing Review costs about nine accuracy points on multiple-choice benchmarks and about four on open-ended ones, averaged across datasets; removing Revise costs about three points on the MedDDx family; option reordering moves raw LLM accuracy by roughly 8 to 16 points but the agent by roughly 1.5 to 4; swapping the underlying graph (PrimeKG to OGB-biokg) changes accuracy from 0.69 to 0.67.
- Unmappable entities (absent from the graph) are retained as "incomplete knowledge" rather than rejected.

**Inference (stream 03, with user's corrections).**

- Because every input to Review is deterministic for a given triplet, Review is a pure function of (head, relation, tail). Resubmitting the same triplet yields the same verdict. Revise therefore cannot rescue a Review false negative; it can only produce a different fact.
- The transferable idea is the architecture, not the component: a generator cannot be its own judge, and the graph is used to verify rather than to retrieve, which is why swapping graphs barely moves performance.
- Review does more than a lookup: it scores triplets that are not literal edges, using structural position (the running example verified a family-level triplet with no direct edge).

**Unresolved.** The paper reports Revise's benefit on the hardest MedDDx subset and describes its purpose only as covering more concepts. Four candidate mechanisms were proposed in this stream and each failed under scrutiny (table below). The stream's position at archiving is that no defensible mechanism exists in the paper or in the stream's own reasoning, and the benefit should be reported as an unexplained empirical result.

## Limitations found

1. **The soft-constraint hole.** An entity the graph has never seen rides into the verified set unverified. In the running example the distractor gene absent from the graph was never rejected.
2. **Revise's mechanism is unexplained** (see table).
3. **TransE-style embeddings handle hierarchy poorly**, which matters if the method is applied to an ontology where parent-child is the relation of interest.
4. **The headline ablation numbers are averages** across seven datasets; gold-standard and MedDDx subsets point in opposite directions.

## The four explanations for Revise, and why each failed

| # | Proposed mechanism | Why it fails | Who broke it |
|---|---|---|---|
| 1 | Revise repairs a wrong candidate into the right one | Generate already proposes the correct entity's triplet independently, one per option; nothing needs to be reached | User |
| 2 | Revise is a safety net for Review false negatives | Malformed triplets land in the unmappable branch, not the False set, so they never reach Revise; and Revise swaps head or tail, so it moves away from the original entity rather than re-verifying it | User |
| 3 | Revise expands the concept set beyond the generated triplets | True as a description, but a verified fact about an unrelated entity does not restore evidence for a correct candidate whose own triplet was misclassified | User |
| 4 | Revise gives a second independent shot at Review | Review is deterministic: same triplet, same verdict; there is no second shot | User, via the fine-tuning question |

## Key excerpts

> **User:** I can't think of any scenario where [Revise] is even needed. Can you? If so, can you tell me when revise gets properly [used]?

> **Stream 03:** Fine-tuning is offline and one-time. Review's LoRA fine-tuning happens once, before deployment, on PrimeKG triplet-completion data [...]. At inference the weights are frozen. Nothing updates between rounds — there's no online learning anywhere in the loop. [...] Same triplet → same Z → same forward pass → same verdict. [...] Revise cannot recover a Review false negative. Full stop. [...] I should stop here rather than construct a fourth explanation. Across this conversation I've offered three mechanisms for Revise's measured benefit on MedDDx-Expert, and you've correctly taken apart each one. The paper reports the number and describes Revise's purpose only as covering "more medical concepts" — it never explains the mechanism, and I don't have one I can defend.

> **Stream 03:** What survives is narrow and worth keeping that way for the talk: Revise is the only route by which concepts outside T enter V; MedDDx-Expert is where T carries the least discriminating signal; the ablation shows extra rounds help there. Those three facts sit next to each other. The causal link between them is not something the paper establishes or I can supply.

## Errors and corrections preserved

- Stream 03 asserted that Review's inputs collapse to a single distinguishing row ("byte-identical" claim) and retracted it the next turn as an overstatement.
- Stream 03 introduced an entity (HSPA5) into a worked example that did not come from the paper, and later stated plainly that it was invented for illustration.
- Stream 03 proposed the "safety net" and "second shot" mechanisms and withdrew both. The retraction is above.
- Stream 03 stated the reordering-robustness result compared the same system under two conditions; the user asked whether it held, and it did (two different systems are measured, raw model versus agent), so that claim stands.

## Relevance to candidates

- **Candidate 02 (neuro-symbolic + metacognitive):** LIT-001 is a concrete instance of neural generation plus symbolic verification. Its unexplained component is a caution against treating "add a verifier" as sufficient.
- **Candidate 04 (evaluation, verification, safety):** the reordering result is an evaluation finding about reliability rather than accuracy, and the determinism argument is a reproducible property worth exploiting in evaluation design.
- **Family 5 (biomedical KG + LLM reasoning):** the graph-independence result argues that the graph matters as a verification substrate, not as a retrieval source.
