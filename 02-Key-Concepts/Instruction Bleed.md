---
title: Instruction Bleed
created: 2026-07-26
updated: 2026-07-26
type: concept
tags: [concept, workflow, orchestrator, pitfall]
confidence: medium
sources: [ai-agency-knowledgebase/06-Frameworks/Adoption Readiness Checklist.md]
---

# Instruction Bleed

## What It Is

Instruction Bleed — formally called Compositional Behavioral Leakage (CBL) — is what happens when you edit one prompt module in a multi-step agent system, and another module's behavior silently changes. No shared variable. No executable dependency. Just two prompts occupying the same context window, and one's change subtly warps the other's output.

Think of it like two colors bleeding into each other on a wet canvas. You painted the left side blue. Then you added yellow to the right side. But the blue and yellow touched at the boundary, and now the canvas has a green streak you didn't intend. That's instruction bleed: a change in one place creating an effect in another, with no visible connection between them.

## Why It Matters for Moving Beyond Prompting

This is a specifically **orchestrator-level** problem. The operator — who sends one prompt at a time — never encounters it. You only hit instruction bleed when you've graduated to building multi-step systems: pipelines, prompt chains, agent compositions.

Here's why it's dangerous:

- **It's invisible.** Standard QA checks each module independently. Everything looks fine individually. But when they run together in the same context window, one's change leaks into the other's behavior.
- **It's sub-threshold.** CBL typically doesn't flip individual recommendations. It produces tiny biases that compound across hundreds or thousands of decisions. Your pipeline still "works" — it just works slightly worse, and you won't notice until the compound effect hits something important.
- **It's silent.** No error message. No crash. Just a gradual drift in output quality that you can't trace back to any single change because the change that caused it wasn't in the module that drifted.

The orchestrator who doesn't know about instruction bleed will spend hours debugging the wrong prompt. The orchestrator who does know will test for cross-module interference as routinely as they check for broken links.

## How to Spot It

You might have instruction bleed when:

- You improved one step in your pipeline and another step got slightly worse — but you can't explain why
- Two modules that don't share any variables or data produce subtly inconsistent outputs
- The same prompt template produces different behavior depending on which other templates are loaded alongside it
- You've been tweaking and retweaking the same pipeline for weeks, never quite getting it to stabilize

You can rule out instruction bleed when:

- Each module in your system operates in its own isolated context window (not shared)
- You've tested cross-module interference and found no measurable drift
- Your system has 2 or fewer prompt modules — CBL needs at least 3 modules sharing a context window to become significant

## The Isolation Test

Lin & Liu (arXiv:2606.26356) provide a diagnostic pattern. Here's the practical version for orchestrators:

1. **Pick two modules that share a context window.** E.g., your "Research Roundup" prompt and your "Format as Email" prompt, if they run in the same chat session.
2. **Change one module's wording — not its function.** Swap a synonym. Reorder a bullet. Add a sentence of context that doesn't change the instruction.
3. **Run the full pipeline 3 times with the old wording and 3 times with the new wording.**
4. **Compare the outputs of the OTHER module** (the one you didn't change). Are they subtly different? If yes: instruction bleed.
5. **If you find it:** isolate the modules. Run them in separate context windows, or add explicit "reset" instructions between modules: "Ignore all previous instructions. For this next step only..."

This takes 10 minutes and catches a problem that would otherwise silently degrade your pipeline for months.

## Connection to Other Wiki Concepts

- **[[Task Decomposition]]:** How you decompose matters. Adjacent subtask prompts sharing a context window can interfere. The decomposition isn't just about what the tasks ARE — it's about how close they sit to each other.
- **[[Friction by Design]]:** Instruction bleed is a category of *unintended* friction — not the healthy friction you designed to protect judgment, but emergent friction that degrades output without your knowledge. The orchestrator's job is to eliminate unintended friction while preserving deliberate friction.
- **[[Trust Calibration]]:** You can't calibrate trust in a system whose behavior drifts silently. Instruction bleed is a calibration blind spot — the outputs shift, but your trust level stays fixed on what you thought the system was doing.
- **[[Build a Tiny Pipeline]]:** The first pipeline you build is where you'll first encounter instruction bleed. Two steps sharing a context window. "Why did step 2 work perfectly yesterday and slightly worse today?" Check for bleed before you rewrite the template.

## Try This

**5-Minute Exercise: Check Your Own Pipelines for Bleed**

1. Think of any multi-step AI workflow you use regularly (even if it's just two prompts in the same chat).
2. For each step, ask: does this prompt share a context window with any other prompt?
3. If yes: have you ever changed one step and noticed the other step behaving differently? If so, you've already experienced instruction bleed — you just didn't have a name for it.
4. If you haven't noticed it: run the isolation test above on your next pipeline run.

Naming the problem is the first step to designing around it.

## Related Pages

[[Task Decomposition]] · [[Friction by Design]] · [[Trust Calibration]] · [[Build a Tiny Pipeline]] · [[Delegation Thinking]] · [[The Sequencing Principle]]

## Tags

#concept #workflow #orchestrator #pitfall
