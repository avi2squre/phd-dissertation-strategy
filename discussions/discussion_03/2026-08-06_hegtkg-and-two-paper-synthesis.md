# Provenance-anchored generation, and the two-paper synthesis: verify-after versus supply-before

- **Period:** 2026-08-03 to 2026-08-06 (preparation of a journal-club presentation given 2026-08-06)
- **Sources:** LIT-002 (HEG-TKG), LIT-004 (ChronoMedKG), LIT-001 (KGARevion)
- **Related:** `2026-07-23_kgarevion-verification-analysis.md`

## Why this is archived

This entry holds the stream's clearest statement of a research framing that neither paper states: that LIT-001 and LIT-002 make the same diagnosis (parametric memory is unreliable for a specific class of output) and adopt opposite strategies, and that the strategies cover different error classes. It also archives an independent second-reader critique of the stream's own summary report, which caught four errors.

## Digest of LIT-002

**Source-supported.**

- Setting: five frontier models on 36 clinician-validated scenarios across three neuromuscular disease pairs. Without citation prompts, no model returned a clinically relevant PubMed identifier. With a single instruction to cite, models produced on the order of hundreds of identifiers per model, of which roughly 79 to 83 percent resolved to real papers in the wrong specialty and 6 to 8 percent did not exist. The strongest citation-prompted model reached 15.3 percent relevance.
- The system attaches provenance (PubMed identifiers), quality tiers, and temporal anchors to graph edges, and the synthesis model copies identifiers from context rather than generating them. Its output-cited identifiers resolved at 100 percent versus 0 percent for both baselines.
- Three neurologists rated verifiability significantly higher for the system; the temporal-precision dimension did not reach significance for any rater.
- A second-order audit found only about half of cited claims directly entailed by the cited abstract, with most of the rest neutral and a small fraction contradicted.
- Blind LLM judges rated the citation-free baseline highly on verifiability with inter-rater agreement below chance; given a PubMed audit, the same judges reversed. The authors' own construction was by a single annotator without inter-annotator agreement, and most retrieved evidence sits in the lowest tier.

**Inference (stream 03).**

- The retrieval baseline was denied identifiers by design, so the paper does not establish that graph structure is required for traceability. The defensible claim is narrower: citation identifiers must travel with the evidence to the point of synthesis; a graph does that naturally, and a retrieval system can if built for it.
- Tier labels record how a claim was found, not how established it is.
- The privacy-compliant configuration (local models) is the least tested, which matters for any enclave deployment.

## The synthesis

**Inference, stream 03's own framing.** Mechanically the two papers are opposites: LIT-001 generates first and verifies after with a fine-tuned classifier; LIT-002 supplies identifiers first and the model transcribes, with no verification step. What is shared is one level up: both identify a class of output that parametric memory is unreliable for (facts in one case, identifiers in the other) and route around it by sourcing that output externally. The strategies are complementary rather than equivalent. Supplying identifiers eliminates fabrication (a model copying from context cannot invent an identifier that was not there) but does nothing about misattribution (a real identifier attached to a claim the paper does not support), which is exactly what the second-order audit found. A Review-style check is the mechanism for misattribution, and LIT-002 has none at inference time. A system with both would supply identifiers and verify the attachment; neither paper does both.

**Surface-form observation (inference).** LIT-002's feature-matching substring method has a high false-negative rate, and LIT-003's false negatives are dominated by linguistic variation. These are the same error class in two different tasks: exact-string matching against clinical language.

**Attribution stated in the stream.** From the papers: every number, both architectures, both papers' own arguments. From the stream: the verify-after versus supply-before framing and the complementarity argument; the class-based verification proposal (`2026-07-23_rare-phenix-verification-proposal.md`); the surface-form observation. Not the stream's: the substring-matching problem, the single-annotator curation, and the disease-scope limits, all conceded by the authors.

## Comparison with LIT-004

The same group's temporal knowledge graph operates at far larger scale with a public benchmark and external validation against a curated resource. The stream's assessment was that, choosing fresh, LIT-004 is the methodologically stronger paper for the temporal question, while LIT-002 has the more striking single result. LIT-004 was not presented; it was read for comparison and positioned as the natural next step. Both papers name PrimeKG (LIT-005) as inadequate, one for coverage and one for lacking a temporal dimension, which connects to the July finding that verification is only as good as the underlying graph.

## Key excerpts

> **User:** "The line to land: the model never generates a PMID — it copies one already in its context. That explains 100% vs 15.3%, and it's the same principle as KGARevion's Review" how is it the same as KGARevion's review?

> **Stream 03:** It isn't, and I overstated it. [...] What's actually shared is a level up: both papers identify that parametric memory is unreliable for a specific class of output, and route around it by sourcing that output externally. KGArevion for facts — don't trust the claim, check it. HEG-TKG for identifiers — don't ask for a PMID, hand one over. Same diagnosis, opposite strategies: verify-after versus supply-before. And the more interesting point — they're complementary, not equivalent.

> **Stream 03:** It lands on a proposal, not a summary. A system with both would supply identifiers and verify the attachment. Neither paper does both. [...] And state one thing plainly: this is your framing. Neither paper describes itself this way, and HEG-TKG doesn't cite KGArevion.

> **Stream 03:** "Graph structure is required for traceability" doesn't follow from their experiment, because their RAG arm was denied identifiers. [...] The defensible claim: citation identifiers must travel with the evidence to the point of synthesis. A graph does that naturally. RAG can too, if built for it.

## Errors and corrections preserved

- Stream 03 claimed identifier transcription was "the same principle" as LIT-001's Review; retracted (excerpt above) and replaced with the synthesis.
- Stream 03 attributed one model's citation counts to "prompted models" generally; the user corrected it to a single model, and the generalization was restated as a range across the three prompted models.
- Stream 03 supplied a convenience value ("~4.9") for a clinician-rated dimension that was not in the paper; the user lost time searching for it. Rule adopted: state where every number comes from (paper, derived, or inferred) before it is used.
- Stream 03 built a hypothesis about the synthesis model's behavior over several turns and abandoned it after reading the full system prompt in the supplement.
- Stream 03 claimed one output-type routing stage that does not exist in the pipeline as specified; corrected on reading the supplement.
- An independent second reader reviewed the stream's summary report and identified four errors the stream had missed. The user's conclusion, adopted by the stream: do not use the same model to verify its own work. This is now project practice and is the reason the repository has independent streams.

## Relevance to candidates

- **Candidate 04 (evaluation, verification, safety):** the LLM-judge inversion result and the second-order (entailment) audit are evaluation-design findings: verifiability must be measured against an external resolver, not by a model's assessment.
- **Candidate 02:** the supply-plus-verify system sketched above is a concrete neural-plus-symbolic architecture that no examined paper implements.
- **Candidate 01 (trustworthy agentic AI):** provenance that travels with evidence to the point of synthesis is a system-design requirement for any agentic clinical workflow.
