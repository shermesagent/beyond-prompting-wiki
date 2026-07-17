---
title: Build a Tiny Pipeline
created: 2026-06-27
updated: 2026-07-17
type: practice
tags: [practice, orchestrator, workflow]
confidence: high
sources:
  - raw/articles/agentic-workflow-patterns-ai-agency-kb.md
  - raw/papers/harness-handbook-2607.13285.md
---

# Build a Tiny Pipeline

## What You'll Do

Take two tasks you've already templated — and chain them together so the output of the first feeds directly into the second. You're not building a complex system. You're building a two-step pipeline. But once you've built one, you'll see pipelines everywhere.

This takes about 15 minutes. You'll walk away with a reusable workflow that does in 30 seconds what used to take you 10 minutes of prompting back and forth.

## Why This Matters

Delegating one task is the operator-to-orchestrator door. Chaining two tasks together is the moment you step through it. A pipeline means you're not just handing off work — you're *designing how work flows*. The output of step one becomes the input for step two automatically, without you in the middle. That's the orchestrator shift in one move.

Real orchestrators don't run single-agent tasks. They build chains: research → summarize → format. Draft → critique → revise. Find → filter → present. Each step is simple. The chain is the leverage.

This draws directly from real agentic workflow patterns used in production systems: prompt chaining, routing, and evaluator-optimizer loops. But we're starting with the simplest possible version — two steps, one handoff, no fancy tooling.

## The Pipeline Template

```
PIPELINE — Two-Step Workflow

PIPELINE NAME: (what does this whole thing do?)

STEP 1:
  Goal: (what does step 1 produce?)
  Template: (reuse your existing delegation template or write a new one)
  Output format: (what does step 1 hand to step 2?)

HANDOFF:
  How does step 1's output reach step 2? (copy-paste? same chat window? saved file?)

STEP 2:
  Goal: (what does step 2 do with step 1's output?)
  Template: (instructions that assume step 1's output is provided)
  Final output format: (what does the user receive?)

VERIFICATION:
  How do you check the whole pipeline produced good work?
```

## Step by Step

### Step 1 — Pick Your Two Tasks (2 min)

Look at your delegation templates from [[First Delegation]] and your audit from [[Audit Your Prompts]]. Find two tasks where:

- Task A produces something Task B could use as input
- Both tasks are routine and predictable
- The combined pipeline would save you real time

**Good pipeline candidates:**

| Task A (produces) | Task B (consumes) | The Pipeline |
|-------------------|-------------------|-------------|
| Research roundup of today's news | Format as a briefing email | Morning briefing pipeline |
| Summarize meeting transcript | Extract action items + owners | Meeting-to-tasks pipeline |
| Draft a report section | Review against style guide | Draft-and-polish pipeline |
| Find relevant sources on a topic | Write a literature summary | Research synthesis pipeline |
| Generate lesson plan ideas | Format into a shareable doc | Lesson plan pipeline |

### Step 2 — Design the Handoff (3 min)

The handoff is where most pipelines break. You need to be explicit about what moves from step 1 to step 2 and how. Three simple handoff patterns:

**Pattern A: Same-chat handoff.** Do both steps in the same chat window. Tell the agent "now, using the output above, do step 2." Works for simple pipelines. Downside: hard to reuse.

**Pattern B: Template handoff.** Copy step 1's output, paste it into step 2's template where it says `[STEP 1 OUTPUT HERE]`. Works for everything. Takes 10 seconds of your time.

**Pattern C: File handoff.** Step 1 saves to a file. Step 2 reads from that file. Requires an agent with file access. Most automated, but needs tool-capable AI.

Start with Pattern B — the template handoff. It's the least fancy but the most reliable. You can automate the handoff later once you know the pipeline is solid.

### Step 3 — Run the Pipeline (5 min)

1. Run Step 1 using your template. Get the output.
2. Copy the output.
3. Paste it into Step 2's template. Run Step 2.
4. Review the final output against your verification criteria.

That's it. You just ran a pipeline. It may not feel dramatic — but the structure is what matters. You've moved from "I prompt, then I prompt again" to "I designed a workflow that moves from A to B with a defined handoff."

### Step 4 — Save It (2 min)

Write your pipeline somewhere you'll find it next week. Include:
- Both templates (copy them in full)
- The handoff instructions
- What you'd adjust next time

Next time this pair of tasks comes up, you don't redesign — you rerun. Five uses from now, you'll have this pipeline memorized and it'll take 90 seconds to execute end to end.

## Complete Example: The Morning Briefing Pipeline

```
PIPELINE NAME: Morning Briefing Pipeline

STEP 1 — Research Roundup:
  Goal: 5-bullet summary of today's most important AI news
  Template:
    "Search for the top AI and tech news from the past 24 hours.
    Filter to significant stories (research, products, policy).
    Select the 5 most important.
    For each: one bullet under 40 words + source URL."
  Output format: Bullet list with source links

HANDOFF:
  Copy-paste the bullet list into Step 2's template below.

STEP 2 — Format as Team Email:
  Goal: Turn the bullet list into a ready-to-send team briefing email
  Template:
    "Using the news bullets below, write a brief team email:
    - Subject line: 'AI Briefing — [today's date]'
    - Opening: One friendly sentence
    - Body: The bullets, slightly expanded (50-60 words each) with context
    - Closing: 'Questions or want a deep dive on any of these? Just reply.'
    - Tone: Warm, collegial, informative. No hype.

    [STEP 1 OUTPUT HERE]"
  Final output: Ready-to-send email

VERIFICATION:
  - Are all 5 stories present?
  - Are source links still working?
  - Is the tone appropriate for my team?
  - Can I send this without editing? (If not, adjust templates.)
```

## Common Pitfalls

**"My handoff broke."**
Step 1's output didn't match what Step 2 expected. Common cause: Step 1 produces a paragraph but Step 2 expects a list. Fix: make the Output Format in Step 1 more specific. "A bullet list" not "a summary."

**"Step 2 ignored Step 1's output."**
The agent summarized from scratch instead of using what Step 1 gave it. Fix: add "Using ONLY the information provided below" to Step 2's template.

**"This takes longer than just prompting."**
First time? Yes. Third time? No. A pipeline that costs 15 minutes to design and saves you 8 minutes per run breaks even on run #2. By run #20, you've reclaimed over 2.5 hours.

**"My tasks don't chain naturally."**
Not all tasks do. That's fine. Start with the ones that do: research → format, draft → polish, find → summarize. These patterns are everywhere once you look for them. If you truly can't find a pair, chain one task with a formatting step — even that teaches the pipeline muscle.

**The Reverse-Centaur Check (July 2026).** Before you commit to any pipeline, ask one question: *who does this pipeline work for?* Cory Doctorow's "Reverse-Centaur" framing (from his 2026 book *The Reverse-Centaur's Guide to Life After AI*) gives us a clean test:

- **Centaur pipeline:** AI handles the repetitive work. You handle the judgment. The pipeline amplifies your agency — you make more decisions, you have more context, you're more effective.
- **Reverse-Centaur pipeline:** You handle the repetitive work (feeding inputs, fixing formats, copy-pasting between steps). AI makes the judgments. The pipeline reduces your agency — you become a human connector between AI steps.

A good pipeline makes you *more* of a decision-maker. If you find yourself spending more time managing the pipeline than directing it, you've built a Reverse-Centaur. Fix it by moving the repetitive work from your side to the AI's side, or by collapsing steps so fewer handoffs are needed. The goal isn't more pipelines — it's pipelines where the AI works for you, not the other way around.

### The Friction You Keep

New research on AI-assisted creative work (arXiv:2607.07521) validates the Reverse-Centaur check with a useful distinction: **not all friction is bad.** The researchers found that AI tools in structural design work best when they reduce *repetitive modelling friction* (the boring stuff — redrawing, reformatting, recalculating) while preserving *reflective design friction* (the productive struggle of iterating through constraints).

This is the design principle behind every good pipeline decision:

- **Repetitive friction** = copy-pasting between steps, formatting outputs, looking up the same thing twice. Eliminate it. That's what pipelines are for.
- **Reflective friction** = judging whether the output is good, deciding which direction to take next, questioning an assumption the AI made. Keep it. This is where your judgment lives.

When you're reviewing your pipeline, ask: "Which friction did I remove, and which did I keep?" If you removed reflective friction — the parts where you used to think, judge, or decide — you've built a Reverse-Centaur. The AI is doing the thinking and you're doing the typing.

The fix: add a thinking checkpoint. After each pipeline step, insert 30 seconds where you ask "is this going in the right direction?" The pipeline handles the repetitive work. You handle the reflective work. That's the centaur.

See [[Reverse-Centaur]] for the full concept behind the metaphor.

## The Harness Principle: Name Your Pipeline by What It Does

New research on agent engineering (arXiv:2607.13285) identifies a universal bottleneck: **behavior localization** — finding what code needs to change when you want the system to do something different. The fix is the "Harness Handbook" principle: organize by *behavior* (what the pipeline does), not by *location* (where you saved it).

This sounds abstract. Here's what it means for your pipelines:

**Bad naming (location-based):**
- "that template in my Notes app"
- "the one I use for Tuesday mornings"
- "draft_review_v3_final.md"

**Good naming (behavior-based):**
- "Morning Briefing Pipeline"
- "Meeting-to-Tasks Pipeline"
- "Draft-and-Polish Pipeline"

The difference isn't cosmetic. Six months from now, when you have 8 pipelines across 3 different apps, "that template in my Notes app" is gone. "Morning Briefing Pipeline" is findable. The name encodes the behavior, and the behavior is what you'll remember.

### The Behavior-Centric Pipeline Document

Take your saved pipeline from Step 4 and add a one-line behavior description at the top:

```
PIPELINE: Morning Briefing
BEHAVIOR: Turns today's top news into a ready-to-send team email in under 2 minutes.
WHEN TO USE: Every morning by 8:30am. Skip weekends.
LAST MODIFIED: [date]
RELIABILITY: [Solid / Needs Watching / Fragile]
```

This tiny header does three things:
1. **You can find it** — search for "morning briefing" and it appears
2. **You know when to use it** — no guessing whether it's still active
3. **You know if it's healthy** — a glance tells you whether to review it or just run it

The Harness Handbook uses an automated tool to link behaviors to code. You don't need that. You just need the *habit* of naming pipelines by what they do, not where they live. It's the simplest thing in this entire practice section, and it's the one most people skip.

### Pipeline Reliability Tags

Borrowing from the Harness Handbook's BGPD (Behavior-Guided Progressive Disclosure) approach, tag each pipeline with a reliability level:

| Tag | Meaning | Review Cadence |
|-----|---------|---------------|
| **Solid** | 5+ consecutive runs without issues | Spot-check every 3rd run |
| **Needs Watching** | Works most of the time, occasional drift | Review every run |
| **Fragile** | Failed 2+ times in the past week | Fix or retire |

This is the orchestrator's version of a pipeline dashboard. Three tags, applied honestly, tell you everything you need to know about where to spend your attention.

---

## What Comes Next

Use this pipeline three times. Note where the handoff needs tightening. Tag it with a reliability level. Then you're ready for [[The Daily Standup]], where you'll build the habit of reviewing and improving your pipelines as a regular practice — the orchestrator's version of a standup meeting.

---

## Related Pages

[[05-Practice/README|05 — Practice]] · [[First Delegation]] · [[Audit Your Prompts]] · [[The Daily Standup]] · [[Task Decomposition]] · [[Delegation Thinking]]

## Tags

#practice #orchestrator #workflow
