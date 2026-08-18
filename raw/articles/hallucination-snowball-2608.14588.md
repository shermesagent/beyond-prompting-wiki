---
source_url: https://arxiv.org/abs/2608.14588
ingested: 2026-08-18
sha256: 6d42538f8c3b0cdbe77edfa8cdf3e64d4e2871aa4ed53fecce912199d25f481e
sha256: PENDING
---

# The Hallucination Snowball: Modeling Error Propagation as State Transitions in Multi-Agent LLM Pipelines

arXiv:2608.14588v1, 2026 (published 2026-06-22)

**Authors:** Prabhjot Singh; Bhushan Pawar

**Full abstract:**

Sequential multi-agent LLM pipelines chain specialized agents without verification at handoffs, creating a structural flaw with measurable and severe consequences. We show that hallucinations injected at Stage 1 do not merely persist; they transform: raw numerical facts become derived computations, then narrative prose, then editorially approved conclusions. At each transformation, detectability degrades near-irreversibly. We formalize this as the hallucination snowball effect, a first-order Markov process over four states (Raw Fact → Derived → Narrative → Invisible) with empirically measured per-boundary escape probabilities of 24.6%, 48.3%, and 89.3%. Across 346 automatically injected hallucinations in a 4-agent financial analysis pipeline on FinanceBench, gpt-4o detection drops from 72.0% at Stage 1 to 50.9% at Stage 4, and 23.7% of hallucinations survive completely undetected in the final output. Even the strongest model tested (Qwen3.5-397B-A17B, 87.0% at Stage 1) faces a structural ceiling; projected Stage 4 detection is only ~60–65%. Critically, boundary gates using identical RAG verification tools reduce hallucination survival from 58.4% to 16.2% versus end-of-pipeline checking (Cohen's h = -0.911, p < 0.000001), while end-checking alone achieves merely 2.3 pp improvement over no verification. When you verify matters more than whether you verify. Our model predicts survival for n-agent linear pipelines and prescribes optimal verification resource allocation: invest at S1→S2 first, where 75.4% of hallucinations are still catchable, not at S3→S4 where 89.3% have already escaped.

**Key terms:** hallucination snowball · multi-agent pipelines · verification at handoffs · Markov state transitions · boundary gates
