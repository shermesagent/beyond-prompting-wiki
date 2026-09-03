---
title: The Retrievability Gap
created: 2026-09-03
updated: 2026-09-03
type: barrier
tags: [barrier, mindset, verification, orchestrator]
sources:
  - raw/articles/knowing-is-not-enough-retrievability-2609.01976.md
confidence: high
---

# The Retrievability Gap

## What It Is

You're reviewing the AI's work. You're paying attention. You have the skill to catch errors. And the mistake still sails past — because the one fact that would have exposed it wasn't reachable at the moment you reviewed.

That's the retrievability gap: **error detection depends less on how carefully you check than on whether the checking information is actually accessible when you check.** Knowing is not enough — retrievability is the precondition.

A September 2026 study put this to a direct test with 640 customer-facing employees across two randomized field experiments (arXiv:2609.01976). Their errors weren't a skill problem or a motivation problem. When the reasoning needed to verify an LLM output was accessible at review time, detection improved. When it wasn't, capable, motivated people approved the wrong thing.

## Why It's Normal (or: What Makes It Worse)

When AI errors slip past review, organizations reach for two familiar fixes: **train reviewers better** (a capability problem) or **tell them to care more** (an engagement problem). The study says both miss the mechanism. The error passes because the trail that would prove it wrong — the source behind a claim, the number behind a summary, the assumption behind a recommendation — simply isn't in front of the reviewer when they look.

Worse, this is what smooth AI looks like by design. The interface shows you the polished answer, not the evidence it rests on. Your attention is the last line of defense, and the environment has quietly removed the ammunition.

So if you've approved something wrong, that's not a verdict on your vigilance. It's a description of the arrangement you were reviewing inside.

## Why It Matters for Moving Beyond Prompting

The more you delegate, the more **your review is the safety system** — and the retrievability gap is where that system fails silently. It's the difference between:

- An **operator**, who checks what they can see, and
- An **orchestrator**, who designs the deliverable so the thing they need to see is there when they check.

Every delegation pattern on this wiki — [[The Review-First Pattern]], [[The Observability Gap]], [[The Validator Trap]] — assumes a human will verify at the end. The retrievability gap says that assumption fails unless the verification information is *at hand at the moment of review*. Build the check, and you've built half the bridge; put the evidence next to the claim, and you've built the other half.

## The Bridge

Three concrete moves, each mapped to what the study found works:

| Move | What It Does | How to Do It |
|------|-------------|-------------|
| **The Pre-Review Note** | *Generative encoding:* writing your own explanation before you see the output encodes the reasoning you later check against — and measurably improves error detection | Before opening the AI's deliverable, write 2–3 sentences predicting what a correct version will claim and which facts it must get right. Read the output with your note beside it |
| **The Retrieval Cue** | *Cue-supported reactivation:* a standing cue brings verification reasoning back when vigilance decays under repeated use — the study's fix for routine, day-after-day delegation | Pick one question you ask at every review of delegated work: "Which number in here would I bet on?" "What source should back this claim?" "What did the last failure look like?" Ask it out loud, every time |
| **The Evidence-Adjacent Rule** | Fixes the arrangement itself: specify that delegated outputs carry the evidence next to each claim — sources inline, numbers traceable, assumptions stated | When you brief an agent, add one line: "For each key claim, show the source or the reasoning on the same screen." If the checking info isn't in the artifact, the review is theater |

The first two are personal practice; the third is a delegation standard. All three are cheap, and all three attack the arrangement instead of your character.

## Try This

**The 5-Minute Pre-Review Note.** Pick the next AI deliverable on your list — a draft, a summary, a data pull. Before you open it, write two sentences: *"A correct version of this will claim... and it will get these facts right..."* Then review the output with your note beside it.

Count the disagreements. That count is your retrievability score for that task — and it will tell you, faster than any training, which of your delegated tasks hand you the evidence and which hand you a verdict.

## Related Pages

[[The Review-First Pattern]] · [[The Observability Gap]] · [[The Validator Trap]] · [[Knowledge Debt]] · [[Trust Calibration]] · [[Run-to-Run Variance]]

## Tags

#barrier #mindset #verification #orchestrator
