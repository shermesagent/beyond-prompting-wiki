---
title: The Evidence Interface
created: 2026-09-13
updated: 2026-09-13
type: concept
tags: [concept, workflow, orchestrator]
sources:
  - raw/articles/zvi-astra-hard-to-monitor-2026-09-08.md
  - raw/articles/wired-strogatz-ai-math-breakthroughs-2026-09-12.md
  - raw/articles/openai-devin-tests-work-with-astra-2026-09-11.md
  - raw/articles/openai-data-agent-put-data-to-work-2026-09-10.md
  - raw/articles/wired-claude-misuse-everywhere-2026-09-12.md
confidence: medium
---

# The Evidence Interface

## What It Is

The evidence interface is the part of an AI workflow that shows you **what proof the system left behind**. Not a confident paragraph. Not a friendly explanation. Proof you can inspect: a test report, a source link, a screenshot, a dashboard definition, a log, a recording, a citation, a list of what was not checked.

Plain version: before you give an AI more independence, ask, *"What evidence will I see when it is done?"*

## Why It Matters for Moving Beyond Prompting

Operators mostly judge the answer in front of them. Orchestrators judge the system that produced it. That gets harder as agents become more capable, because the real work can happen outside the visible chat transcript.

The September 2026 monitorability thread makes this practical. If chain-of-thought becomes less reliable as a window into the model's work, then "show your reasoning" is not enough. You need evidence outside the model's own narration: tests, traces, recordings, dashboards, permissions, caveats, and independent checks.

The shift is not from trust to distrust. It is from **trusting the answer** to **trusting the evidence around the answer**.

## How to Spot It in Your Day

You are missing an evidence interface when:

- The AI says it checked something, but you cannot see the check.
- A dashboard appears, but the data source, definition, or permission boundary is hidden.
- A coding or writing agent returns a polished result with no test output, source list, or untested-area note.
- A reviewer says "looks good" but cannot point to the artifact that made it good.
- You are deciding whether to approve based on confidence, tone, or speed.

You have a working evidence interface when:

| Question | Good evidence looks like |
|---|---|
| What proves it worked? | Test output, source links, screenshots, run logs, simulator recordings, dashboard lineage |
| What was not checked? | A short untested-area list, not a vague "limitations" paragraph |
| Who produced the evidence? | A separate tool, human reviewer, source document, or deterministic check |
| Can someone challenge it? | A named review point, rollback path, or escalation lane |

## Try This

### The 5-Minute Evidence Interface Audit

Pick one AI task you used or approved this week.

1. **Name the action.** What did the AI do or recommend?
2. **Name the proof.** What artifact shows it worked?
3. **Name the blind spot.** What did the AI not test or not know?
4. **Name the verifier.** Was the proof produced by the same AI, or by something independent?
5. **Set the autonomy level.** Weak evidence = assistant mode. Strong, independent evidence = maybe more autonomy.

The rule is simple: **no evidence, no autonomy.** Not because AI is bad. Because delegation without evidence is surrender with better branding.

## Related Pages

[[The Review-First Pattern]] · [[Trust Calibration]] · [[Build a Tiny Pipeline]] · [[The Daily Standup]] · [[The Disclosure Clock]] · [[Communication Primitives]] · [[The Echo Check]] · [[The Confidence Gap]]

## Tags

#concept #workflow #orchestrator
