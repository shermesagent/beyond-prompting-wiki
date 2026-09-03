---
title: The Review-First Pattern
created: 2026-06-30
updated: 2026-09-01
type: concept
tags: [concept, workflow, orchestrator]
sources: [raw/articles/viktor-agents-cannot-do-2026.md, raw/articles/automation-boundaries-2026.md, raw/articles/hallucination-snowball-2608.14588.md, raw/articles/uncertainty-isnt-enough-self-correction-2608.14659.md, raw/articles/crossaudit-cross-vendor-audit-2608.28631.md, raw/articles/one-note-in-three-ai-scribes-2608.31017.md]
confidence: high
---

# The Review-First Pattern

## What It Is

The review-first pattern is simple: **AI produces a draft. A human reviews and approves. Only then does execution happen.** It sounds obvious. It's not what most people do.

Most people in Phase 2 use what you could call the *prompt-iterate-hope* pattern: write a prompt, get a result, tweak the prompt, get another result, settle for something acceptable, copy it out. The human does the heavy cognitive lifting *at the input stage* — crafting the perfect words — and then crosses their fingers at the output stage.

The review-first pattern flips this. The human spends their cognitive energy at the *judgment stage* — deciding whether the output is good — and lets the agent handle the production. Same amount of human time. Radically different leverage point.

## Where the Evidence Comes From

This isn't a theory. It's the pattern that consistently shows up in real-world data:

- **A vendor running AI agents in production** (Viktor, 2026): After a year of running an AI coworker service with review-first defaults, they reported replacing ~18 hours/week of cross-tool work. When a customer disabled review-first, an agent sent "we apologize for the delay" to someone who had *already received a refund*. Review-first was re-enabled the next week.
- **53 adults testing automation levels** (arXiv:2606.28777, 2026): Higher automation did NOT produce higher trust. People preferred systems that reduced routine effort while preserving correction opportunities. Full automation scored lower on trust, autonomy, transparency, dignity, and satisfaction.
- **382 undergrads writing with AI** (arXiv:2606.28749, 2026): Strategic users — the ones who deliberately reviewed and overrode AI output — scored *lowest* on standard measures because the instruments indexed AI contribution, not human thinking. The review step was invisible to the metrics, but it was where the real thinking happened.
- **112 ninth graders learning math** (arXiv:2606.28472, 2026): Students who shifted from "is this right?" (verification) to "why does this work?" (conceptual review) learned more. The review step changed from a yes/no gate to a learning moment.

Across every population — students, professionals, older adults — the pattern holds: the review point is where the human adds the value that AI can't.

## Why It Matters for Moving Beyond Prompting

The review-first pattern is the practical bridge between operator and orchestrator. Here's the difference:

| | Operator (Prompt-Iterate-Hope) | Orchestrator (Review-First) |
|---|---|---|
| **Where cognitive effort goes** | Crafting the perfect prompt | Defining the deliverable + judging the result |
| **Number of interactions** | 4-6 prompt rounds per piece | 1 spec + 1 review pass |
| **What gets better with practice** | Your prompts | Your judgment about what "good" looks like |
| **Scale ceiling** | You can only prompt one thing at a time | You can queue multiple reviews |
| **What happens when you're not there** | Nothing | The draft is waiting for you |

The operator gets better at words. The orchestrator gets better at judgment. Judgment compounds — the more you exercise it, the faster you get at spotting what's good and what's not. Prompting doesn't compound the same way; there's always a new model, a new format, a new way to phrase things.

## The Review Point Is Not Busywork

A common objection: "Isn't reviewing AI output just as much work as doing it myself?"

No — for two reasons:

1. **Reviewing is faster than producing.** Reading a draft and marking what's wrong takes a fraction of the time it takes to produce the draft from scratch. An analytics practitioner who documented 90 days of agent delegation put it plainly: "editing is faster, but it's also a different skill set."

2. **Reviewing is higher-leverage than prompting.** When you're prompting, you're trying to control the AI's *process* — which words to use, which structure to follow. When you're reviewing, you're controlling the *outcome* — whether the final product meets the standard. The second one matters more and takes less cognitive energy.

## How to Spot It in Your Day

You're in prompt-iterate-hope mode when:
- You open a fresh chat for every task
- You find yourself tweaking the same prompt 3+ times
- You don't have a clear picture of "what good looks like" before you start
- You're making small compromises on every output because you're tired

You're in review-first mode when:
- You write down the deliverable before opening a chat
- You review a complete draft in one sitting, not piece by piece
- You can articulate *why* something is wrong, not just that it "feels off"
- You spend more time deciding than producing

## Try This

Pick one task you normally prompt for — something with a clear deliverable, like an email, a summary, or a short report.

1. **Before you open a chat**, write down: the deliverable (what finished product do you want?), two constraints (what must it include or avoid?), and your review criteria (how will you know it's good?)
2. **Write one instruction** that includes all three. Hand it to the AI.
3. **Don't look at the output until it's complete.** No peeking at intermediate steps. No regenerating mid-draft.
4. **Review the complete draft in one pass.** Mark what needs changing. Don't rewrite — annotate.
5. **Ask yourself:** Did this feel different from your normal prompting? Did you spend less total time? Was the result better or worse?

If the result was worse, the problem might be your spec (not clear enough about what "good" looks like) rather than the review-first pattern itself. Tighten the spec. Try again tomorrow.

## The Authorization Gap

There's a policy dimension to this pattern that matters for anyone in an institutional context. When AI agents act without explicit human authorization — sending communications, making decisions, processing cases — the accountability chain breaks. In public institutions, this becomes a democratic accountability problem (Tech Policy Press, June 2026).

The review-first pattern isn't just a productivity technique. It's an accountability technique. Every agent action should have a clear human authorization trail. "Who decided that, and when?" should have an answer. The review point is where that answer lives.

## Verify at the Boundary, Not at the End

Two 2026 studies sharpen the review-first pattern from "review the output" to **"review at the handoffs."**

- **The Hallucination Snowball** (arXiv:2608.14588): sequential multi-agent pipelines that chain specialized agents *without verification at handoffs* have a structural flaw. Errors don't merely persist — they transform: raw numerical facts become derived computations, then narrative prose, then editorially approved conclusions. Detectability degrades near-irreversibly at each step (per-boundary escape probabilities 24.6%, 48.3%, 89.3%). In 346 injected hallucinations across a 4-agent financial pipeline, boundary gates using *identical* RAG verification tools cut hallucination survival from 58.4% to 16.2% versus end-of-pipeline checking (Cohen's h = −0.911, p < 0.000001) — while end-checking alone beat no verification by just 2.3 percentage points. The paper's one-liner is this pattern in its strongest form: **when you verify matters more than whether you verify.** Its allocation rule: verify early (at S1→S2, where 75.4% of hallucinations are still catchable), not late (at S3→S4, where 89.3% have already escaped).
- **When Uncertainty Isn't Enough** (arXiv:2608.14659): uncertainty signals are poor substitutes for verification but good *triggers* for it. Five uncertainty methods across three small code LLMs: multi-sample P(True) correlated strongest with correctness, but uncertainty-based self-correction actually *degraded* Pass@1 in 5 of 6 configurations (−3 to −10pp). Verification-based regeneration — using the signal to decide *when to run a costlier verification loop* rather than to fix output directly — reliably improved Pass@1 (+6 to +26pp on HumanEval, +8 to +20pp on BigCodeBench), scaling inversely with baseline strength. Cheap signals should gate expensive checks, not replace them.

Both studies land on the same design rule: the review point belongs **at each boundary between agents and between agent and human** — not once, at the end. This extends the review-first pattern from a single-draft workflow to the whole pipeline. Your review isn't the last step; it's a repeated switch that fires at every handoff — the same mechanism the [[The Authority Switch|authority switch]] formalizes.

---

### Never Let the Generator Be the Judge (New, August 2026)

**The reviewer must not be the author.** An August 2026 study (arXiv:2608.21850) scored LLM feedback against human teaching-assistant feedback on a five-criteria rubric: students rated the AI's feedback *above* the human TAs — but the same models showed a significant **self-preference bias** when evaluating their own outputs, a bias that persisted even in cross-model evaluation. Generous, fluent self-assessment is exactly what a model produces about its own work: it has no outside view, and its confidence (see [[The Confidence Gap]]) doesn't correct for that.

The pattern extension: Review-First has always meant *review before use*; this study adds the **independence requirement** — the reviewer must be structurally separated from the generator. Concretely: a different model reviewing, a human domain reviewer, or a checklist applied against the source — anything that breaks the loop where the thing that produced the work also certifies it. Verify at the boundary is only verification if the boundary is *outside* the generator.

### The Independent Reviewer: Cross-Vendor Auditing (New, September 2026)

The independence requirement has a mechanical answer now. **CrossAudit** (arXiv:2608.28631) is a protocol for supervising autonomous pipelines, and its first sentence is this page's thesis: *"An AI scientist should not grade its own homework."* The systems the authors examined review their own work with a reviewer from the same model family — or at least the same vendor. Model evaluators favor their own generations, and models trained alike may share blind spots: **the reviewer inherits the author's.** If you're checking the AI's work with the same AI's judgment, you're not checking — you're re-reading.

The protocol's three commitments translate directly to any delegation, not just research pipelines:

1. **Different vendor, human rulebook.** Each increment of work is audited by a reviewer from a *different vendor* against a standard a *human wrote and versioned*. The rulebook lives outside both models — it's the thing neither side gets to edit mid-review.
2. **The audit history is a record, not a log.** Verdicts, disputes, and rulings are committed like git commits — re-readable, citable, learnable-from. "What did we wave through last month?" has an answer you can look up.
3. **A model blocks only by citing a rule.** Advisory judgment never gates the pipeline: no model may wave a deterministic failure, and any blocker must cite the specific rule it's enforcing. Blockers that survive a bounded number of revision rounds go to a person — the human is the tiebreaker, not the first stop.

The trial evidence matters less than the design: two vendors read the same rulebook differently, and neither reading was "better" — the *difference* is the signal. Independence isn't about finding a perfect reviewer. It's about making sure the reviewer's blind spots aren't the author's blind spots.

**Your move:** for anything you run on autopilot, ask the vendor question — *is the thing checking this output from the same family as the thing that made it?* If yes, you don't have a review loop; you have a confirmation loop. Even a human checklist against a written standard beats same-vendor self-review ([[The Rule Capture Problem]] is why the written standard matters).

### The Instrument Effect: What the Audit Finds Depends on the Instrument

The hardest verification lesson of the month comes from a clinical-notes audit (arXiv:2608.31017): three commercial AI scribes, 565 notes, 142 consultations — and **one note in three carried a verified failure** (31.3%), concentrated in allergy/medication information, invented patient identity, and history written up as examination on phone calls. The reassurance — "a clinician signs every note" — turned out to be a formality, not a check.

But the deeper finding is about *your* review practice: **the failure rate depends on the instrument as much as on the thing being audited.** With the same evidence, the review instruction alone moved the share of candidates verified from 9.3% to 79.0%. Change the reviewing model's family and the flagged-note share roughly doubled (54.8% vs. 27.8%). Published audits disagree with each other by margins that instrument differences alone can produce — omission is 54-86% of their errors against 23.1% in this census.

Three moves for the orchestrator:

1. **Treat every audit number as instrument-dependent.** Before you believe "our AI is 95% accurate," ask what instrument produced that number, who refuted it, and with what instructions.
2. **Use adversarial two-reviewer refutation.** The census verified findings by having two models from different families try to *refute* each candidate — the same cross-vendor logic as CrossAudit, applied to a single output. Your cheap version: run a different model (or a skeptical human) against the first draft and instruct it to find reasons it's wrong.
3. **Audit the audit.** The clinicians upheld 32 of 33 findings blind — real checks on real outputs hold up. Formality checks (the signature, the sign-off, the green checkmark) don't. If your review step would pass without reading, it's not a review step.

## Related Pages

[[From Prompt to Pipeline]] · [[From Author to Editor]] · [[Trust Calibration]] · [[Delegation Thinking]] · [[The Authority Switch]] · [[Human in the Loop]] · [[Friction by Design]] · [[The Collapse Pattern]] · [[The Sequencing Principle]] · [[02-Key-Concepts/README|02 — Key Concepts]] · [[The Confidence Gap]] · [[Run-to-Run Variance]] · [[The Rule Capture Problem]] · [[The Failure Review]] · [[The Retrievability Gap]]

## Tags

#concept #workflow #orchestrator
