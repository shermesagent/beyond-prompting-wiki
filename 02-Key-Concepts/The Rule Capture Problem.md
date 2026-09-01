---
title: The Rule Capture Problem
created: 2026-09-01
updated: 2026-09-01
type: concept
tags: [concept, mindset, workflow, orchestrator]
sources: [raw/articles/organizational-rules-fail-ai-oibar-2608.29055.md]
confidence: high
---

# The Rule Capture Problem

## What It Is

Every prompt, SOP, playbook, and process document you write is a **lossy copy of the job**. It captures the *know-what* — the steps, the inputs, the outputs. It almost never captures the *know-how*: the negative boundaries (what the rule doesn't cover), the runtime judgments (when experienced people quietly deviate), and the learning history (what broke last time and why).

The Rule Capture Problem is the name for what happens when that lossy copy meets an AI: **the AI receives the procedure, but the organization operates on the procedure plus everything that didn't fit in it.** The rule looks complete. It isn't. The gaps are exactly where judgment lives — and they're invisible until something falls through one.

A 2026 paper (arXiv:2608.29055) argues this is a *knowledge representation* problem, not a discipline problem. You can't fix it by writing a longer prompt. The fix is externalizing the boundaries — deliberately, and as an organizational habit.

## Why It Matters for Moving Beyond Prompting

This is the research version of something every operator discovers the hard way: **"write a better prompt" has a ceiling.** You hit it the day you realize the people who do the work well aren't following the written rule — they're applying unwritten judgment on top of it. When you hand that rule to an AI, you hand it the lossy copy and expect it to do the full job.

The shift from operator to orchestrator is partly a shift in what you write. Operators write instructions and hope. Orchestrators write **boundaries** — they name the conditions, the exceptions, the failure cases, and what to do when the situation is unresolved. That's the difference between a prompt and a delegation.

The O-I-B-A-R scaffold from the paper gives you the vocabulary:

| Part | What it captures | Plain-language example |
|------|-----------------|------------------------|
| **OPEN** | When the rule applies at all | "For routine parent emails — not for anything involving a complaint or legal risk" |
| **IS** | When the judgment holds | "A reply within one business day is standard" |
| **BUT** | A concrete failure — more than just "not this" | "Last month an 'apologize and reassure' reply backfired when the parent had already received a refund — the apology read as the system ignoring them" |
| **ACTION** | What to do in this state | "Acknowledge the refund first, then apologize" |
| **RESULT** | What you learned, or what's still unresolved | "New rule: check for prior contact before drafting. Still unresolved: what to do when the parent is angry *and* we don't have the record yet — escalate to a human" |

The **BUT** clause is the gold. A concrete failure contains more information than "not this." Compare a success and a failure case side by side until you find the one variable that changed — that variable is a decision dimension worth tracking forever.

And the **suspension** is the most important word in the whole framework: the state where a dimension matters but its value is unresolved. A good rule doesn't guess at that moment. It says what to *do*: measure, ask, retrieve, or **escalate to a human**. Suspensions are where human-AI handoffs are born.

## How to Spot It in Your Day

- You have a "trusted" prompt that works 80% of the time, and the failures are always the same kind — but you've never written down what makes them different.
- A colleague says "oh, for *that* kind of request, you don't use the standard process" — and that exception lives only in their head.
- You review an AI output and think "anyone who knew the context would never have done it this way" — the context was never in the rule.
- Your SOP document and the way the work actually gets done have drifted apart, and nobody can say when it happened.

## Try This

**The 5-Minute Boundary Audit**

1. Take one prompt or SOP you use weekly — ideally the one that works "most of the time."
2. Write down what's NOT in it: three things a competent human would know that the written rule doesn't say.
3. For each gap, ask the comparison question: think of a time it went right and a time it went wrong. What one variable changed between them?
4. Write one **BUT** clause for that variable and one **suspension** — "when this is unresolved, do X / ask Y / escalate to a human."
5. Next time you delegate that task, add those two lines to the brief. Notice what changes in the output — and what new gap appears in its place.

The gap never closes completely. That's not failure. That's the job: the boundary work is the work.

## Related Pages

[[The Review-First Pattern]] · [[Intent Scaffolding]] · [[06-Glossary/SOP|SOP]] · [[Knowledge Debt]] · [[Delegation Thinking]] · [[The Vibe Compiler]]

## Tags

#concept #mindset #workflow #orchestrator
