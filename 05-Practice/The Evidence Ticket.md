---
title: The Evidence Ticket
created: 2026-09-18
updated: 2026-09-27
type: practice
tags: [practice, orchestrator, workflow]
confidence: high
sources:
  - raw/articles/do-frontier-models-seek-safety-evidence-2609.17865.md
  - raw/articles/graphecho-evidence-provenance-2609.17695.md
  - raw/articles/publication-authority-challengeable-claims-2609.17631.md
  - raw/articles/teaching-memory-instructional-reasoning-2609.19488.md
  - raw/articles/cares-regulation-grounded-safety-reporting-2609.19429.md
  - raw/articles/zvi-ambition-permission-2026-09-26.md
  - raw/articles/rand-freedom-of-action-2026-09-15.md
  - raw/articles/wired-meta-muse-design-privacy-2026-09-26.md
---

# The Evidence Ticket

## What You'll Do

Before an AI workflow acts, publishes, sends, recommends, or hands work to the next step, you create a tiny ticket that says what evidence it needed, what evidence it checked, what it skipped, and what exact output you are approving.

This is not paperwork for paperwork's sake. It is a 3-minute habit that turns “the AI said it was done” into something another person can inspect.

## Why This Matters for Moving Beyond Prompting

Prompting often ends with a polished answer. Orchestration has to end with a defensible handoff.

Recent research points to the same practice from several angles: frontier models do not always seek safety evidence before acting; graph agents can walk many paths without finding independent evidence; AI-assisted publication can become impossible to challenge when the evidence, approval, and final surface refer to different versions; and saved teaching materials often preserve the artifact but lose the reasoning behind it.

The evidence ticket is the small bridge. It makes the work inspectable before trust becomes a vibe.

## The Ticket Template

Copy this into any recurring AI workflow:

```text
EVIDENCE TICKET — [Workflow / Output]

1. Evidence needed:
   What information would change whether this output is safe, accurate, useful, or ready?

2. Evidence checked:
   What did the AI actually inspect? List links, files, records, examples, tests, or people.

3. Independence check:
   Are these separate roots of evidence, or repeated paths back to the same source?

4. Skipped evidence:
   What was not checked? Why — no access, too costly, time limit, unavailable, or forgotten?

5. Reasoning note:
   Why did I accept, change, or reject the AI's output?

6. Exact state approved:
   What exact version am I approving — file name, timestamp, draft, link, or screenshot?
```

## How to Use It in Your Day

Use the ticket whenever an AI output leaves your personal scratch space:

| If the AI is... | Ticket focus |
|---|---|
| Summarizing | Which source documents were checked, and what was not included? |
| Recommending | What criteria did it use, and what evidence would change the recommendation? |
| Drafting something to send | What claims need source links, and what exact draft are you approving? |
| Building a report | Which data version, query, or file produced the numbers? |
| Reviewing another AI's work | Is this independent review, or the same evidence echoed back? |

## Try This: The 3-Minute Evidence Ticket

Pick one AI output you were already going to use today. Before you act on it:

1. Write one sentence for **evidence needed**.
2. List the actual sources/files/examples the AI used.
3. Circle anything that traces back to the same origin.
4. Name one thing you did not check.
5. Save the exact version you approved.

If you cannot fill out the ticket, don't panic. That is the point of the exercise. The workflow is telling you where it needs a better evidence interface.

## What Good Looks Like

A good ticket is short, boring, and specific:

```text
EVIDENCE TICKET — Parent email draft, attendance intervention
Evidence needed: current attendance rule, student's latest absence count, campus tone expectations.
Evidence checked: FISD attendance FAQ, Skyward absence count as of 9/18, prior principal email.
Independence check: policy and student record are separate roots; principal email is tone only.
Skipped evidence: did not check counselor notes — not needed for this routine version.
Reasoning note: accepted structure, changed sentence 3 to avoid sounding punitive.
Exact state approved: Google Doc v3, 2026-09-18 7:42 AM.
```

That is enough for future-you or a colleague to understand what happened without re-interviewing the AI.

## Add a Decision Gate for External Action

The ticket describes proof, but it also needs to say whether a conversation was **just a discussion** or **permission to act**. A September 26 practitioner essay quotes a user whose agent sometimes treated hypothetical talk as a cue to proceed. Do not infer how often that happens from one report; use it to test whether your own brief distinguishes the two. ^[raw/articles/zvi-ambition-permission-2026-09-26.md]

Before a pilot sends, changes, buys, or accesses sensitive information, add four short lines to the ticket:

```text
Status: DISCUSS ONLY / DRAFT ONLY / APPROVED TO ACT
Approval: named person and exact action approved
Review date + evidence: what would expand or end this pilot?
Exit: who can stop it and how does the manual route work?
```

The review-date idea is an analogy to RAND's strategy for preserving options under uncertainty, not an intervention RAND tested on teams. When the tool has a friendly face, add an *affected-person check*: WIRED's Muse report raises concrete age-access and training-use questions. Before a district trial, obtain approved privacy review; do not paste live student or personnel data into an unapproved service. ^[raw/articles/rand-freedom-of-action-2026-09-15.md] ^[raw/articles/wired-meta-muse-design-privacy-2026-09-26.md]

**Five-minute trial:** use a public document and ask the agent to draft a summary without sending it. Fill the four lines above, then see whether any proposed step crosses the approval boundary. [[The Absent Person Test]] catches people the task brief forgot; [[The Control Surface]] supplies the stop handle.

## Related Pages

[[Build a Tiny Pipeline]] · [[First Delegation]] · [[The Daily Standup]] · [[The Evidence Interface]] · [[The Review-First Pattern]] · [[Trust Calibration]] · [[The Translation Layer]]

## Tags

#practice #orchestrator #workflow
