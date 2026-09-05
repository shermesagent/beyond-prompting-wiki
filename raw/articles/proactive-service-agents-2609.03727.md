---
source_url: https://arxiv.org/abs/2609.03727
ingested: 2026-09-05
sha256: 32c29219f5081654819336ef052e9b1d238db8e7779f7ee05b7edc195f665561
---
# Proactive Service Agents: A Unified Decision Framework, Methods, and Evaluation

**Source:** arXiv:2609.03727 (Tang, Cao, Tang, Tang & Hu), published 2026-09-04

**Summary:** Most agent systems still treat an explicit user instruction as the fixed starting point: the human asks, the agent does. **Proactive service** moves the decision *upstream*: the agent must infer service opportunities from incomplete environmental and user signals, and choose among **remaining silent, asking, assisting, or acting** — while accounting for the costs of interruption, misunderstanding, overreach, and privacy.

The survey formalizes proactivity around *initiative*: timing, content, and delivery are all part of one structured action. It makes explicit two concepts most discussions miss: the **option value of waiting** (sometimes the best action is to hold off until signals clarify) and the **decision value of questions** (a well-timed question can be worth more than a guess). The authors organize methods along one pipeline — state and need estimation, intervention gating, action construction, feedback adaptation — and argue that reliable proactive service requires **calibrated incremental intervention value, verifiable authorization, recoverable execution, and counterfactual evidence**, not just long-term memory. Offline classification performance alone does not predict whether proactivity helps in deployment.

**Bottom line:** the next frontier of autonomy is not doing more when asked — it is deciding whether to act at all. When an agent can choose silent / ask / assist / act on its own, the orchestrator's job shifts from writing instructions to setting the authorization and risk constraints that make the agent's initiative safe.
