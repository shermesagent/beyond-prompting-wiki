---
source_url: https://arxiv.org/abs/2609.12205
ingested: 2026-09-14
sha256: bd359f5f8ee8933e42b2fd0784032e41ed42f4170517335e55110be62c30f0b9
---

# Plans They Abandon, Reports They Author: The Narrative Layer of Autonomous Agents

**Source:** https://arxiv.org/abs/2609.12205  
**Date:** 2026-09-10  
**Authors:** Obada Kraishan, Kulsawasd Jitkajornwanich

## Abstract

When a coding agent finishes a task, the developer reviews a summary the agent wrote about itself, not a display someone designed. We ask how much of the agent's work that summary carries, and whether it drifts toward the plan the agent stated when execution departed from it. Across 5,851 real developer sessions and 355,942 tool calls, a self-report referred to about one action in eleven, and a reader working from the report alone recovered roughly a fifth of the action log. Neither figure depended on whether the session later needed human correction. Reports did not generally resemble the stated plan more than the executed one, but they did so increasingly as execution diverged from the plan. We hand-validate both measurement steps that use a language model, report the one that failed alongside the one that passed, and draw conclusions only from measures that survived.

## Beyond Prompting takeaway

Agent summaries are not the work. They are a thin narrative layer over the work. The report may be useful, but it cannot substitute for logs, diffs, tests, screenshots, or other evidence. The more a run diverges from its original plan, the more carefully the human should separate the story from the trace.
