---
source_url: https://arxiv.org/abs/2609.00652
ingested: 2026-09-04
sha256: 38d739316106cf7be948e6262f59460084385cad97839004e77f224f4d1207d8
---
# Self-Reports Are Not Verification: Environment-Grounded Auditing of LLM Operators

**Source:** arXiv:2609.00652 (Pan, Zhou & Hu), published 2026-09-01

**Summary:** Language-model agents increasingly propose actions, observe external feedback, and explain their own behavior. Their stated confidence and rationales are convenient monitoring signals — but **convenience is not verification**. The paper builds an environment-grounded audit in which every intermediate proposal receives an exact outcome: an LLM operates an evolutionary Contexto search whose feedback function assigns every valid guess an exact rank, with no human annotation. Across 200 runs spanning five configurations and three model families, four reporting configurations produce 12,249 self-reports.

Three assumptions get tested — and **all three fail**:

1. **Stated confidence is calibrated?** No. Operators overstate top-100 success by factors of **4.8 to 9.3**, and calibration and discrimination dissociate across model families.
2. **Inherited rationales affect later proposals?** Barely. Controlled interventions on 754 inherited rationales bound any measured benefit of the genuine rationale to roughly 250 ranks.
3. **Fitness-based selection improves report quality?** No detectable selection differential or parent-to-offspring transmission in report accuracy — despite sharply different search behavior.

**Bottom line:** agent self-reports — "I'm confident this worked," "here's why I did that" — are **claims to verify against the environment, not evidence of their own reliability**. The check has to come from the outcome, not the agent's account of itself.
