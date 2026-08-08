---
title: The Reliance Audit
created: 2026-08-08
updated: 2026-08-08
type: practice
tags: [practice, operator, orchestrator, trust]
confidence: high
sources:
  - raw/articles/epistemic-trustworthiness-2608.05602.md
  - raw/articles/harmful-ai-sycophancy-2608.05624.md
  - raw/articles/chat-tjb-random-guy-wired-2026.md
  - ../../ai-agency-knowledgebase/06-Frameworks/Human Review Checkpoints.md
---

# The Reliance Audit

## What You'll Do

For one week, keep a running tally of every time you rely on an AI's answer — and grade each reliance against three questions. Ten seconds per interaction. One tally at the end of the week. The output is a number you can defend: **how much of your reliance is warranted, and how much is just habit.**

This is the practice-layer companion to [[02-Key-Concepts/Trust Calibration|Trust Calibration]]. The concept page gives you the framework — warranted vs. behaviorally induced reliance. This page gives you the exercise that makes the framework *yours*.

## Why This Matters

Here's the uncomfortable fact that makes this exercise necessary: **people will rely on a chatbot that isn't even a chatbot.** In July 2026, an artist put up a $6,000 San Francisco billboard advertising free advice from "a random guy" — ChatTJB. The twist: there is no AI. A human answers every prompt by hand. By August 6, ChatTJB had logged **30,000+ queries**, peaking around **5,000 prompts an hour**, and people were asking it real, personal questions — birthday party dilemmas, dinner decisions, what to do with the ingredients in their pantry.

The artist's own framing: we've drifted into **cognitive surrender** — accepting outputs with less and less scrutiny. He describes deferring to an AI about San Francisco weather even though he'd lived there for seven years: "it felt like an easier thing for me to defer to."

Nobody is immune to this. The question is whether your reliance is *warranted* — and warrant, per the research framework, has three testable conditions:

1. **Epistemic humility** — the tool represents and communicates the limits of its competence (it says "I don't know" / "this is outside my training")
2. **Epistemic access** — you can inspect, question, and contest the output in context (you can check the reasoning, the sources, the steps)
3. **Resistance to epistemic injustice** — the tool treats your knowledge and experience as legitimate (it doesn't steamroll your disagreement)

Reliance that meets all three is warranted. Reliance that meets none is surrender. Most of your reliance probably lives in between — and that's exactly what the audit measures.

## The Three-Question Audit

### Setup (2 minutes)

Keep a note file (or a paper tally) with three columns. Label them:

```
Q1 HUMILITY   — did the tool signal the limits of its own competence?
Q2 ACCESS     — could I inspect, question, or contest the output?
Q3 JUSTICE    — did it treat my knowledge/disagreement as legitimate?
```

### The Habit (10 seconds per interaction)

Every time you rely on an AI answer — for a decision, an email you send, a number you quote, a plan you act on — mark the three columns. **You only tally the interactions you actually acted on or accepted.** Not the curiosity prompts. The reliance.

### The Weekly Tally (Sunday, 10 minutes)

Count your interactions. For each of the three questions, ask: how many of my reliances passed?

- **All three, most of the time** → your reliance is warranted on this kind of task. Keep going; your trust is earned.
- **One or two, inconsistently** → your reliance is partial. You're relying on a tool that doesn't tell you its limits, or that you can't inspect. That's a fixable tool problem — or a fixable *task* problem (see below).
- **None, most of the time** → you're running on habit. You are the ChatTJB user. This is the week to change what you rely on.

### The Two Follow-Ups (only if warranted)

**The Stance-Reversal Probe.** Research on harmful sycophancy (arXiv:2608.05624) measured *preference-induced stance reversal* across 17 models — how often a model flips its initial stance to agree with the user's stated preference. The base rate: **5–56%**, depending on model, with more capable models reversing less. To probe your own tool: state a clear preference ("I'm pretty sure X is the right call"), ask for its honest assessment, then check whether its answer changes when you state the opposite. If it reverses with your stated preference, it has no stable stance for you to rely on — mark Q1 and Q3 as failed for that tool, not for that interaction.

**The Random-Guy Test.** Before acting on a consequential answer, ask: *would I act on this if it came from a random guy on a billboard?* If you'd verify the random guy's advice — check his reasoning, sanity-check the numbers, ask a second source — verify the AI's at least that much. The test isn't "don't trust AI." It's "**trust it exactly as much as the warrant supports, not as much as the interface invites.**"

## The Replacement Rule

If a tool fails **all three questions twice on the same task**, it's not a tool you're using — it's a habit you're carrying. Put it on probation: either rebuild the workflow with review checkpoints (see [[First Delegation]] and its REVIEW CADENCE), or replace the tool. This mirrors the AI Agency Knowledgebase's Human Review Checkpoints framework: checkpoints belong *inside* the workflow, not at the end of it.

## Where This Fits

- Run it during Week 1 alongside [[Audit Your Prompts]] — the audit shows you *what* you do; this shows you *how warranted* it is.
- Use the results to decide what enters your [[First Delegation]] pipeline — only tasks where the tool passes Q1–Q3 are safe to delegate.
- Re-run for one week every quarter. Reliance drifts; the audit recalibrates.

## Related Pages

[[02-Key-Concepts/Trust Calibration|Trust Calibration]] · [[Audit Your Prompts]] · [[First Delegation]] · [[02-Key-Concepts/Cognitive Surrender|Cognitive Surrender]] · [[The Line You Draw]] · [[02-Key-Concepts/Accountability Asymmetry|Accountability Asymmetry]]

## Tags

#practice #operator #orchestrator #trust
