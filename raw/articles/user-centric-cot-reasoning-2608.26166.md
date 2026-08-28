---
source_url: https://arxiv.org/abs/2608.26166
ingested: 2026-08-28
sha256: abfe579d12749ee86f19e7699eadec3184e84fb829246c941c1ec1a51fcffd3b
---
# Improving LLM Interpretability with User-Centric Chain-of-Thought Reasoning

**Source:** arXiv:2608.26166 (cs.HC / interpretability)

**Abstract:** Advancing reasoning capabilities allow large language models (LLMs) to tackle increasingly complex problems, while reasoning traces - intermediate steps toward solutions - open up high-stakes applications by enabling human inspection of AI decision-making. However, current approaches prioritize model performance over human interpretability, limiting effective human-AI collaboration. In this study, we design and evaluate a human-centered approach that structures reasoning traces based on self-contained, verifiable steps, enabling users to independently assess and correct AI reasoning. Our approach uses XML-like tags to encode reasoning content and metadata, facilitating targeted feedback. Evaluation on mathematical reasoning tasks shows our approach maintains equivalent performance to standard Chain-of-Thought reasoning while enhancing interpretability. User studies demonstrate significant improvements in perceived usefulness and ease of use. This work advances understanding of how user-centric design of LLM outputs can better serve human collaboration needs in high-stakes AI deployments.

**Key takeaways for the wiki:**
- Reasoning traces can be structured into self-contained, verifiable steps — without hurting performance — so a human can inspect and correct each step independently.
- "Show your work" is not just a request: it can be a designed property of the output (XML-like tagged steps), and users find it more useful and easier to use.
- The orchestrator version: ask agents to return their reasoning in discrete, checkable steps — each step verifiable on its own — instead of one polished final answer.
- Checkable steps turn trajectory review (The Daily Standup's Fifth Question) from a feeling into a concrete pass.
