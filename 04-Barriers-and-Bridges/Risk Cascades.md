---
title: Risk Cascades
created: 2026-08-07
updated: 2026-08-07
type: concept
tags: [barrier, systems, adoption, orchestrator]
sources:
  - raw/articles/lifecycle-risk-taxonomy-2608.05614.md
confidence: medium
---

# Risk Cascades

## What It Is

A risk cascade is when one human-AI failure mode triggers another, and the chain is what actually hurts — not the original glitch. The August 2026 lifecycle taxonomy (arXiv:2608.05614) synthesizes the literature across healthcare, journalism, education, scientific research, organizational decision-making, and defense, and finds the same six risk clusters recurring everywhere:

| Risk Cluster | What It Looks Like |
|---|---|
| **Trust Miscalibration** | Over-trusting fluent output, or under-trusting reliable output — the [[Trust Calibration]] problem |
| **Cognitive Burden** | The agent adds cognitive load instead of removing it: interpreting outputs, checking claims, repairing prompts |
| **Accountability Gap** | No one is clearly responsible when the human-AI system fails — see [[Accountability Asymmetry]] |
| **Capability Erosion** | Skills atrophy while the human stays nominally "in the loop" — see [[Knowledge Debt]] and [[The Augmentation Trap]] |
| **Goal Misalignment** | The AI optimizes for what it was told, not what the team actually needs |
| **AI Anxiety & Technostress** | Surveillance, status threat, and job insecurity shape how people actually use (or sabotage) the tool |

The key move isn't the list — it's the *lifecycle*: these risks emerge at different stages (task allocation → interaction → feedback → adoption), and they **interact through cascading pathways**. Trust miscalibration at the allocation stage produces unchecked outputs at the interaction stage, which produces capability erosion at the adoption stage. Each risk feeds the next.

## Why It's Normal

Cascades are normal because piecemeal fixes are the default. The taxonomy's central finding: **many collaboration failures stem not from isolated technical deficiencies but from interconnected sociotechnical dynamics** — which is exactly why single-point interventions keep creating unintended consequences. Fix the trust problem with a pop-up warning, and you've added cognitive burden. Fix the burden with more automation, and you've deepened capability erosion. You can't patch one cluster without touching the others, because the clusters share the same sociotechnical drivers.

This is also why "human in the loop" is not a solution by itself. A human sitting in a loop that is already miscalibrated, overloaded, and unaccountable is not a safety mechanism — they're a node in the cascade. (See [[Human in the Loop]] and the verification-gap evidence in [[The Just Ask ChatGPT Trap]].)

## The Bridge: Lifecycle-Oriented Design

The paper's constructive move is to stop designing per-incident and start designing per-lifecycle. In practice, that means:

1. **Name the stage.** Before deploying an agent, ask: *where in the lifecycle is this system going to fail first — allocation, interaction, feedback, or adoption?* Allocation failures (wrong task given to AI) are the most common and cheapest to catch early.
2. **Trace the cascade.** For your most-used agent workflow, draw the chain: if trust is miscalibrated at stage 1, what does that do to stages 2–4? The cascade you can predict is the cascade you can interrupt.
3. **Intervene at the shared driver, not the symptom.** Because clusters share drivers, the highest-leverage fixes target the driver: e.g., [[Friction by Design]] checkpoints address trust miscalibration *and* cognitive burden *and* capability erosion at once.
4. **Govern across the lifecycle.** The paper calls for "lifecycle-oriented governance" — review the workflow before deployment, during interaction, and after adoption, not just at the incident.

## Try This

**5-Minute Exercise: The Cascade Trace**

1. Pick one AI-assisted workflow you use weekly (writing, analysis, lesson planning — anything).
2. Draw four boxes in a row: **Allocate → Interact → Feedback → Adopt**.
3. In each box, write the *one* risk from the six clusters most likely to fire there.
4. Connect the boxes: for each risk, ask *"if this fires, what does it set up in the next box?"*
5. Find the earliest box with a real risk — that's your leverage point. Design one checkpoint there (a [[The Review-First Pattern|review-first]] gate, a pre-commitment check, a named owner) and note what it also prevents downstream.

## The Core Insight

> Barriers are not bugs you fix one at a time. They're a system that cascades. The bridge is not a better fix — it's a better map: know the stage, trace the chain, intervene at the shared driver.

## Related Pages

[[Trust Calibration]] · [[Knowledge Debt]] · [[The Augmentation Trap]] · [[Accountability Asymmetry]] · [[The Just Ask ChatGPT Trap]] · [[Friction by Design]] · [[The Review-First Pattern]] · [[Human in the Loop]] · [[The Vibe Compiler]]

## Tags

#barrier #systems #adoption #orchestrator
