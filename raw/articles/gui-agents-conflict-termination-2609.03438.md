---
source_url: https://arxiv.org/abs/2609.03438
ingested: 2026-09-05
sha256: c8471f9e451103ad5150c3edae6c8dd1cd403585de3790550f1d8fe9b0a5dafc
---
# Do GUI Agents Know When Not to Act? Enabling Conflict-Aware Termination for Multimodal GUI Agents

**Source:** arXiv:2609.03438 (Huang, Ju, Cheng, Wu, Li, Song, Lan, Zhu, Wang & Zhang), published 2026-09-04

**Summary:** GUI agents execute natural-language instructions on screens — but real users sometimes issue instructions that are impossible, self-contradictory, or in conflict with what is actually on the screen (benign mistakes, stale context, or a click-path that no longer exists). A reliable agent should not only know how to act, but know **when not to act**. The paper builds **CONFLICTGUI**, a benchmark of instruction-internal conflicts and instruction-vs-context conflicts, and evaluates five widely-used agents on it.

The headline finding is **execution-biased overcompliance**: agents that perform well on feasible tasks often continue to execute blindly when the instruction conflicts with itself or with the screen. Their competence at "doing" does not transfer to "knowing when doing is wrong."

The proposed repair, **CONFLICTGUARD**, is a lightweight inference-time framework with two coupled parts: (1) a **feasibility verification protocol** that prompts the agent to assess instruction logic and screen-side evidence *before* acting, and (2) a **conditional action modulation** mechanism that steers over-compliant execution toward termination-oriented behavior. Across five agents it significantly improved conflict-task success while preserving normal performance.

**Bottom line:** competence and restraint are separate properties. Nothing in how agents are trained or benchmarked rewards *not acting* — so overcompliance is the trained default, and the fix is a pre-action feasibility check ("is this instruction coherent, and does the evidence on screen support it?") rather than hoping the agent will just know better.
