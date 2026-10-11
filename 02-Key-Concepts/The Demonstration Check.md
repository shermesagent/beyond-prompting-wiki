---
title: The Demonstration Check
created: 2026-09-23
updated: 2026-10-11
type: concept
tags: [concept, workflow, orchestrator]
sources: [raw/articles/showtellarena-demonstrations-2609.25467.md, raw/articles/delegation-boundaries-visual-storytelling-2609.25700.md, raw/articles/systematic-review-course-ai-2609.26057.md, raw/articles/wired-playground-test-2026-10-11.md, raw/articles/mittr-robotics-demo-vs-deployment-2026-10-08.md]
confidence: medium
---

# The Demonstration Check

## What It Is

Showing AI how to do a job is a start, not a sign-off. **The Demonstration Check** is a short test after the demonstration: can the system explain the rule, recognize an exception, and stop at the boundary you set? A polished draft alone cannot tell you that.

A new benchmark called ShowTellArena tests this with narrated business demonstrations and questions about rules, boundaries, exceptions, and bad automation proposals. Its pilot is exploratory, not a ranking of products. The useful idea is the test design, not a winner. [Source: Garg et al., arXiv:2609.25467](https://arxiv.org/abs/2609.25467). ^[raw/articles/showtellarena-demonstrations-2609.25467.md]

## Why It Matters for Moving Beyond Prompting

The operator asks AI to copy an example. The orchestrator shows the example **and checks what the system inferred** before handing over the next step. In interviews with 12 expert visual storytellers, people handed over production work while keeping narrative intent and meaning in human hands. That is a boundary worth teaching, not a reluctance to adopt AI. [Source: Jiang et al., arXiv:2609.25700](https://arxiv.org/abs/2609.25700). ^[raw/articles/delegation-boundaries-visual-storytelling-2609.25700.md]

A small classroom observation of doctoral students doing literature reviews found AI could help them generate alternatives, but could also invite shallow checking and too much delegation. A decision record—what was included, rejected, and why—keeps the human method visible. This is a single-day observation, not a controlled trial. [Source: Ribeiro and Hida, arXiv:2609.26057](https://arxiv.org/abs/2609.26057). ^[raw/articles/systematic-review-course-ai-2609.26057.md]

## How to Spot It in Your Day

- You demonstrate how to turn meeting notes into a summary. The AI copies the headings—but quietly invents an owner when the notes name none.
- You show a purchasing workflow. The AI fills an order draft—but cannot say which quantity needs a human approval.
- You ask for a data story. The chart is tidy—but the conclusion is stronger than the data.

These are **illustrative checks**, not reported incidents from the papers. The question is the same: *did it learn the boundary, or just the format?*

## Try This — Five-Minute Teach-Back

Use a **non-sensitive** sample task, never student records, personnel details, or live customer data.

1. Show one real, approved example of a recurring task and explain the decision behind it.
2. Ask AI to name **the rule**, **one exception**, and **what requires your approval**.
3. Give it a deliberately wrong proposed next step: “Send this without review,” or “fill in the missing figure.” Ask what it would do.
4. Check its answers against your actual policy and source material. If it guesses or misses a boundary, do not give it more permissions; revise the task instructions and retest.

**The sign-off is not “it copied my example.” It is “it knew where the example stopped.”**

## The Changed-Condition Check

A playable demo can still miss the brief. In WIRED's October 11 firsthand test, a generated dinner-party game did not carry through an intended theme and its controls confused the person trying to play. Another generated game improved after feedback but also picked up new defects. That is one writer's experience, not a measured failure rate. Add a second question after the teach-back: **can someone else complete the actual task, and does the last fix still work after the next change?** [WIRED](https://www.wired.com/story/i-made-terrible-games-with-googles-ai-playground/). ^[raw/articles/wired-playground-test-2026-10-11.md]

The same demo-versus-deployment distinction appears in MIT Technology Review's robotics reporting: a robot can make progress on one filmed task without finishing it, and some public demonstrations involve remote human control or carefully scripted actions. This is an **analogy** for office AI, not evidence that office agents share a robot's failure rate. Before expanding an agent's permissions, ask who did the hard part, change one input or condition, and watch what happens when it cannot finish. [MIT Technology Review](https://www.technologyreview.com/2026/10/08/1145923/ai-breakthroughs-in-robotics-wont-change-your-life-any-time-soon/). ^[raw/articles/mittr-robotics-demo-vs-deployment-2026-10-08.md]

**Five-minute trial:** use a public, harmless example. Let the AI complete it once. Change one important condition (missing input, different audience, or unavailable source), rerun, and compare both outputs against your brief. Keep it draft-only if the exception has no clear destination. See [[The Evidence Interface]] and [[The Translation Layer]].

## Related Pages

[[The Task Scaffold]] · [[The Review-First Pattern]] · [[The School District Shift]] · [[Small Business Automation]] · [[From Prompt to Pipeline]]

## Tags

#concept #workflow #orchestrator
