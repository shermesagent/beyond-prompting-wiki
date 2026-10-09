---
source_url: https://arxiv.org/abs/2610.11025
ingested: 2026-10-09
sha256: 16f0bb6e8c8c73498858c5d44324ac6c9290eda143545e1485777f0ea318aa0d
---
# Intent Graph: Navigating the Analytical Reasoning Space for Exploratory Data Analysis

Authors: Junran Yang, Shruti Badrish, Teanna Barrett, Leilani Battle. Submitted 2026-10-08; announced in October 9, 2026 arXiv RSS (new preprint). Source: https://arxiv.org/abs/2610.11025

Primary abstract (verbatim except whitespace normalization): Exploratory data analysis (EDA) is rarely open-ended in practice: analysts work from high-level domain questions toward the concrete analyses that can answer them, prioritizing directions with domain knowledge and prior hypotheses. Large language models (LLMs) can supply such knowledge, but their responses are unstructured, leaving analysts no way to see what has been explored, what is missing, or why one direction was chosen over another. We present DAG-EDA, a system that lets analysts and an LLM co-navigate the space of possible analyses through two linked structures. An intent graph, governed by a grammar of analytical intent, decomposes an ambiguous natural-language question into progressively concrete analysis tasks, keeping alternative framings open and letting analysts branch, backtrack, and compare paths. A multi-layered knowledge graph externalizes the LLM's domain knowledge, linking domain concepts to the dataset variables that can measure them, so analysts can inspect and contest how their question is grounded in the data. Both graphs are constructed from only the dataset and the analyst's question, and the analyses the analyst reaches are rendered as interactive dashboards. We illustrate the system through a usage scenario and describe a user study design for examining whether the system scaffold analysts' reasoning and navigation.

Practical translation (editorial, not a tested intervention): A proposed analytic interface makes alternative questions and dataset mappings visible; evaluation is planned, not demonstrated.
