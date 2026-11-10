---
title: The Known-Case Check
created: 2026-11-10
updated: 2026-11-10
type: concept
tags: [concept, workflow, orchestrator]
sources: [raw/articles/known-good-known-bad-2611.11673.md, raw/articles/from-dialogue-to-task-2611.11435.md]
confidence: medium
---

# The Known-Case Check

## What It Is

Before trusting an AI workflow on unfamiliar work, give it a case whose correct answer you already know. Then change one important detail and see whether it notices **and** repairs the answer. This is a small trial, not a guarantee of future accuracy.

## Why It Matters for Moving Beyond Prompting

An operator may be satisfied when the AI sounds helpful. An orchestrator tests the whole handoff: did it notice a changed condition, did the final result follow from the correction, and did a person check the result? A chemistry teaching demonstration found an AI that noticed a unit problem on a second pass but still kept an incorrect downstream conclusion. That is one small demonstration, not evidence that all models fail at that rate. [Lavinda, preprint](https://arxiv.org/abs/2611.11673). ^[raw/articles/known-good-known-bad-2611.11673.md]

## How to Spot It in Your Day

- A polished answer is accepted because it mentions the right issue, even though the final number or recommendation was not repaired.
- A pilot uses only examples where the tool already looked good.
- The team counts chat sessions, not what happened after the chat. In a higher-education observational study, conversation depth and later task outcomes were different measures; this does not establish what will happen in your workplace or a K–12 classroom. [Zhuang and colleagues, preprint](https://arxiv.org/abs/2611.11435). ^[raw/articles/from-dialogue-to-task-2611.11435.md]

## Try This

**Five-minute public-information test:** Choose a public event notice whose date is verified on an official page. Ask an approved AI tool to summarize the notice. Then give it a copy with *one deliberately altered date*, clearly labeled as a test and never shared as a real notice. Record two separate scores: `flagged the changed date?` and `final summary used the verified date?`. Check both against the official notice yourself. Do not use student, personnel, patient, or other private records as test material.

## Related Pages

[[Trust Calibration]] · [[The Evidence Interface]] · [[The Task Scaffold]] · [[The Review-First Pattern]]

## Tags

#concept #workflow #orchestrator