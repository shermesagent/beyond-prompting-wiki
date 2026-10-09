---
title: The Evidence Ticket
created: 2026-09-18
updated: 2026-10-09
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
  - raw/articles/checkable-delegation-reasons-2610.00961.md
  - raw/articles/graepel-reasoning-ledger-mittr-2026-10-02.md
  - raw/articles/wired-muse-relationship-profiles-2026-10-03.md
  - raw/articles/wired-nurse-scheduling-appeals-2026-10-02.md
  - raw/articles/wired-amazon-data-center-ndas-2026-10-02.md
  - raw/articles/intent-graph-analytical-paths-2610.11025.md
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

## The Reversal Line: Could Someone Test Your Reason?

Add a seventh line to the ticket for **consequential** recommendations: `What changed fact would reverse this choice, and where can I check it?` In a conceptual delegation paper, Lumbroso argues that approval without a checkable reversal condition can become a rubber stamp. Graepel's MIT Technology Review essay makes the separate case for a visible record of evidence and unanswered questions rather than a polished story of thinking. These are proposals and an expert argument, **not** a validated scoring tool. ^[raw/articles/checkable-delegation-reasons-2610.00961.md] ^[raw/articles/graepel-reasoning-ledger-mittr-2026-10-02.md]

**Try it (3 minutes):** on a public-data recommendation, fill `Choice / Source fact / If that fact changed / Who checked it`. If the AI cannot name the condition or the source is unavailable, keep the output in draft; do not pretend the extra line verified it. [[The Reversal Condition]] has a five-minute flip test. For district work, use only approved systems and de-identified examples; a teacher or other authorized reviewer owns the decision.

## Close the Loop on a Correction

Three reported stories put the ticket's limits in view: an assistant may infer information about people who never joined, a nurse may struggle to get a local schedule corrected, and a public disclosure pledge may leave contractor-held facts out of reach. The common test is not whether the system offers a log or feedback form; it is whether the affected person can **see the relevant fact, reach an authorized editor, and confirm the changed version**. These are journalistic accounts in different settings, not a validated universal protocol. ^[raw/articles/wired-muse-relationship-profiles-2026-10-03.md] ^[raw/articles/wired-nurse-scheduling-appeals-2026-10-02.md] ^[raw/articles/wired-amazon-data-center-ndas-2026-10-02.md]

Add a small correction receipt when a consequential result is disputed: `AFFECTED ROLE / ERROR REPORTED / OWNER + DEADLINE / EXACT CHANGE / INDEPENDENT READ-BACK`. Try it with a throwaway, public-information draft and a planted error; never use live student, patient or personnel records for the exercise. [[The Absent Person Test]] identifies who needs the path; [[Procedural Standing]] asks whether it is usable.

## Save the Unchosen Question (October 2026)

An AI-made chart can look finished while hiding how a broad question became that particular chart. The Intent Graph preprint proposes an interface that shows branches from a question to possible analyses and the data fields behind them; its abstract describes a usage scenario and a planned user study, **not evidence that this interface improves decisions**. Use the idea as a paper exercise, not a product endorsement. [Yang and colleagues, preprint](https://arxiv.org/abs/2610.11025).

**Try it in five minutes with a public dataset:** write your starting question, two possible narrower questions, and the actual field you would need to answer each. Choose one route. Add to the ticket: `CHOSEN QUESTION / DATA FIELD CHECKED / ALTERNATIVE QUESTION / WHY NOT CHOSEN`. If the necessary field is missing, label the answer unsupported; do not let a polished graph stand in for evidence. Compare this with the task-fit check in [[First Delegation]] and keep the final approval human-side through [[The Review-First Pattern]]. Never use identifiable school records in an unapproved tool.

## Related Pages

[[Build a Tiny Pipeline]] · [[First Delegation]] · [[The Daily Standup]] · [[The Evidence Interface]] · [[The Review-First Pattern]] · [[Trust Calibration]] · [[The Translation Layer]] · [[The Reversal Condition]]

## Tags

#practice #orchestrator #workflow
