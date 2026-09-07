---
source_url: https://arxiv.org/abs/2609.04373
ingested: 2026-09-07
sha256: b88c28a166084ae1b2ad83bc6ba721dcab8933e59d9453b146a4944e8c218402
---
# Why Better Models Can Create Riskier Systems: Evidence from LLM Agents in Financial Markets

**Source:** arXiv:2609.04373 (Ross, So, De Simone, Pozniak & Lo), published 2026-09-03

**Summary:** LLMs are being deployed at scale in consequential real-world systems — financial markets, content moderation, hiring. This paper shows that **improving individual model capability can degrade rather than improve system-level outcomes**. The mechanism is correlation: shared training and architectures lead more capable LLMs to behave *more* similarly, creating correlated actions that do not diversify away.

The authors build a general framework showing how this correlation creates a **non-diversifiable risk floor**, then test it in financial markets with an agent-based simulation of LLM traders at varying capability levels. Three findings:

1. **Frontier LLMs exhibit significantly correlated behavior that increases with capability.** The smarter the models, the more they think alike.
2. **When their shared reasoning is accurate, more agent participation reduces market-level risk.** Correlation is only dangerous when it is correlated *error*.
3. **When agents share a common misinformation environment, the same correlated behavior becomes a liability.** The better the models, the more efficiently they all make the same mistake.

The authors call this a **capability paradox**: improving individual models does not necessarily produce better system-level outcomes. Whether the same dynamics arise outside financial markets is an open empirical question.

**Bottom line:** when you upgrade every agent in your system to the newest, best model, you may be upgrading your *correlation* — a team of frontier models from the same generation is one mind in many bodies, and risk that doesn't diversify doesn't go away because the components got smarter.
