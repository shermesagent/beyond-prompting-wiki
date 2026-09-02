---
title: The Failure Review
created: 2026-09-02
updated: 2026-09-02
type: concept
tags: [concept, workflow, orchestrator, research]
sources: [raw/articles/ai-morbidity-mortality-framework-2609.00076.md]
confidence: medium
---

# The Failure Review

## What It Is

When an AI system in your workflow does something wrong — a wrong number, a wrong note, a wrong decision that slips past review — most organizations do one of two things: fix the output quietly and move on, or look for someone to blame. **The Failure Review** is a third option, borrowed from medicine's "morbidity and mortality" conferences (where hospitals review deaths and complications to learn, not to punish): a structured, blameless ritual for dissecting what went wrong so the *system* gets better instead of the incident getting buried.

A 2026 framework paper (arXiv:2609.00076) argues that aggregate monitoring ("the model's accuracy dipped") and traditional incident reporting ("something bad happened") both fail to explain **how risk actually emerged** — across the interaction of the AI, the human operator, the workflow, and the organizational controls around it. The Failure Review answers that with four linked questions, applied to a single case:

| Dimension | Question it answers | Example |
|-----------|--------------------|---------|
| **Trigger** | What condition exposed the vulnerability? | "The agent was given access to the full customer database at 2am, outside normal review hours." |
| **Mechanism** | What process produced the risk? | "The agent's instruction said 'resolve all tickets' with no escalation rule for refunds." |
| **Consequence** | What did it do to the work (or the person)? | "A refund was issued twice. Customer notified of the error." |
| **Corrective Action** | What fix is assigned, and to whom? | "Add a refund-hold rule; re-run last 90 days of tickets; owner: ops lead." |

The framework's discipline: **preserve the evidence** (freeze the prompts, logs, and outputs before anyone "cleans up"), review the case blamelessly, and **track the corrective action** until it's done. In the paper's demonstration, two independent clinician reviewers applied all four axes to the same cases and agreed on every classification — the structure is teachable, not a vibe.

## Why It Matters for Moving Beyond Prompting

The shift to orchestrator means you delegate real work to agents — and real work fails sometimes. The operator's failure response is "the AI is bad" or "I prompted wrong." The orchestrator's failure response is a review: *what exposed this, how did the risk travel, what do I fix so it doesn't happen again?*

The Failure Review is also the organizational answer to a problem this wiki keeps circling: when AI is in the loop, **blame stops being useful** (see [[No One to Blame]]). Nobody can point at the "responsible" node in a human-AI-workflow tangle. The Failure Review gives you a blameless alternative that still produces learning — which is the only thing blame was ever for.

It pairs with [[The Review-First Pattern]] (check work *before* it ships) and [[Failure-Path Preservation]] (design so failures stay *visible*) as the third leg: when a failure happens anyway, review it *properly*.

## How to Spot It in Your Day

- An AI output went wrong, someone fixed it, and you never heard about it again — the fix was silent and the lesson evaporated.
- A meeting about an AI mistake turned into "whose fault is this?" within five minutes.
- Your team has a "lessons learned" habit for human errors but nothing for AI errors.
- You keep seeing the *same kind* of AI failure recur — the tell-tale sign no one ever reviewed the first one.

## Try This

**The 10-Minute Failure Review** — next time a delegated AI task produces something wrong:

1. **Freeze the evidence.** Copy the prompt, the agent's log, and the output before touching anything. (If you can't reconstruct what happened, that's finding #1.)
2. Write the four rows of the table above: Trigger, Mechanism, Consequence, Corrective Action. One sentence each.
3. Read the Mechanism row out loud and check: does it name a *process*, not a person? If you wrote "Sarah didn't check it," rewrite it as "no checkpoint existed between the agent and the customer."
4. Assign the Corrective Action to a named owner and a date. Add it to your next standup.

You've just turned an embarrassing incident into the fourth leg of your delegation system. Do this three times and you'll start noticing the same triggers recurring — that's the point: the fourth failure gets prevented instead of reviewed.

## Related Pages

[[From Prompt to Pipeline]] · [[The Review-First Pattern]] · [[No One to Blame]] · [[Failure-Path Preservation]] · [[Trust Calibration]]

## Tags

#concept #workflow #orchestrator #research
