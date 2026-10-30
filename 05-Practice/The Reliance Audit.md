---
title: The Reliance Audit
created: 2026-08-08
updated: 2026-10-30
type: practice
tags: [practice, operator, orchestrator, trust]
confidence: high
sources:
  - raw/articles/epistemic-trustworthiness-2608.05602.md
  - raw/articles/harmful-ai-sycophancy-2608.05624.md
  - raw/articles/chat-tjb-random-guy-wired-2026.md
  - ../../ai-agency-knowledgebase/06-Frameworks/Human Review Checkpoints.md
  - raw/articles/ai-overreliance-complex-adaptive-system-2608.19616.md
  - raw/articles/reliance-behaviors-problem-solving-2610.30195.md
  - raw/articles/productive-friction-writing-2610.30945.md
  - raw/articles/proof-learning-offloading-2610.31481.md
  - raw/articles/critical-thinking-coordination-2610.38910.md
  - raw/articles/human-planning-creative-writing-2610.37916.md
---

# The Reliance Audit

## What You'll Do

For one week, keep a running tally of every time you rely on an AI's answer — and grade each reliance against three questions. Ten seconds per interaction. One tally at the end of the week. The output is a number you can defend: **how much of your reliance is warranted, and how much is just habit.**

This is the practice-layer companion to [[02-Key-Concepts/Trust Calibration|Trust Calibration]]. The concept page gives you the framework — warranted vs. behaviorally induced reliance. This page gives you the exercise that makes the framework *yours*.

## Why This Matters

Here's the uncomfortable fact that makes this exercise necessary: **people will rely on a chatbot that isn't even a chatbot.** In July 2026, an artist put up a $6,000 San Francisco billboard advertising free advice from "a random guy" — ChatTJB. The twist: there is no AI. A human answers every prompt by hand. By August 6, ChatTJB had logged **30,000+ queries**, peaking around **5,000 prompts an hour**, and people were asking it real, personal questions — birthday party dilemmas, dinner decisions, what to do with the ingredients in their pantry.

The artist's own framing: we've drifted into **cognitive surrender** — accepting outputs with less and less scrutiny. He describes deferring to an AI about San Francisco weather even though he'd lived there for seven years: "it felt like an easier thing for me to defer to."

Nobody is immune to this. The question is whether your reliance is *warranted* — and warrant, per the research framework, has three testable conditions:

1. **Epistemic humility** — the tool represents and communicates the limits of its competence (it says "I don't know" / "this is outside my training")
2. **Epistemic access** — you can inspect, question, and contest the output in context (you can check the reasoning, the sources, the steps)
3. **Resistance to epistemic injustice** — the tool treats your knowledge and experience as legitimate (it doesn't steamroll your disagreement)

Reliance that meets all three is warranted. Reliance that meets none is surrender. Most of your reliance probably lives in between — and that's exactly what the audit measures.

## The Three-Question Audit

### Setup (2 minutes)

Keep a note file (or a paper tally) with three columns. Label them:

```
Q1 HUMILITY   — did the tool signal the limits of its own competence?
Q2 ACCESS     — could I inspect, question, or contest the output?
Q3 JUSTICE    — did it treat my knowledge/disagreement as legitimate?
```

### The Habit (10 seconds per interaction)

Every time you rely on an AI answer — for a decision, an email you send, a number you quote, a plan you act on — mark the three columns. **You only tally the interactions you actually acted on or accepted.** Not the curiosity prompts. The reliance.

### The Weekly Tally (Sunday, 10 minutes)

Count your interactions. For each of the three questions, ask: how many of my reliances passed?

- **All three, most of the time** → your reliance is warranted on this kind of task. Keep going; your trust is earned.
- **One or two, inconsistently** → your reliance is partial. You're relying on a tool that doesn't tell you its limits, or that you can't inspect. That's a fixable tool problem — or a fixable *task* problem (see below).
- **None, most of the time** → you're running on habit. You are the ChatTJB user. This is the week to change what you rely on.

### The Two Follow-Ups (only if warranted)

**The Stance-Reversal Probe.** Research on harmful sycophancy (arXiv:2608.05624) measured *preference-induced stance reversal* across 17 models — how often a model flips its initial stance to agree with the user's stated preference. The base rate: **5–56%**, depending on model, with more capable models reversing less. To probe your own tool: state a clear preference ("I'm pretty sure X is the right call"), ask for its honest assessment, then check whether its answer changes when you state the opposite. If it reverses with your stated preference, it has no stable stance for you to rely on — mark Q1 and Q3 as failed for that tool, not for that interaction.

**The Random-Guy Test.** Before acting on a consequential answer, ask: *would I act on this if it came from a random guy on a billboard?* If you'd verify the random guy's advice — check his reasoning, sanity-check the numbers, ask a second source — verify the AI's at least that much. The test isn't "don't trust AI." It's "**trust it exactly as much as the warrant supports, not as much as the interface invites.**"

## The Replacement Rule

If a tool fails **all three questions twice on the same task**, it's not a tool you're using — it's a habit you're carrying. Put it on probation: either rebuild the workflow with review checkpoints (see [[First Delegation]] and its REVIEW CADENCE), or replace the tool. This mirrors the AI Agency Knowledgebase's Human Review Checkpoints framework: checkpoints belong *inside* the workflow, not at the end of it.

## The Visibility Effect: Verification Is Social

Your audit tallies verification as a private act — you checked, or you didn't. New population-level modeling of AI reliance (Biswas, arXiv:2608.19616) adds a social dimension your tally is missing: **whether other people can see you verify changes whether *they* verify.**

The model treats a whole group of users as one system, with three results that reframe the audit:

1. **The environment sets the baseline.** Task difficulty and AI quality fix how much overreliance a population can fall into — before anyone's habits enter the picture.
2. **Social proof turns reliance into a cascade.** When people can see others *using* AI output without checking it, verification gets suppressed and the whole group tips into **collective overreliance** — even users who privately knew better.
3. **Visible verification reverses it.** Making your checking visible — or dampening the social proof of unchecked use — prevents the collapse. One person's visible verification is a public good.

### The Audit Addition (30 seconds)

In your weekly tally, add one column:

```
VISIBILITY — did anyone see me verify this?
```

Three grades:

- **Invisible:** I checked it, quietly. Good for me; useless to the team.
- **Visible:** I checked it and said so — "I ran this past a second source before sending" in the channel where others saw it.
- **Exported:** I showed *how* — the check itself is reusable (a link, a rubric, a named step). This is the one that changes group behavior.

The mechanism is the same one that runs the ChatTJB story above: people calibrate to what they see around them. The audit's Q2 (ACCESS) asks whether *you* can inspect the output. The visibility column asks whether your inspection is *contagious* — and that's what protects a team, not just a person. See [[The Daily Standup]]'s Eleventh Question for the habit that makes visibility routine.

## Where This Fits

### Add a use-pattern note, not a personality label

A new scale study of **undergraduate** problem solving grouped self-reported AI use into reflective, cautious, thoughtless and collaborative patterns across several activity samples. Its reliability and fit tests support a measure of *reported behavior*; they do not show which pattern improves learning, or diagnose a person from one chat. [Hou and colleagues, preprint](https://arxiv.org/abs/2610.30195).

**Try this with one public, low-stakes task (3 minutes):** next to your three-question tally, write `My first thought / AI suggestion / What I accepted, changed or checked / Why`. If the answer is “I copied it,” don't mark yourself as a type. Pick one claim to verify next time. The point is to see *how* you relied, not to chase a good-looking score.

Two companion studies suggest a useful boundary: a randomized writing study reported better writing and short-lag transfer with goal-and-step scaffolds even though participants found AI less helpful; an undergraduate proof course saw better AI-supported homework without a detectable exam difference, and more chatbot messages were **associated** with lower later exam scores. Neither tests this audit. For a task where you want to learn, write your own attempt before a hint and later try a new instance without AI. [Writing experiment](https://arxiv.org/abs/2610.30945) · [Proof-course study](https://arxiv.org/abs/2610.31481). See [[The Daily Standup]] for the next-day check.

- Run it during Week 1 alongside [[Audit Your Prompts]] — the audit shows you *what* you do; this shows you *how warranted* it is.
- Use the results to decide what enters your [[First Delegation]] pipeline — only tasks where the tool passes Q1–Q3 are safe to delegate.
- Re-run for one week every quarter. Reliance drifts; the audit recalibrates.

### The Plan–Draft–Change note (October 2026)

Two new preprint abstracts offer a useful way to describe a single *interaction*, rather than label the person using AI. In a writing-chain study with 333 participants and 427 stories, putting a human at the planning stage best balanced creativity and story diversity in that experimental setup. A separate structural study of 891 college students linked critical-thinking measures to how participants divided work with AI and actively reworked its output. Neither paper tests this audit, and the latter is not a causal training trial. [Writing study](https://arxiv.org/abs/2610.37916v1) · [Critical-thinking study](https://arxiv.org/abs/2610.38910v1).

**Try this with a public or fictional draft (3 minutes):** jot `MY PLAN: audience and purpose / AI'S PART: one draft step / MY CHANGE: one decision I revised and why`. Compare it to the output. If you made no change, that is information about this run—not a diagnosis. A human plan is not a substitute for checking facts against a source. Take the note to [[The Daily Standup]] for tomorrow's review.

## Related Pages

[[02-Key-Concepts/Trust Calibration|Trust Calibration]] · [[Audit Your Prompts]] · [[First Delegation]] · [[02-Key-Concepts/Cognitive Surrender|Cognitive Surrender]] · [[The Line You Draw]] · [[02-Key-Concepts/Accountability Asymmetry|Accountability Asymmetry]]

## Tags

#practice #operator #orchestrator #trust
