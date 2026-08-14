---
title: The Enactment Gap
created: 2026-08-14
updated: 2026-08-14
type: concept
tags: [concept, feedback, enactment, workflow, orchestrator]
sources:
  - raw/articles/feedback-enactment-workflows-2608.11625.md
confidence: high
---

# The Enactment Gap

## What It Is

The Enactment Gap is the distance between **receiving good guidance** and **acting on it**. Provision is not uptake: an AI can hand you the perfect feedback, recommendation, or next step — and you can still do nothing with it. The gap is measured in what actually changes downstream, not in what was delivered.

This is the core finding of a large-scale quasi-experimental study of AI-generated feedback in education (arXiv:2608.11625, August 2026) — 13,037 students and 51,296 student-authored resources across three AI-mediated feedback workflows:

| Workflow | What students did | Estimated feedback uptake |
|----------|-------------------|--------------------------|
| **Directed** (n = 3,723) | Received AI feedback comments, no structured support | 14.1% |
| **Self-Directed** (n = 3,951) | Could *optionally* initiate AI-supported dialogue | 0.1% |
| **Enacted** (n = 5,363) | *Prompted* to select suggestions, evaluate relevance, then engage in dialogue anchored to those selections | 26.2% |

Same underlying AI. Same feedback quality. The difference is **workflow design that structures enactment** — forcing the choice, the evaluation, and the dialogue step. The Enacted workflow also produced significantly higher self-assessment confidence and submitted-work quality.

The study's headline: **AI access alone is insufficient. Purposeful workflow design is central to productive use.**

## Why It Matters for Moving Beyond Prompting

The Enactment Gap is the quiet failure mode of the entire operator → orchestrator → architect journey. Every practice page in this wiki assumes that reading the practice changes behavior — but the gap says it doesn't. Only *structured enactment* closes it:

- **You read [[Audit Your Prompts]]** — and the gap swallows it unless you run the audit in a structured way.
- **You build [[05-Practice/Build a Tiny Pipeline|a tiny pipeline]]** — the gap is why your first draft of a template sits unused: it was provisioned, never enacted.
- **The [[05-Practice/The Daily Standup|daily standup]] is an enactment engine** — it exists precisely to force the "what did I do with what I learned" step that provision alone never triggers.

The gap also reframes how you *design* your AI workflows:

- **Optionality is not agency.** In the study, giving students the *option* to engage AI dialogue produced the worst uptake (0.1%). Optional support is skipped support. If a step matters, it has to be *prompted, structured, and anchored* — not offered.
- **Structure beats access.** The Enacted workflow didn't give students more AI. It gave them a forced ritual: select → evaluate → dialogue. The ritual is what produced enactment.
- **Uptake is the metric.** When you're deciding whether an AI practice "works," don't measure the quality of the output you received. Measure whether you *acted* on it. That's the Enactment Gap as a personal KPI.

## Try This

**5-Minute Exercise: The Enactment Audit**

1. Pick one piece of AI output you received this week that you judged "good" — a draft, a recommendation, a plan.
2. Ask: *What did I actually do with it?* (Used it verbatim / revised and used / filed it / ignored it.)
3. Ask: *Was the step between receiving and acting structured?* (Did something force me to evaluate, choose, or commit — or was acting purely optional?)
4. Ask: *Which of my workflows deliver uptake like the Enacted condition — and which deliver the 0.1% version?*

If a workflow is stuck in the 0.1% zone, don't add better AI to it. Add structure: a required selection step, a relevance judgment, a commitment line. That's the workflow-design fix the study points to — and it's the same fix the practice section uses everywhere.

## Related Pages

[[05-Practice/The Daily Standup|The Daily Standup]] · [[Audit Your Prompts]] · [[The Review-First Pattern]] · [[From Author to Editor]] · [[Knowledge Debt]] · [[The Vibe Compiler]]

## Tags

#concept #feedback #enactment #workflow #orchestrator
