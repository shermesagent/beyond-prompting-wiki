---
source_url: https://arxiv.org/abs/2607.19355
ingested: 2026-07-23
sha256: infodiscern-2026-placeholder
---

# Information Discernment in Large Language Models

arXiv:2607.19355, July 23, 2026

LLMs are increasingly used with external knowledge sources like the internet. Do they weigh information appropriately — updating more for reliable sources (source discernment) and more when claims bring priors closer to the truth (truth discernment)? We formalize this as information discernment and introduce Learn2Discern (L2D), an experimental framework and benchmark grounded in three normative axioms with interpretable metrics.

Across 13 models and nearly 670K trials, we find consistent failures across both dimensions: models perform near chance on source and truth discernment, rely on source popularity twice as much as source reliability, and update roughly equally whether a claim improves or worsens their position relative to the ground truth. Models integrate external knowledge most effectively on datasets where their priors are already the most accurate. Newer and larger models improve truth discernment but not source discernment, a blind spot that model complexity does not address.

A pre-registered, quota-matched user study (n=299) confirms that real LLM users endorse all three axioms and report that violations reduce their trust and usage intent.

Key findings:
- Near-chance source discernment across all 13 models
- Popularity weighted 2x over reliability
- Truth discernment improves with scale; source discernment does not
- Users' trust drops when discernment failures are exposed
