---
title: The Daily Standup
created: 2026-06-27
updated: 2026-07-02
type: practice
tags: [practice, orchestrator, workflow, mindset]
confidence: high
sources:
  - raw/articles/constrained-override-policy-2607.00420.md
  - raw/articles/constructive-alignment-2607.00001.md
---

# The Daily Standup

## What You'll Do

Build a 5-minute daily habit of reviewing your AI workflows — what ran, what worked, what didn't — exactly like a software team's standup meeting, but for your delegation pipelines. You're not adding more work. You're adding a feedback loop that makes all the other work better.

This takes 5 minutes a day and requires nothing but your templates and a place to jot notes.

## Why This Matters

Software teams hold daily standups for one reason: **feedback loops shorten improvement cycles.** Without the standup, a broken pipeline might run for two weeks before anyone notices. With it, you catch the drift on day two and fix it in 30 seconds.

The orchestrator's version of this is simpler but no less powerful. Every day, you ask three questions about your AI workflows:

1. **What ran yesterday?** — What pipelines, templates, or delegations did you actually use?
2. **What worked?** — Where did the AI deliver exactly what you expected?
3. **What didn't?** — Where did output drift, boundaries get fuzzy, or handoffs break?

That's it. Three questions. Five minutes. The payoff isn't in any single standup — it's in the thread. After two weeks, you'll have identified exactly which templates need tightening, which pipelines are reliable enough to automate further, and which tasks you should stop delegating because the AI isn't ready for them yet.

This is also the difference between someone who *tries* delegation and someone who *practices* it. Trying is one-and-done. Practicing is iterative. The standup is the iteration engine.

## The Daily Standup Template

```
DAILY STANDUP — [Date]

PIPELINES RAN:
  - [Pipeline name] — ran [N] times
  - [Pipeline name] — ran [N] times

WHAT WORKED:
  - [Pipeline]: [what went well]
  - [Template]: [output matched criteria]

WHAT DIDN'T:
  - [Pipeline]: [what drifted or broke]
  - [Template]: [where output fell short]

ONE FIX:
  - [The single adjustment you'll make today based on what you saw]

YESTERDAY'S FIX RESULT:
  - [If you made a fix yesterday, did it work?]
```

## Step by Step

### Step 1 — Review What Ran (1 min)

Open your notes, templates, or AI history. List every pipeline or template you actually used yesterday. Not what you *planned* to use — what you *used*. Be honest. If you prompted manually instead of using your template, note that too. That's data.

### Step 2 — Quick Quality Check (2 min)

For each pipeline, scan the output against your original success criteria. Don't deep-read everything — you're looking for patterns:

- **Drift:** Output is slowly getting worse over repeated runs (usually because the AI model changed or your inputs shifted)
- **Breakage:** A handoff or formatting step that failed completely
- **Surprise:** Output that was acceptable but *different* from what you expected — often the first sign of future drift
- **Reliability:** A pipeline that's performed perfectly for 5+ consecutive runs — candidate for reducing your review cadence

### Step 3 — Pick One Fix (1 min)

Don't try to fix everything. Pick the single most impactful adjustment — the one that would improve the most runs or prevent the biggest risk. Then make that adjustment to your template.

Examples:
- Tighten a success criterion that was too vague
- Add a stop condition where the agent went off-script
- Clarify the handoff format between two pipeline steps
- Reduce review frequency for a pipeline that's been rock-solid

### Step 4 — Check Yesterday's Fix (1 min)

If you made a fix yesterday, did it work? If yes, note it — that's reinforcement. If no, try a different fix today. If you're not sure, give it one more day of observation.

## Complete Example: Tuesday Morning Standup

```
DAILY STANDUP — Tuesday, June 23

PIPELINES RAN:
  - Morning Briefing — ran 1 time
  - Meeting-to-Tasks — ran 1 time
  - Email Draft (standalone template) — ran 3 times

WHAT WORKED:
  - Morning Briefing: 5th consecutive reliable run. Sources all valid. Tone perfect.
  - Email Draft: All three outputs passed criteria with minor edits.

WHAT DIDN'T:
  - Meeting-to-Tasks: Action item #4 was assigned to the wrong person.
    The transcript used "Sarah will follow up" but the AI assigned it to me.

ONE FIX:
  - Add to Meeting-to-Tasks Step 2 template: "For each action item,
    identify the person explicitly named in the transcript as the owner.
    If no person is named, flag as 'Owner Unclear' — do not guess."

YESTERDAY'S FIX RESULT:
  - Added source URL requirement to Morning Briefing — worked. All 5 bullets
    now consistently include working links.
```

## The One Constraint Rule

A large field experiment (N=553 workers) tested three ways to manage human oversight of autonomous AI: no overrides, unlimited overrides, and **exactly two overrides per decision episode**. The result: unlimited overrides made things worse — workers overcorrected, introduced bias, and reduced overall performance. Constrained overrides (two per episode) produced the best outcomes, because the limit forced workers to be *selective* about when their human judgment actually added value.

This applies directly to your standup practice:

**Give every pipeline a two-override budget.** For each pipeline you run, you're allowed to intervene exactly twice per day — change a parameter, reject an output, adjust a step. After two interventions, the pipeline runs as designed and you accept the result.

Why two? The study found it was the sweet spot between "no oversight" (which misses legitimate human knowledge) and "unlimited oversight" (which introduces noise and bias). Two is enough to catch the most important things. Not enough to second-guess everything.

**Track it in your standup.** Add to the PIPELINES RAN section:

```
OVERRIDES USED:
  - [Pipeline name]: 2/2 used — adjusted [what] and [what]
  - [Pipeline name]: 1/2 used — only needed to fix [what]
  - [Pipeline name]: 0/2 used — ran clean
```

After a week, the override count tells you something important. Pipelines that consistently use 0 overrides are candidates for reducing your review cadence — they've proven themselves. Pipelines that consistently use 2 overrides need template tightening — your judgment is being burned on predictable corrections. Pipelines that *exceed* their budget (you can't stop yourself from intervening more) are the ones where you need to either redesign the task or admit it's not ready for delegation yet.

The constraint isn't a punishment. It's a sharpener. When you know you only get two interventions, you save them for the moments that actually matter.

---

## The Fourth Question — Metacognitive Check-In

Every AI interaction subtly shapes what you value, what you attend to, and what you consider "your job." This isn't a problem — it's a fact of working with any tool over time. The practice is *noticing* it.

Add a fourth question to your daily standup, after What Ran, What Worked, and What Didn't:

**4. How did delegating today change how I feel about the work?**

Not "did the output meet criteria" — you already answered that in What Worked. This is different. Ask yourself:

- Did delegation make me feel more capable, or less?
- More connected to the outcome, or more distant?
- Did I feel relief (good — the pipeline handled something draining) or unease (worth investigating)?

The answers aren't right or wrong. They're data. After two weeks, look back at your standup notes and notice the pattern. Are there types of delegation that reliably make you feel more engaged? Types that reliably make you feel disconnected? That pattern tells you where your lines should be — and where they might be ready to move.

This is the metacognitive layer of the orchestration practice. The operator asks "did the AI do what I wanted?" The orchestrator asks "and how did that change me?"

---

## What to Do With the Patterns

After a week of standups, you'll start seeing signal:

**Pipeline is reliable (5+ consecutive good runs):** Reduce your review cadence. Move from checking every output to spot-checking every 3rd run. You can also consider adding it to a larger pipeline — it's proven itself.

**Pipeline is unreliable (fails criteria 2+ times in a week):** Tighten the template. Usually the problem is vagueness in the Goal or Success Criteria. Be more specific about what "done" looks like. If it still fails, the task may not be ready for delegation yet — and that's OK. Some tasks genuinely require human judgment.

**You're not using your templates:** This is the most important signal. If you built a template but keep prompting manually, ask why. Is the template too rigid? Does it take longer to set up than just prompting? Is the task actually less routine than you thought? The answer tells you whether to fix the template, simplify it, or retire it.

**Everything is working perfectly:** Great. Now look for the next task that *isn't* templated yet. The standup freed your attention — use it to expand.

## Common Pitfalls

**"I skipped a day and now I feel behind."**
The standup isn't a streak to maintain. It's a tool. Skip a day, pick it up tomorrow. The value is in the pattern, not the perfect attendance record.

**"Nothing went wrong, so the standup felt pointless."**
If nothing went wrong, your standup is 90 seconds: "Everything worked. No changes." That's not pointless — it's confirmation that your pipelines are healthy. Write it down and move on.

**"I don't have enough pipelines to review."**
Start with whatever you have. Even one template is worth reviewing. The standup grows with you — today it's one pipeline, next month it's five.

**"Fixing things every day feels like I'm bad at this."**
The opposite. Finding and fixing issues quickly is the mark of an orchestrator. Operators don't notice the drift. Orchestrators catch it on day two. The standup is how you catch it.

---

## Related Pages

[[05-Practice/README|05 — Practice]] · [[Build a Tiny Pipeline]] · [[First Delegation]] · [[Audit Your Prompts]] · [[The Line You Draw]] · [[Delegation Thinking]] · [[Trust Calibration]]

## Tags

#practice #orchestrator #workflow #mindset
