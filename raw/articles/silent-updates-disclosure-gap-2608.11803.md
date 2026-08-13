---
source_url: https://arxiv.org/abs/2608.11803
ingested: 2026-08-13
sha256: 30040776b3c7980041067242691ecc43b9e696c11ff2a59f3730ddd1977a5207
---

# Silent Updates: Measuring and Closing the Post-Deployment Disclosure Gap

arXiv:2608.11803v1, AI governance / model deployment (published 2026-08-12)

**Authors:** Sophia Abraham, Ben Bucknall

**Full abstract:**

Deployed foundation models are often not static systems, with providers able to modify system behavior through fine-tuning, classifier updates, system prompt revisions, retrieval changes, and routing changes. These updates can be made silently -- that is, without public disclosure, a version increment, or re-evaluation. Such silent updates challenge a core assumption behind current AI governance frameworks that an externally verifiable chain of custody links the model referred to in evaluation results or a system card to the model served to users. In this paper, we examine post-deployment disclosure practices across first-party API providers and inference hosts to establish the extent to which a chain of custody exists in practice. We find that providers commonly publish substantial safety documentation, including quantitative evaluations and version-specific reports, but no provider in our sample published information allowing an external party to verify that the artifact being served is the same one referred to in this documentation. We introduce the Silent Updates Scorecard, a public instrument for measuring post-deployment disclosure practices across providers and hosts, and preliminary results for a sample of nine first-party API providers and seven third-party inference hosts. We also propose a Three-Part Behavioral Trigger System for determining when post-deployment modifications to a system motivate disclosure or re-evaluation obligations.

**Key terms:** silent updates · post-deployment disclosure gap · chain of custody · Silent Updates Scorecard · Three-Part Behavioral Trigger System · version verification
