---
source_url: https://arxiv.org/abs/2607.26191
ingested: 2026-07-30
sha256: e70461e76891fc7cdac8f328d32291ba102bc84bc04199ff4e12852e8c8e604d
---
# Trust Inflation in Evaluation

**arXiv:** 2607.26191
**Date:** 2026-07-30
**Domain:** cs.AI (Artificial Intelligence)

## Abstract

Evaluation methodologies for language models increasingly combine multiple signals, from automated metrics and LLM-as-judge ratings to human assessments and benchmark suite results. When these signals are aggregated via averaging, evaluation confidence can then substantially exceed the reliability of the weakest signal: a phenomenon we call trust inflation in evaluation. We argue that evaluation scores should be treated as epistemic claims with three properties: formality (human evaluation provides stronger evidence than an automated metric), scope (a benchmark result applies to the tested distribution, not universally), and validity windows (benchmark results expire as contamination accumulates and distributions shift). Several converging research traditions (chain-of-thought analysis, possibilistic logic, and algebraic theory) establish weakest-link aggregation as the conservative endpoint of a parameterized operator family controlled by a single pessimism parameter. Drawing on those traditions, and on concrete lessons from building an evaluation harness for agentic AI, we propose that evaluation results carry explicit metadata (formality tier, scope declaration, and expiration date) to make their epistemic status transparent. We illustrate the cost of mean aggregation on the public HELM leaderboard: across 54 frontier models on ten scenarios, the top-five models ranked by mean score and by weakest-link are completely disjoint.

## Key Findings

- "Trust inflation": mean aggregation of evaluation signals produces confidence exceeding weakest signal reliability
- Top-5 models by mean score vs. weakest-link are completely disjoint (54 models, 10 scenarios)
- Evaluation scores should carry metadata: formality tier, scope declaration, expiration date
- Weakest-link aggregation is the conservative endpoint of a parameterized pessimism family
- Human evaluation provides stronger evidence than automated metrics (formality hierarchy)

## Relevance

Directly relevant to Trust Calibration — extends the calibration challenge from "can I trust this output?" to "can I trust this leaderboard?" The finding that top-5 by mean and top-5 by weakest-link are completely disjoint is jarring and practical. Also relevant to The Certification Boundary: evaluation is the certification mechanism for AI capabilities, and trust inflation means that certification is systematically overconfident.
