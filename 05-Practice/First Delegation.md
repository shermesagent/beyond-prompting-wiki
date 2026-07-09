---
title: First Delegation
created: 2026-06-26
updated: 2026-07-02
type: practice
tags: [practice, operator, orchestrator]
confidence: high
sources:
  - raw/articles/you-shall-not-pass-2607.00533.md
---

# First Delegation

## What You'll Do

Take one recurring task from your audit — something you're currently doing by typing a prompt every time — and design a simple, repeatable agent workflow for it. Then test it once. That's it.

This takes about 10 minutes. You'll walk away with a delegation template you can use every time that task comes up again.

---

## Why This Matters

The operator types a prompt. The orchestrator hands off a task with clear instructions, checks the result, and moves on. The difference isn't complexity — it's clarity. This exercise builds the muscle of defining work *before* you hand it off, which is the single habit that separates Phase 2 from Phase 3.

You're not building a system yet (that's Week 3). You're learning to think like someone who builds systems.

---

## The Delegation Template

For any task you want to delegate, answer these five questions. Write your answers down — don't just think about them.

```
FIRST DELEGATION — Template

GOAL:
  What outcome do I want? (One sentence. Not "help with…" — the finished thing.)

TOOLS:
  What does the agent need access to? (Search? A file? A style guide? Nothing?)

STEPS:
  What are the 2–5 specific things the agent should do, in order?
  1.
  2.
  3.

SUCCESS CRITERIA:
  How will I know this worked? (Be specific. "The output includes X, excludes Y, and fits format Z.")

REVIEW CADENCE:
  When do I check it? (Every time? Spot-check every 3rd run? Weekly review?)
```

---

## Before You Delegate: Draw Your Line

Before you pick your task, take 2 minutes to answer a question most people skip: **what would you *not* delegate, even if the AI could do it perfectly?**

Research on 448 professionals found that people draw boundaries around three kinds of work:
- **Identity work** — tasks that feel like "who I am" professionally
- **Human-facing work** — tasks where someone else will judge *you* for the output
- **Design/taste work** — tasks that require judgment, not just correctness

You don't need to resolve these today. You just need to know where they are. If your audit showed 7 "Could Delegate" candidates but 3 of them cross your identity line, start with one of the other 4. Build confidence on the safe side of the line first. You can always move the line later — but you can't un-burn the trust from a bad first delegation.

**Quick check:** Look at your delegation candidate. Does it cross any of these lines?
- [ ] This task feels like "who I am" — my professional identity
- [ ] Someone else will see this output and judge me for it
- [ ] This task requires taste and judgment, not just accuracy

If you checked any box, that candidate isn't wrong — but it's not your *first* delegation. Pick one you didn't check. Start safe. Grow outward.

For a deeper exercise (5 minutes, reusable), do the full [[The Line You Draw]] boundary audit. It pairs with your prompt audit: one tells you what you *could* delegate, the other tells you where to start.

---

## Step by Step

### Step 1 — Pick Your Task (1 min)
Look at your audit worksheet from Week 1. Pick one task marked Y (could delegate) that:

- Shows up at least once a week
- Has a clear, predictable output (a document, a list, a summary, a draft)
- Doesn't require real-time judgment or deep creative exploration every time

Good candidates: daily news briefing, meeting note summary, weekly status update, email draft, data table generation, research roundup.

### Step 2 — Fill the Template (5 min)
Work through each section. Be specific. Vague goals produce vague output.

- **Goal:** "A daily briefing" is vague. "A 5-bullet summary of the day's top AI news, each bullet under 40 words, with source links" is specific.
- **Tools:** If the agent needs to search the web, say so. If it needs access to your notes, say so. If it can work from scratch, say so.
- **Steps:** Think of these as instructions you'd text a new team member. "1. Search for today's top AI stories. 2. Pick the 5 most significant. 3. Write a one-sentence summary of each. 4. Include the source URL for each. 5. Format as bullet points."
- **Success Criteria:** This is the checkpoint. If you can't describe what "good" looks like before you see the output, you're still in operator mode.
- **Review Cadence:** Delegation doesn't mean abdication. Decide up front how often you'll spot-check.

### Step 3 — Test It (3 min)
Open your AI tool. Paste your STEPS as the prompt. Don't over-explain. Don't add context. Just hand it off and let it run.

When the output comes back, check it against your success criteria. Does it pass? If not, adjust one thing in your STEPS — not the prompt you write, but the *template* — and try again next time.

### Step 4 — Save the Template (1 min)
Copy your filled template somewhere you'll find it next week. A note, a document, a pinned message. The point is that next time this task comes up, you don't rewrite the prompt — you reuse the template.

---

## Complete Example: Daily News Briefing

Here's what a filled delegation template looks like for a common recurring task.

```
FIRST DELEGATION — Daily News Briefing

GOAL:
  A 5-bullet summary of the most important AI news from the last 24 hours.
  Each bullet under 40 words. Each includes a source link.

TOOLS:
  Web search (for current news)

STEPS:
  1. Search for the top AI and tech news stories from the past 24 hours.
  2. Filter to stories with real significance — new research, product launches,
     policy changes, major industry moves. Skip rumors and hype.
  3. Select the 5 most important stories.
  4. For each story, write one bullet: the key fact in under 40 words,
     followed by the source URL.
  5. Format as a clean bullet list. Add a one-line header with today's date.

SUCCESS CRITERIA:
  - Exactly 5 bullets
  - Each bullet is a single, factual statement under 40 words
  - Every bullet has a working source link
  - No opinion, no commentary, no "in a significant development…"
  - I can read the whole thing in under 30 seconds

REVIEW CADENCE:
  Spot-check every 3rd briefing. Full review if a bullet feels off.
```

### Why This Works

- **The goal is specific.** Not "tell me the news" — a defined format with a defined constraint.
- **The steps are executable.** Anyone (or any agent) could follow them in order.
- **The success criteria are testable.** You can run down the checklist in 15 seconds.
- **The review cadence is realistic.** You don't need to check every output. You check often enough to catch drift.

---

## Common Pitfalls

**"My first template was too vague."**
Normal. Vague goals produce vague output. Tighten one section — usually the Goal or Success Criteria — and test again.

**"The agent didn't follow my steps."**
Also normal. Agents are literal. If it skipped a step, your instruction probably wasn't explicit enough. Add the missing detail to your template, not to a one-off follow-up prompt.

**"This feels like more work than just typing a prompt."**
It is — the first time. But a template that takes 10 minutes to create saves you 3 minutes every time you reuse it. After four uses, you're ahead. After twenty, you've reclaimed an hour of your life.

**"I don't have a recurring task."**
Look again at your audit. Content generation and research tasks almost always repeat in different clothes. If you truly have nothing recurring, pick the single task that annoys you most and template it anyway. The practice is the point.

**"I let the agent do the thinking and just wait for the output."**
This is the Cognitive Outsourcing Trap — and it's backed by new research (arXiv:2607.07522). In a controlled study of human-AI co-creativity, people who self-reported higher cognitive outsourcing ("I let the other person do the thinking") produced LESS original ideas, even when working with another human. Delegation is task handoff, not thinking handoff.

The fix is simple: before you run your delegation template, write down one sentence about what *you* think the right answer might be. Your guess. It doesn't have to be correct — it just has to be yours. Then compare it to the agent's output. This 10-second check keeps your judgment in the loop and prevents the slide from "I'm delegating tasks" to "I'm outsourcing my thinking."

If you consistently find that the agent's output is better than your guess, that's not a problem — that's the point of delegation. If you find you've stopped making guesses at all, that's the trap. Start again.

---

## What Comes Next

Use this template at least twice before moving to Week 3. Each time you use it, note what worked and what didn't — then adjust the template. After two rounds, you're ready for [[Build a Tiny Pipeline]], where you'll chain two templated tasks together.

---

## Related Pages

[[05-Practice/README|05 — Practice]] · [[Audit Your Prompts]] · [[Build a Tiny Pipeline]] · [[The Line You Draw]] · [[Delegation Thinking]] · [[Task Decomposition]]

## Tags

#practice #orchestrator
