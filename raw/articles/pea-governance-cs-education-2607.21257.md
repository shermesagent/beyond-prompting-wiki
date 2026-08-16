---
source_url: https://arxiv.org/abs/2607.21257
ingested: 2026-07-25
sha256: 0a570be570f211c90c2d3bb0d768e02403bde9eb529945003de435f9e8970c06
---
# Exploring the Design Space of LLM-Based Programming Support in CS Education: A Scoping Review through the Lens of Assistance Governance

- **Title:** Exploring the Design Space of LLM-Based Programming Support in CS Education: A Scoping Review through the Lens of Assistance Governance
- **arXiv ID:** 2607.21257
- **Date:** 2026-07-24 (new)
- **Authors:** Multiple (cs.HC)
- **URL:** https://arxiv.org/abs/2607.21257
- **Source type:** research_paper
- **Status:** active

## Abstract

As large language models (LLMs) become integrated into programming education, learner-facing systems increasingly differ in how that assistance is bounded, enacted, and controlled. These governance decisions are often described implicitly, making it difficult to compare systems in educationally meaningful ways. To address this gap, we conduct a scoping review and qualitative synthesis of 90 peer-reviewed LLM-based programming support systems in CS education. We analyze assistance governance through three dimensions, which we refer to collectively as PEA: Policy, capturing what forms of help are allowed or restricted; Enforcement, capturing how those boundaries are operationalized through interaction and system behavior; and Authority, capturing who can configure, adapt, or override them during use. Our findings show that systems often share similar pedagogical goals, but implement those goals through varied enforcement mechanisms. At the same time, authority remains highly centralized in system logic, with fewer systems giving learners or instructors runtime control. This work contributes PEA as a three-dimensional analytic lens, a governance codebook empirically refined within these dimensions, and a map of underexplored configurations in the current design space of LLM-based programming support.

## Key findings

- PEA framework: Policy (what help is allowed), Enforcement (how boundaries are enforced), Authority (who can configure/override)
- 90 systems analyzed — similar goals, different enforcement
- Authority is highly centralized; few systems give runtime control to users
- The framework applies beyond CS education to any AI-assisted workflow
- Underexplored: user-configurable assistance governance

## Relevance to beyond-prompting

The PEA framework gives orchestrators a vocabulary for designing delegation boundaries. When you set up a pipeline, you're making governance decisions: what help is allowed (Policy), how those boundaries are enforced (Enforcement), and who can override them (Authority). Moving beyond prompting means being intentional about all three, not just hoping the AI behaves.
