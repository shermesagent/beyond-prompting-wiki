---
title: Intent Scaffolding
created: 2026-08-06
type: concept
tags: [concept, delegation, orchestration, transparency, shared-understanding]
sources: [raw/articles/intentlint-intent-scaffolding-2608.04331.md]
confidence: medium
---

# Intent Scaffolding

## What It Is

**Intent scaffolding is making your intent explicit and *checkable* — not a vibe in your head, but structured, editable rules that both you and the AI check prompts against before they run.**

The idea comes from **IntentLint** (Feng, Zhao & Crisan, 2026), a research system for human-AI collaborative data analysis. When analysts share a notebook with an AI assistant, the analysis evolves fast — and the things that should capture shared understanding get messy: assumptions go undocumented, two people's intents silently disagree, prompts show up with no context, and the AI does things nobody asked for.

IntentLint's fix has two parts:

1. **Intent scaffolding** — infer what the collaborators actually intend from the work itself (the notebook, the history), and turn it into *structured, editable rules* anyone can read and change.
2. **Prompt-time linting** — every time someone writes a prompt, check it against the shared rules *before* it runs. The AI flags conflicts while they're cheap to fix.

In a study with 16 data analysts, the system improved people's awareness of what their collaborators intended, and nudged them to reflect on their own analytic strategies.

## Why It Matters for Moving Beyond Prompting

The moment you move from asking questions to delegating real work, **intent becomes the thing you can't delegate**. The orchestrator writes the spec; the scaffold is the spec made checkable.

Three reasons this concept matters:

- **Shared work breaks without shared rules.** A solo prompt is a private conversation. A pipeline, a team workflow, a delegated system — those are public. The failures IntentLint documents (undocumented assumptions, cross-user misaligned intent, context-poor prompts, unwanted agent behaviors) are exactly the failures that show up when a team starts delegating for real.
- **The check belongs *before* the work, not after.** Prompt-time linting catches a conflict before the agent burns an hour executing the wrong thing. That's the same logic as a good review checkpoint — but automated, and cheaper than any review.
- **Rules you can edit beat rules you can remember.** "I told the AI once" is not a system. "Here are the four rules of this job, and the AI checks my prompts against them" is a system. The second one survives vacations, handoffs, and your own memory.

## How to Spot It in Your Day

- Your prompts carry assumptions nobody else could see — and you can't point to where they're written down.
- The agent does something unwanted that your prompt never mentioned (but a rule would have covered).
- Two people prompt the same AI system with intents that contradict each other, and nobody notices until the output collides.
- You keep re-explaining the same context in every prompt because the rules of the job live only in your head.
- A delegated task "went fine" but you can't say *why* — there's no record of the intent behind it.

**The tell:** you can describe what you want, but you can't show anyone a *checkable statement* of it — a rule that either holds or doesn't.

## Try This

1. Pick one task you delegate at least once a week (a report draft, an email batch, a schedule).
2. Write **three checkable rules** for it. Examples: a *constraint* ("never include prices in the draft"), an *output rule* ("every section ends with a question"), and a *truth rule* ("if you don't know something, say 'unknown' instead of guessing").
3. Put the rules at the top of the prompt — or, better, in a shared file the agent reads every time.
4. When the agent breaks a rule, **edit the rule, not the prompt**. The prompt is the conversation; the rule is the contract.
5. Next week, add one rule and delete one that proved useless. Scaffolding is a habit, not a document.

## Related Pages

[[From Prompt to Pipeline]] · [[Task Decomposition]] · [[Trust Calibration]] · [[The Just Ask ChatGPT Trap]] · [[Accountability Asymmetry]] · [[Memory as Infrastructure]] · [[The Review-First Pattern]]

## Tags

#concept #delegation #orchestration #transparency
