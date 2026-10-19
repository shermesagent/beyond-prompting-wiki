---
source_url: https://arxiv.org/abs/2610.23304
ingested: 2026-10-19
sha256: 9b3024afb6c8323afbd96dc3b55c355713971375933c04fd5e11edc4788c2be7
---
# Designing for Imperfect Prompts: A Simulation-Based Evaluation of an LLM-Based Enterprise Data Assistant Using Knowledge Graphs

Publisher: arXiv (preprint, version 1)
Published: 2026-10-16
Authors: Niklas Wagner, Alexander Mädche

## Publisher abstract (full text not reviewed)

Enterprise data assistants using large language models (LLMs) promise democratized data access in organizations. Yet in our real-world deployment within the CFO unit's data lake at an industry partner, we observed that business users frequently pose imperfect prompts that include domain-specific vocabulary and lack schema references or structural information. This Design Science Research study examines automatic resolution using a semantic mediation layer. We design and evaluate two design variants: schema-based mediation via semantic similarity, and knowledge graph-based mediation leveraging an automatically constructed knowledge graph from the data lake. Our simulation-based evaluation using real-world data, supported by LLM-as-a-Judge assessments and human validation, shows that knowledge graph-based mediation outperforms the schema-based approach in Precision, Recall, F1, and preserving user intent. We propose a design principle for knowledge graph-based mediation, demonstrating that structured knowledge representation bridges user intent and database structure and guides the design of enterprise data assistants across skill levels.

## Curator note (interpretation, not source text)

Real CFO-unit deployment informed a simulation-based comparison: a knowledge-graph bridge between business language and database structure outperformed a schema-similarity approach on the reported metrics, with human validation alongside model judging. Try a small approved dictionary mapping work terms to public-data column names; do not assume better simulated matching guarantees safe production answers.
