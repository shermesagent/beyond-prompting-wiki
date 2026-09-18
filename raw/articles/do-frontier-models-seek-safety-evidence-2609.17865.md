---
source_url: https://arxiv.org/abs/2609.17865
ingested: 2026-09-18
sha256: 635617dbaecfb6f7ae7a2316b46e7b481b09b448fa600a8122f401c30c7e2ace
---
# Do Frontier Models Seek Safety Evidence Before Acting?

- Source URL: https://arxiv.org/abs/2609.17865
- Source type: Research paper
- Date: 2026-09-15
- Ingested: 2026-09-18
- Authors: Omer Tafveez

## Abstract / Summary

Frontier models are often evaluated on how they respond to safety information once it is already in context. We study an earlier decision point: whether models choose to acquire safety-relevant evidence before acting. We introduce SAFE, a controlled benchmark in which models make deployment decisions with optional evidence that varies in retrieval cost, probability, severity, and presentation. Across GPT-5.5, o3, Claude Opus 4.8, and Claude Sonnet 4.6, we find distinct evidence-acquisition policies: Opus inspects nearly by default, o3 is the most skip-heavy and threshold-sensitive, and GPT-5.5 and Sonnet occupy intermediate regimes. Inspection increases strongly with severity and decreases with retrieval cost, whereas probability has much weaker behavioral influence. These results suggest that deployment-time safety depends not only on how models respond to known risks, but also on whether they acquire the evidence needed to know that acting is safe.

## Beyond Prompting Translation

Before an AI acts, the useful question is not just whether it can use evidence. It is whether it goes looking for the evidence it needs when looking costs time, effort, or convenience.

## Practice Hook

Use this source to strengthen practice routines that require visible evidence, source independence, state-specific approval, and saved reasoning — not just smoother AI output.
