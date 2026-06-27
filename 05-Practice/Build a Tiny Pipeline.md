---
title: Build a Tiny Pipeline
created: 2026-06-27
updated: 2026-06-27
type: practice
tags: [practice, orchestrator, workflow]
confidence: high
sources:
  - raw/articles/agentic-workflow-patterns-ai-agency-kb.md
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

## What Comes Next

Use this pipeline three times. Note where the handoff needs tightening. Then you're ready for [[The Daily Standup]], where you'll build the habit of reviewing and improving your pipelines as a regular practice — the orchestrator's version of a standup meeting.

---

## Related Pages

[[05-Practice/README|05 — Practice]] · [[First Delegation]] · [[Audit Your Prompts]] · [[The Daily Standup]] · [[Task Decomposition]] · [[Delegation Thinking]]

## Tags

#practice #orchestrator #workflow
