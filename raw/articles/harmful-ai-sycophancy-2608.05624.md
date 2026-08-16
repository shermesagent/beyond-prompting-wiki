---
source_url: https://arxiv.org/abs/2608.05624
ingested: 2026-08-08
sha256: 73df52ac012947b591805ef4b8dd79ace206a807e2879555133f61ea3ea46f39
---

# Measuring and Detecting Harmful AI Sycophancy

arXiv:2608.05624, August 2026 (LLM measurement / sycophancy detection; 17 open- and closed-source LLMs, 12 everyday-advice domains)

**Full abstract:**

Sycophantic responses are becoming pervasive in large language models (LLMs), and prior work has pointed out that some of them could be harmful. This paper focuses on one harmful sycophancy: preference-induced stance reversal sycophancy (PSRS), where a model reverses an initial stance merely to align with a user's stated preference. While existing research mainly measures how sycophantic a model is, we go further and ask whether PSRS can also be detected automatically from a single response. To investigate this at scale, we introduce CAP (Contrastive Anchor Probing), a framework for collecting labeled PSRS data. Applying CAP to 17 open- and closed-source LLMs, we collect 290,460 labeled responses across 12 everyday-advice domains. We organize our study around three research questions. (1) How often does PSRS occur? (2) How well can it be detected? (3) How does detection generalize to unseen models? We first reveal that PSRS rates range from 5% to 56% across LLMs, with more capable models being less sycophantic. Next, we show that detecting PSRS is feasible from the response text alone, and detectors need to learn subtle PSRS patterns from the training data. Because new LLMs appear rapidly, detectors inevitably encounter unseen models, making cross-model generalization an important framework goal. We demonstrate that detection performance drops on unseen models and propose an initial approach to address this challenge. We will release our dataset and code to support future research.

**Key terms:** preference-induced stance reversal sycophancy (PSRS) · Contrastive Anchor Probing (CAP) · stance reversal 5–56% across models · capability gradient (more capable = less sycophantic) · detection from single response
