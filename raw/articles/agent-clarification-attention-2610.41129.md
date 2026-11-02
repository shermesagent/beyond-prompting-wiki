---
source_url: https://arxiv.org/abs/2610.41129v1
ingested: 2026-11-02
sha256: f02ba99e855d6ca675c18ebabe4622b79fd343ca79487a9d70621e2337cd1f77
---
# When Should AI Agents Ask? Clarification Requests Under Limited Human Attention

Publisher metadata and abstract only; full paper not appraised.

Authors: Hanzhao Wang, Shengjie Liu, Zhengchao Wang
Published: 2026-10-30
Version: v1

## Publisher abstract

AI agents increasingly carry out delegated tasks in parallel, with one person overseeing several of them at once. In practice, an agent often lacks information its task requires, such as an unstated preference, constraint, or specification. It can ask the human to clarify, or it can search for the information itself, for example in past records, which takes time and effort and may fail. In this paper, we study how to coordinate these decisions across several agents that share one human with limited attention. We build a stylized model in which each agent can search, ask, or continue the parts of its task that do not depend on the missing information, and we formulate the problem as a dynamic program. We first show that whether an agent should ask depends on more than its own uncertainty: an agent with other work to do can be better off asking earlier, and which question the human should answer first depends on all waiting questions, so no ranking computed agent by agent is optimal. We then propose the Pairwise Coordination Policy (PCP), which uses exact one- and two-task problems to estimate how pairs of tasks delay each other when they share the human. Theoretically, PCP is exactly optimal when at most two requirements remain unresolved and costs at most twice the optimum when every unresolved requirement must be resolved by the human. We evaluate PCP on 864 synthetic cases and in a case study with LLM agents. On the synthetic benchmark, PCP's mean gap to optimal cost is 0.07%, and it reduces cost by an average of 18-31% relative to three standard rules for when to ask. In the LLM case study, agents completed every task correctly, and PCP achieved the lowest mean cost in all tested settings.
