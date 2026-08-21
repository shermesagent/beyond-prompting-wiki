---
title: The Practice Style
created: 2026-08-21
updated: 2026-08-21
type: concept
tags: [concept, practice, skill-formation, evaluation, operator]
confidence: high
sources:
  - raw/articles/when-the-scaffold-stays-on-2606.06253.md
---

# The Practice Style

## What It Is

Your **practice style** is the mode you use AI in while you're still learning something — and it comes in two flavors:

- **Substitute mode:** AI stands in for the practice itself. The AI does the reps, you accept the output. Today's task gets done faster; tomorrow's skill never gets built.
- **Complement mode:** AI accelerates the practice. You do the attempt, the AI critiques it, you debug together. Today's task takes about the same; tomorrow's skill grows.

Same tool. Same task. Different mode — and the mode, not the tool, decides whether your ability grows or erodes.

## Why It Matters

This is the practice-layer version of [[Scaffold, Don't Substitute]] — the design principle applied to your own learning. The substitution problem isn't only something systems do to people. It's something people do to themselves, quietly, one accepted answer at a time. And because the substitute mode feels *exactly* like productivity (the task finished faster!), it's nearly invisible from the inside.

The research that names this comes from elite competitive programming (Yao, arXiv:2606.06253). Two very different environments:

- **Codeforces** — unproctored, open to everyone, AI allowed. Practice shifted toward an "AI-prompt signature" (first-attempt acceptances, fewer attempts, fewer debugging retries).
- **ICPC / IOI** — the elite contests, AI **prohibited** under in-person proctoring.

The key finding: in unproctored Codeforces, a stronger AI signature predicted **smaller rating gains** for users who never qualified for the proctored contests — the substitute users weren't growing. But for users who *had* qualified, the AI signature predicted no loss. And inside the proctored ICPC environment, AI-style practice predicted **higher** non-AI scores for the AI-era entrants.

The same behavior, carrying opposite signs in the two environments — that's exactly what a **separating gate** looks like. The gate doesn't punish AI use. It separates the mode: if your skill is real, it survives the no-AI screen; if it was the AI's skill, the screen says so.

## How to Spot Your Own Mode

| Signal | Substitute mode | Complement mode |
|--------|-----------------|-----------------|
| First draft | Accepted as-is, almost always | Treated as a starting point to argue with |
| Retries | Rarely needed — AI fixes it | Normal — you debug together |
| After the task | Couldn't reproduce it without AI | Can do it (slower, maybe) on your own |
| Your role | Approve | Attempt, critique, revise |
| Time feel | Fast, effortless | About the same, engaged |

## Try This: The Weekly Gate

You don't need a proctored contest to run a gate. Once a week, pick one practice task and impose **AI-prohibited rules on yourself** — no AI until your own attempt is complete. Then compare:

1. Could you produce a real attempt at all? (If not, you've been substituting — the gate just told you.)
2. How far was your attempt from the AI's version? (Far apart → you're learning. Near-identical → the AI is doing the thinking.)
3. Now let the AI critique *your* version instead of writing one. That's the complement move.

This is the same pattern as [[The Scaffold Match]]'s rule to test the tool's default intervention level — except the tool is you. The weekly gate is a 20-minute check that your practice is actually yours.

## The Constructive Message

The paper's message is deliberately constructive, and it's worth holding onto: **AI-style practice is compatible with frontier skill.** The erosion risk isn't in using AI — it's in the substitute mode. And that mode is separable by gates, the kind already standard at credential boundaries: medical boards, legal bars, professional certification. If you're designing training for other people, the design question is never "allow AI or not?" It's "how do we govern the *mode* of use?" — and the answer is a gate that screens the mode, not the tool.

## Related

- [[Scaffold, Don't Substitute]] — the design-side version of this principle
- [[The Scaffold Match]] — matching the tool's intervention level to the learner's gap
- [[First Delegation]] — know your practice style before you delegate the thing you're still learning
- [[The Line You Draw]] — the boundary check for what never gets fully handed over
- [[Audit Your Prompts]] — the audit reveals your delegation default; this page names the mode behind it
- **The augmentation benchmark (KB cross-pollination)** — CentaurBench (arXiv:2608.18554) shows automation rankings barely predict augmentation quality: the automation winner loses on 5 of 7 assistance tasks, and only one model's guidance beats no guidance on average. Same lesson at benchmark scale: "can it do the task?" and "does it make *you* better?" are different questions — judge assistance on assistance evidence, the way the Weekly Gate judges your mode.
