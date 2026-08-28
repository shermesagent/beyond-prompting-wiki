---
title: Run-to-Run Variance
created: 2026-08-28
updated: 2026-08-28
type: concept
tags: [concept, workflow, orchestrator, practice]
sources:
  - raw/articles/human-llm-screening-workflows-2608.26885.md
  - raw/articles/mitigating-fabrication-hiring-pipelines-2608.26171.md
confidence: high
---

# Run-to-Run Variance

## What It Is

Run-to-run variance is the gap between what the same AI produces on two identical runs. Same prompt, same model, same day, same settings — and a different answer. It's not a bug report; it's a design fact about how these systems work, and it's measurable.

The cleanest measurement comes from a preregistered study of literature screening (arXiv:2608.26885): 1,131 records screened by humans and by LLMs. Two **nominally identical** runs of the same model, same configuration, agreed on 91.7% of records — and disagreed on 94. Of those 94, **29 were verified-eligible records that only one of the two runs caught.** Run the same screening twice and you miss 29 relevant studies on the second pass — or catch them on the first and think the second run is the wrong one. Neither run is "wrong." They're just different.

## Why It Matters for Moving Beyond Prompting

Every delegation is a bet on a single run. You hand a task to an agent, it returns output, you review it, you ship it. Run-to-run variance means **the output you reviewed is one sample from a distribution of possible outputs** — and the difference between samples can be the difference between catching something and missing it.

This matters more the more you move beyond prompting, for three reasons:

1. **The cost of a miss goes up with autonomy.** An operator eyeballs each answer. An orchestrator spot-checks a pipeline that runs unattended. When the pipeline runs 20 times and each run has a few percent variance, the variance compounds into a steady drip of small misses you never see.
2. **Review trains you on a moving target.** If you calibrate your trust on run #7 and run #8 comes back different, your calibration data is contaminated. You can't learn "this pipeline is reliable" from one good run — you learn it from the *distribution* of runs.
3. **The fix is embarrassingly cheap.** You don't need better AI. You need one more run.

## How to Spot It in Your Day

- You re-run a prompt "to check" and get a different result — and you can't tell which one is right.
- A pipeline that "passed" last week fails today on identical input.
- You ask the AI the same question twice in one session and get two different answers — and you assume the second one is better (it isn't automatically).
- Your review notes say "output was good" but you only ever saw one output.

## Try This

**The Two-Run Test (5 minutes).** Pick your most-delegated task. Run it twice, back to back, same prompt, same template, no changes. Then:

1. Put the two outputs side by side.
2. Mark every difference: wording, structure, facts, omissions, additions.
3. Classify each difference: cosmetic (fine), material (one run has info the other lacks), or contradictory (they can't both be right).
4. If you found material or contradictory differences, that task needs a **built-in second run** before you ship — and a rule for what happens when the runs disagree (tiebreak: run a third time, or route to a human, or flag for review).

The point isn't that the AI is flaky and can't be trusted. The point is that **"checked once" is not "checked."** A second run is the cheapest verification instrument you own — cheaper than a review checklist, cheaper than a second model, cheaper than a human reviewer. Most people never use it because they assume identical inputs produce identical outputs. They don't.

## Why "Checked Once" Is Not "Checked"

The screening study's other finding sharpens this: LLM performance depended more on the *workflow* (file-batch vs. all-at-once) than on the model. And in the hiring-pipeline study (arXiv:2608.26171), a newer-generation model still fabricated at a 90.0% baseline rate — model progress alone didn't fix the problem. The same logic applies to variance: **don't assume a better model will make the re-run unnecessary.** The re-run is a workflow property, not a model property. Build it in.

## Related Pages

[[The Review-First Pattern]] · [[The Confidence Gap]] · [[The Observability Gap]] · [[Distributed Counsel]] · [[Build a Tiny Pipeline]] · [[Trust Calibration]]

## Tags

#concept #workflow #orchestrator #practice
