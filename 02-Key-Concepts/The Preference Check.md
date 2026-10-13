---
title: The Preference Check
created: 2026-10-13
updated: 2026-10-13
type: concept
tags: [concept, mindset, workflow, orchestrator]
sources:
  - raw/articles/latent-preference-observation-2610.13185.md
  - raw/articles/agent-naming-user-behavior-2610.13156.md
confidence: medium
---

# The Preference Check

## What It Is
A person repeating an action is not the same as that person **choosing** a lasting rule for an AI. They may be working around a bad menu, following a temporary deadline, or simply trying something. The Preference Check asks: *Before I turn this pattern into an automatic default, has the person had a clear chance to say what they want?*

A theoretical [study of preference learning](https://arxiv.org/abs/2610.13185) shows why observation alone can be ambiguous under its model: different underlying situations can produce identical actions. A separate [desktop-assistant field study](https://arxiv.org/abs/2610.13156) found that people who renamed the assistant used it differently and tended to prefer different replies. That association is useful for offering choices, **not** proof of a person's identity, intent, or consent. ^[raw/articles/latent-preference-observation-2610.13185.md] ^[raw/articles/agent-naming-user-behavior-2610.13156.md]

## Why It Matters for Moving Beyond Prompting
An operator checks one answer. An orchestrator sets defaults for repeated work. At that point, a mistaken guess about someone's wishes can be repeated at scale. Ask once at the point of reuse; keep the setting editable and let the person change it. A warmer greeting, for example, is not permission to read more files or contact anyone on their behalf.

## How to Spot It in Your Day
- An assistant proposes a permanent style because you used it in one rushed email.
- A team turns last month's workaround into the standard procedure without asking why it happened.
- A conversational tool interprets friendly language as a request for more personal involvement.

## Try This
**Five-minute preference card:** On a public, low-stakes recurring task, write three lines before saving any AI default:

1. **Observed:** What did the person actually do? (No mind-reading.)
2. **Ask:** “Was that your preferred way, or just what worked today?”
3. **Scope and change:** “Use this only for [task]; ask again before [higher-stakes step]. Change it by [simple route].”

If you cannot ask the person, leave the behavior as a suggestion, not a permanent rule. For students or staff, use only district-approved tools and policies; do not infer preferences from private activity logs.

## Evidence Boundary
The preference-learning result is mathematical under specified assumptions and **does not** establish a validated real-world questioning method. The desktop study reports associations and reply judgments in one assistant setting; it does not show that renaming *caused* a need for a particular style. The card above is a cautious workflow proposal, not a tested intervention.

## Related Pages
[[Intent Scaffolding]] · [[Co-Construction Blindness]] · [[The Rule Capture Problem]] · [[The Meaning Check]]

## Tags
#concept #mindset #workflow #orchestrator
