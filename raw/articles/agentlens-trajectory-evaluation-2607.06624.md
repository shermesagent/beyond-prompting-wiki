---
source_url: https://arxiv.org/abs/2607.06624
ingested: 2026-07-09
sha256: <to be computed>
---

# AgentLens: Production-Assessed Trajectory Review Benchmarks

**Authors:** Anonymous (2026)
**arXiv ID:** 2607.06624
**Published:** July 7, 2026

## Abstract

AgentLens is a benchmark for evaluating AI coding agents that reviews the entire trajectory (the full sequence of actions, tool calls, and decisions), not just pass/fail on the final output. The benchmark pairs formal verification (did the agent produce a correct result?) with LLM-written trajectory reviews that explain why the score is what it is. Each run yields a readable explanation diagnosing where the agent succeeded, where it went wrong, and what it could have done differently. The approach is used to compare agent versions, diagnose progressive tasks where errors compound, and detect regressions in subtler dimensions like code quality and test coverage that pass/fail alone can't surface.

## Key Findings

- Pass/fail evaluation misses trajectory quality — an agent can produce correct output via a terrible path
- Formal verification + LLM trajectory review = readable diagnostic per run
- Progressive tasks (long horizon) are where trajectory evaluation matters most
- Enables comparison of model versions on process quality, not just outcome
