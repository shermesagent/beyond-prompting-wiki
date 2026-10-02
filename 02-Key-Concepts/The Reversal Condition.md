---
title: The Reversal Condition
created: 2026-10-02
updated: 2026-10-02
type: concept
tags: [concept, orchestrator, practice]
sources:
  - raw/articles/checkable-delegation-reasons-2610.00961.md
  - raw/articles/graepel-reasoning-ledger-mittr-2026-10-02.md
confidence: medium
---

# The Reversal Condition

## What It Is
A **reversal condition** is the fact that would make you change your mind. Instead of only asking an AI *“Why did you recommend this?”*, ask *“What would have to be different for you to recommend something else?”* Then check that fact in a source outside the AI.

This is a practical interpretation of [Lumbroso's proposal](https://arxiv.org/abs/2610.00961), not a tested guarantee. His paper uses illustrative delegation cases, not an experiment proving that this question improves decisions. An [expert essay by Thore Graepel](https://www.technologyreview.com/2026/10/02/1145639/dont-be-fooled-llms-dont-reason/) separately argues for keeping evidence and open questions visible rather than accepting an attractive account of how the system thought. The essay's strong claim about what counts as “reasoning” is Graepel's view, not settled fact. ^[raw/articles/checkable-delegation-reasons-2610.00961.md] ^[raw/articles/graepel-reasoning-ledger-mittr-2026-10-02.md]

## Why It Matters for Moving Beyond Prompting
An operator can accept a fluent recommendation. An orchestrator needs a decision a second person can *challenge*: which fact mattered, where it came from, and whether a change in that fact would change the action. A rationale that only sounds convincing cannot answer that question.

## How to Spot It in Your Day
A team summary recommends sending a message today. Ask: *If the deadline were next month rather than tomorrow, would this still be urgent?* Check the real deadline in the original notice. If the answer does not change when the decisive fact changes, pause rather than trusting the explanation.

## Try This — Five-Minute Flip Test
1. Use a **public, non-sensitive** draft recommendation. Write the action it suggests.
2. Write one concrete fact that *should* reverse the action. Record its original source.
3. In a copy of the draft, change **only that fact** and ask for a new recommendation.
4. Compare the decisions. If they do not change, ask which other fact is carrying the decision, then check that against the original source. If they do change, that is a useful test, **not proof** that the original decision was correct.
5. Put the fact, source, alternate outcome and human approval in [[The Evidence Ticket]]. Never test with identifiable student or personnel records in an unapproved system.

## Related Pages
[[The Evidence Ticket]] · [[The Meaning Check]] · [[The Review-First Pattern]] · [[First Delegation]]

## Tags
#concept #orchestrator #practice
