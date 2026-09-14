---
source_url: https://arxiv.org/abs/2609.11977
ingested: 2026-09-14
sha256: 07bd64c3f310643c36fe8d3786e7cb1bfc7a9069000ccb8511704aaf39a6bdf4
---

# Occamy-1.0: Open Pareto-frontier 35B Intelligence for Co-work

**Source:** https://arxiv.org/abs/2609.11977  
**Date:** 2026-09-04  
**Authors:** Wenhui Chen et al.

## Abstract

Co-work agents execute complex workflows that combine information gathering, tool use, coding, and file manipulation across many model invocations. Because cost and latency accumulate over the full episode, their practical value depends not only on peak capability but also on how efficiently that capability is delivered. Yet many steps in everyday work emphasize state tracking, coordination, recovery, and follow-through rather than frontier-scale reasoning. We present Occamy-1.0, a cost-efficient co-work model obtained by further training the post-trained Qwen3.6-35B-A3B checkpoint. We construct execution-grounded data and environments, capture replayable long-horizon trajectories across multiple harnesses, and use staged post-training to develop and consolidate complementary execution capabilities. Across a broad suite of co-work benchmarks, Occamy-1.0 is consistently among the strongest comparably sized models and remains competitive with substantially larger frontier systems on several tasks. Under our stated evaluation and pricing protocol, its aggregate performance across four representative benchmarks places it at the low-cost knee of the observed cost--performance Pareto frontier. Supporting evaluations in tool calling, coding, and instruction following further show that this specialization preserves broad agentic capability. We release the model weights and a subset of the training data to support research on practical co-work agents and agentic post-training.

## Beyond Prompting takeaway

Real co-work is not just hard reasoning. It is state tracking, coordination, recovery, follow-through, and cost control over a long episode. The useful question for professionals is not “which model is smartest?” but “which system can keep working, recover cleanly, and stay worth the cost?”
