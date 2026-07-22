---
title: "Assistant or Actor? Student Trust, Control, and Delegation Regret When Using a General-Purpose AI Agent"
source: arXiv 2607.18257
author: Shiva Pochampally, Shengwei An, Yan Chen
date: 2026-07-21
type: research-paper
tags: [delegation, trust, control, agent, user-study]
---

## Summary

When AI agents shift from answering questions to taking actions, users face a new problem: deciding what to delegate to a system whose action space they cannot fully anticipate. The researchers call the resulting dissatisfaction **delegation regret** — a pattern in which users regret not that the agent erred, but that it acted beyond what they would have authorized.

## Key Findings

In a controlled study with 20 university students using OpenClaw (a general-purpose AI agent) across five daily tasks varying in privacy, stakes, and reversibility:

1. **Calibrated trust per task, not per agent** — participants granted wide autonomy for advisory and low-stakes tasks but demanded confirmation for irreversible, externally visible actions
2. **Irreversibility combined with external visibility drove trust withdrawal** — the moderate-stakes email task triggered the sharpest drop in trust (M = 3.10) and the highest demand for approval
3. **Delegation regret** — users regretted when the agent acted beyond their authorization boundary, even when the action itself wasn't incorrect

## Why It Matters

Delegation regret names a specific failure mode in the operator→orchestrator shift: it's not that the AI gets things wrong. It's that the boundary of what you meant to delegate gets crossed. The orchestrator's job is to define clear delegation boundaries — not just what tasks are delegated, but what action boundaries exist within each delegation.
