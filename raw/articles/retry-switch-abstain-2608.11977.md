---
source_url: https://arxiv.org/abs/2608.11977
ingested: 2026-08-14
sha256: 6ab0762dcdc010e53f2fcbcab9f6c8fa2459bc3683c6d2d8ac94c883ac49bf34
---

# Retry, Switch, or Abstain? Learning Strategy-Aware Tool-Use Policies via Controlled Error Injection

arXiv:2608.11977v1, 2026 (LLM agents / tool-use robustness, published 2026-08-12)

**Authors:** Chaoran Chen; Vy Nguyen; Ziji Zhang; Abhinav Gullapalli; Ziyi Wang; Yuxuan Lu; Dakuo Wang; Jing Huang; Zhou Yu; Jin Lai

**Full abstract:**

Tool-using LLM agents are commonly trained and evaluated in environments where tool calls succeed reliably, yet deployed tools can fail transiently, persistently, or silently. Robust recovery therefore requires more than repeated retries: an agent may need to retry the same path, switch to an alternative, or recognize that no viable path remains. We present BENCH2ROBUST, a framework that converts failure-free tool-use benchmarks into controlled stochastic environments with scenario-controlled solvability, where episodes explicitly require retrying, switching, or stopping after available paths are exhausted. We use BENCH2ROBUST to study two complementary interventions: structured runtime recovery context through Bayesian Tool Memory (BTM), and curriculum-controlled reinforcement learning. Across 7 models from 4 families and two multi-turn benchmark families, tool failures produce a near-universal robustness gap. On held-out Retail tasks, BTM improves robustness by up to 16.8 percentage points without retraining, while RL learns complementary recovery behavior that remains beneficial without inference-time BTM. Combining the two reaches 40.8-45.5% under injection while preserving failure-free performance. These results suggest that robust tool use benefits from combining environment-specific recovery knowledge with learned recovery behavior.

**Key terms:** tool-use agents · BENCH2ROBUST · Bayesian Tool Memory · retry/switch/abstain · robustness gap · curriculum-controlled RL
