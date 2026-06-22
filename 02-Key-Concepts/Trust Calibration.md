---
title: Trust Calibration
created: 2026-06-21
updated: 2026-06-22
type: concept
tags: [concept, barrier, orchestrator]
sources: [raw/articles/accurate-but-not-confident-acm-2026.md]
confidence: high
---

# Trust Calibration

## What It Is

Trust calibration is the ongoing practice of knowing — specifically, not vaguely — when to trust an AI agent's output and when to verify. It's not a yes/no switch. It's a sliding scale you adjust based on the task, the stakes, your past experience with similar work, and the agent's track record.

Think of it like driving: you don't trust every car on the road equally. You watch some drivers more carefully than others. You check your mirrors more often at night than during the day. Trust calibration is bringing that same situational awareness to your relationship with AI agents.

## Why It Matters for Moving Beyond Prompting

Operators have a crude relationship with AI trust: either they trust everything ("it's so smart!") or nothing ("it hallucinates, I can't rely on it"). Neither position works at orchestrator scale.

When you're delegating multiple tasks across multiple agents, you need **granular trust** — trust that lives at the level of specific task types, not at the level of "the AI" as a whole.

Good trust calibration unlocks:

- **Speed.** You can breeze through the tasks where the agent is reliable and slow down only for the ones where it's not.
- **Delegation confidence.** You stop second-guessing everything (which defeats the point of delegation) and stop blindly accepting everything (which leads to [[Cognitive Surrender]]).
- **Feedback loops.** By paying attention to when an agent surprises you (in either direction), you refine your mental model and get better at calibration over time.
- **Teaming.** You learn which agents are good at what — just like you know which colleague to ask for numbers and which to ask for words.

## How to Spot It in Your Day

Good calibration looks like:

- You have a mental (or actual) list of task types the AI handles well vs. poorly
- You spend proportionally more time reviewing high-stakes outputs
- When the AI produces something that "feels wrong," you can articulate why
- You vary your verification strategy — spot-checks for low-risk tasks, line-by-line for high-risk
- You keep a running mental tally: "this model is solid on summaries, shaky on calculations"

Poor calibration looks like:

- You trust everything the AI says because it "sounds confident"
- You distrust everything and spend as much time verifying as you would doing the work yourself
- A single hallucination makes you abandon the tool entirely (or, the flip side: repeated hallucinations don't change your behavior)
- You can't predict, before running a task, whether the AI will handle it well

## What the Research Says

An ACM study (April 2026) provides the first empirical evidence that **AI support impairs confidence calibration** — your ability to accurately judge your own performance. Here's the finding in plain language:

People using AI get better results but *worse at knowing when they're right or wrong*. Specifically:
- They become **overconfident** when the AI is wrong — trusting bad output because the AI sounds confident
- They become **underconfident** when they're actually right — doubting their own correct judgment when the AI disagrees

This means calibration doesn't just stay flat with AI use. It *degrades*. Unless you actively maintain it. The orchestrator's verification checkpoints aren't optional — they're the countermeasure.

See also: [[Cognitive Surrender]] · [[Friction by Design]]

## Try This

**5-Minute Exercise: Build a Trust Map**

1. Take out a piece of paper (or a note). Draw three columns: **High Trust**, **Medium Trust**, **Low Trust**.
2. Think about the last 5–10 things you used AI for. Place each task type in a column based on your actual experience — not what you think the AI _should_ be good at.
3. For the High Trust column: what do these tasks have in common? (Simple structure? Lots of training data? Clear right/wrong answers?)
4. For the Low Trust column: what's the pattern? (Nuance? Domain knowledge? Math? Current events?)
5. Now pick **one Low Trust task** and think: what would it take to move it to Medium? A different way of decomposing it? A verification step? A different agent?

Keep this map. Update it next week. You're building your own calibration data.

## Related Pages

[[Cognitive Surrender]] · [[Task Decomposition]] · [[Delegation Thinking]] · [[Memory as Infrastructure]] · [[04-Barriers-and-Bridges/README|04 — Barriers & Bridges]]

## Tags

#concept #barrier #orchestrator
