---
source_url: https://arxiv.org/abs/2609.01852
ingested: 2026-09-03
sha256: bec85678df6c36df947b8e8622c6b3ccf423924849a2775db3d7d2093887ca15
---
# The Memory Trust Gap: Capability-Dependent Failures in Persistent-Memory Agents

**Source:** arXiv:2609.01852 (Hu & Ramachandran), published 2026-09-01

**Summary:** Persistent memory supports personalized agents — but a stale stored fact can override current authoritative evidence *without warning*. This paper studies when that harm begins as model capability changes, using a frozen, closed-set, action-scored benchmark with two suites that represent two different meanings of "no memory":

- A **Benefit suite** (unsolvable without the stored fact)
- A **Safety suite** (an authoritative tool always holds the correct value)

The authors evaluate a same-family model-size series (Qwen3 0.6/1.7/4/8B). Key findings:

- The **Memory Trust Gap reflects over-trust, not confusion.** In the Benefit suite, models answer with the stale value 0.92–1.00 of the time at every scale.
- In the Safety suite, harm below the no-memory baseline is **capability-gated**: the larger models collapse most once a stale note is made to look current.
- In a 2×2×2×2 factorial, which feature triggers over-trust depends on both the feature and model scale. **Removing a label amplifies over-trust at every size; a recency feature (stale note dated newer) fools the larger models harder. Source authority is weak and scale-flat**, and position changes sign across the model-size series.
- Mitigation is likewise capability-dependent: **exposing metadata improves accuracy for the capable models, but only pre-resolving the conflict restores accuracy for the two smaller checkpoints.** The pattern replicates on an independent Llama-Instruct series and two external datasets (RGB, MisBench).
- A framing control finds no consistent advantage for the memory label: at the three smaller scales, models trust a stale *document* more than a stale *memory*; at 8B the difference is not significant.

**Key takeaways for the wiki:**
- When an agent has memory, the stored past can outrank the live source of truth — silently, and more often the more capable the model.
- A stale note that *looks current* is the dangerous case: recency dressing fools bigger models hardest.
- The only mitigation that worked at every model scale was pre-resolving the conflict before the agent acts. Exposing metadata helped only the capable models.
- For humans delegating to memory-equipped agents: ask the freshness question, expose metadata where you can, and pre-resolve stored-vs-live conflicts for anything consequential.
