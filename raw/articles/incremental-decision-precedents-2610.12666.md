---
source_url: https://arxiv.org/abs/2610.12666
ingested: 2026-10-12
sha256: ef49c1676be64369a0d68dde8afe7e85ca7aa4d18a078324057c744105961327
---
# Incremental Retrieval-Augmented Generation for Human-in-the-Loop Decision Support

Authors: Federico Mazzoni, Andrea Failla. Submitted 2026-10-08; found in October 12, 2026 arXiv cs.HC RSS (new preprint). Source: https://arxiv.org/abs/2610.12666

Primary abstract (verbatim except whitespace normalization): We introduce iRAG, a human-in-the-loop decision-support system combining Retrieval-Augmented Generation (RAG) with Hybrid Decision-Making. Unlike conventional RAG systems, relying on static Knowledge Bases (KBs), our proposal addresses settings where the KB is initially empty and is progressively populated through human decisions. The system stores previous decisions as retrievable precedents and moves from silent observation to evidence-grounded contestation and, finally, to autonomous handling with abstention. Against an independent baseline, iRAG matches final-decision error under 10% drift without retrieval decay and reduces it under 40% drift across all configurations. Retrieval decay improves performance on changed knowledge while increasing error on stable knowledge, evidencing a stability--plasticity trade-off rather than a general advantage. Human oversight is an architectural provision of the workflow; its usability with real human users remains to be evaluated.

Practical translation (editorial; not a tested intervention): keeping an approved decision, reason, and expiry condition alongside each repeatable recommendation.
