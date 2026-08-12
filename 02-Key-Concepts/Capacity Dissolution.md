---
title: Capacity Dissolution
created: 2026-07-31
updated: 2026-08-11
type: concept
tags: [concept, barriers, practice, orchestrator, skill-erosion]
sources:
  - arXiv:2607.28041
  - arXiv:2607.27586
  - raw/articles/longitudinal-human-ai-measurements-2608.02491.md
  - raw/articles/unaccountable-delegation-fading-skills-2608.08601.md
confidence: medium
---

# Capacity Dissolution

## What It Is

Capacity dissolution is the erosion of five specific human capacities that occurs when AI systems produce outputs — essays, code, reports, decisions — through which institutions traditionally recognize competence. Named and analyzed by Kai Yao (AAAI/ACM AIES 2026), the concept argues that each technical improvement in AI weakens the case for preserving human capacity unless we deliberately design for preservation. The five capacities are:

1. **End-setting** — the ability to define what purposes are worth pursuing. When AI sets the agenda for what gets done, humans lose the practice of deciding what matters.

2. **Reason-giving** — the ability to explain and justify choices. When AI produces the output but humans can't articulate why it's right (or wrong), the reasoning capacity atrophies.

3. **Contestability** — the ability to challenge, dispute, and interrogate outputs. When polished artifacts arrive complete and convincing, the instinct to question them fades.

4. **Refusal/revision** — the ability to say "no" or "not good enough" and demand better. When AI output is always "good enough," the standards that drive revision weaken.

5. **Participation** — the ability to engage meaningfully in the practices AI mediates. When AI handles the work, humans become spectators to their own professional domain.

The central case is assessment: when a polished artifact no longer reliably evidences understanding, institutions must assess the learner's **accountable relationship to AI-mediated work** rather than the artifact alone.

## Why It Matters for Moving Beyond Prompting

The operator→orchestrator shift promises leverage — more output with less effort. But Yao's framework names the hidden cost: **every delegation that skips capacity preservation is a withdrawal from a limited account.** The orchestrator who delegates output without preserving end-setting becomes reactive. Without reason-giving, they become opaque to colleagues. Without contestability, they become credulous. Without refusal, their standards drift downward. Without participation, they become replaceable.

This concept bridges the [[04-Barriers-and-Bridges/README|Barriers & Bridges]] section and the [[05-Practice/README|Practice]] section. Capacity dissolution is the barrier. The three-week practice progression is the bridge. Every exercise in the practice section targets at least two of the five capacities:

| Exercise | Capacities Preserved |
|----------|---------------------|
| [[Audit Your Prompts]] | End-setting, Participation |
| [[The Line You Draw]] | End-setting, Refusal/revision |
| [[First Delegation]] | Reason-giving, Contestability |
| [[Build a Tiny Pipeline]] | End-setting, Reason-giving, Participation |
| [[The Daily Standup]] | Contestability, Refusal/revision |

## Evidence

The N=220 randomized study by Dickey et al. (arXiv:2607.27586) provides direct evidence for a related phenomenon: **evaluating AI output and solving problems yourself are different muscles.** Students who only evaluated GenAI solutions earned higher homework scores but showed no transfer to exams — their evaluation skill didn't build their solving capacity. This is capacity dissolution in microcosm: the student who can spot an error in AI output but can't solve the problem themselves has preserved contestability while losing reason-giving and end-setting.

### The Longitudinal Blindspot (August 2026)

There's a measurement problem hiding inside the dissolution story, and a new position paper names it directly (arXiv:2608.02491, August 2026). Language models integrate into daily life in ways that are *human-like* and *continuous* — which means their risks are **longitudinal**: cognitive, developmental, and socio-affective changes that "might not surface in short-term interactions, but can have lasting long-term effects on users."

The paper's core argument: NLP evaluation has been static and short-term (does this response look good?), but the risks that matter are diachronic (is this *relationship* changing the user?). It calls for long-term measurements of behavioral change, online rather than post-hoc detection of problematic patterns, and modeling "human behavioral shifts as a function of model interactions."

**Why this matters for the five capacities:** every dissolution mechanism on this page is a *longitudinal* phenomenon — erosion that compounds across repeated interactions, invisible in any single one. A student who checks their work for a week sees no change. The problem is the pattern across months. That's exactly why the Capacity Check (below) is phrased as a *recurring* practice: a single check catches nothing; a weekly check over a year catches the drift curve. You can't detect dissolution in the moment any more than a static NLP benchmark can — you can only detect it in the series. Run the check. Log the answers. Compare across weeks. The measurement is the antidote.

## How to Spot It in Your Work

You're experiencing capacity dissolution when:

- You can accept or reject AI output but can't explain *why* it's right or wrong (reason-giving erosion)
- You find yourself doing whatever tasks the AI surfaces rather than deciding what matters (end-setting erosion)
- You've stopped challenging AI output because it's "usually fine" (contestability erosion)
- Your quality bar has drifted to "whatever the AI produces" (refusal/revision erosion)
- You describe your role in terms of what the AI does rather than what you do (participation erosion)

## The Capacity Check (30 Seconds)

After any AI delegation, ask:

1. Did I set the end, or did the AI? (End-setting)
2. Can I explain why this output is right (or wrong)? (Reason-giving)
3. Did I challenge anything in this output? (Contestability)
4. Did I reject or revise anything? (Refusal/revision)
5. Was I engaged, or was I spectating? (Participation)

If you answered "no" to three or more, that interaction produced output but dissolved capacity. That's not always wrong — some tasks genuinely don't require capacity preservation. But if the pattern holds across a week of work, the capacity cost is compounding.

### The O*NET Risk Map: Fading Skills Is a Measured Risk, Not a Fear (August 2026)

The dissolution story now has an empirical map. La Malfa et al. (arXiv 2608.08601, August 2026) generated **8,356 risk scenarios from 2,078 O*NET job tasks**, validated by 45 workers across 10 job roles, and the study's headline finding is exactly the mechanism on this page:

> **Augmentation is not inherently safe because overreliance on agents can gradually erode workers' skills and oversight.**

Two findings deserve emphasis:

1. **The erosion is slow-onset and sits in the augmentation mode.** Automation (agent replaces task) was associated mainly with *organizational* risks. Augmentation (agent assists task, human stays nominally in the loop) was associated mainly with *risks to workers* — including skill and oversight erosion. The "helpful assistant" mode is the one that dissolves capacity.
2. **Erroneous Agent Actions is the largest risk category and the most severe** — and many cases arise at the human-agent boundary. When the human-agent boundary degrades through overreliance, the failure mode that dominates is the agent doing the wrong thing and the human not catching it: exactly the "accept or reject but can't explain why" state from the Capacity Check above.

The study's own conclusion is the point of this page: *"Workplace AI agent risks do not arise from agents alone; they also depend on how people work with agents."* Capacity dissolution is a risk of the *relationship*, not of the tool — which is why the fix is a recurring capacity check, not a better model.

**Source:** "Unaccountable Delegation, Fading Skills: Mapping the Risks of Workplace AI Agents," arXiv 2608.08601 (August 2026)

### The GenAI Catch-22: The Erosion Loop, Measured in a Newsroom (August 2026)

The dissolution mechanism now has a field observation with an official name: the **GenAI Catch-22**. In a ten-month case study of Norwegian newsrooms during the 2025 parliamentary election (Reisjå & Løvlie, arXiv 2608.10773, August 2026), researchers watched institutions try to build audience-facing GenAI products — and watched the ambitions collapse as the real pattern emerged: **mundane internal GenAI use quietly eroding the expertise that monitoring requires.**

The Catch-22, stated by the researchers: **monitoring GenAI requires human expertise — but extensive GenAI use deteriorates exactly that expertise.** The more the newsroom leaned on the tool, the less able it was to supervise the tool. It's the Capacity Check from this page, run at institutional scale:

- The *internal* threat (journalists' own AI use eroding their skills) outweighed the *external* threat (disinformation) they had prepared for.
- Overoptimistic managerial beliefs about AI's capabilities widened the gap between the imagined product and the real tool — making the collapse more expensive.
- What survived the collapse was mundane internal use: GenAI inside existing workflows, where the erosion risk was managed by the routine, reviewable shape of the work.

The transfer to your day: **the erosion loop runs wherever GenAI output is consumed without a capacity-preserving practice attached.** The newsrooms are the district office, the bakery, the hospital admin floor — the Catch-22 is the dissolution mechanism named after a decade of observation, and the counter-measure is the same one this page has always recommended: keep the check, keep the manual path alive, and treat "the AI will catch its own errors" as the specific belief that dissolves the fastest.

**Source:** Reisjå, M. & Løvlie, A.S. "The GenAI Catch-22: Use of Generative Artificial Intelligence in Norwegian Newsrooms During the 2025 Parliamentary Election." arXiv 2608.10773 (August 2026)

## Related Pages

[[06-Glossary/Capacity Dissolution|Quick reference]] · [[The Coaching Stance]] · [[Cognitive Surrender]] · [[The Absorption Pattern]] · [[The Augmentation Trap]] · [[Friction by Design]] · [[From Author to Editor]] · [[Trust Calibration]]

## Tags

#concept #barriers #practice #orchestrator #skill-erosion
