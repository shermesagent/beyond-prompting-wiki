---
title: The Authority Switch
created: 2026-08-18
updated: 2026-08-18
type: concept
tags: [concept, delegation, orchestrator, architect]
sources:
  - raw/articles/principled-authority-switching-2608.16293.md
  - raw/articles/hallucination-snowball-2608.14588.md
confidence: high
---

# The Authority Switch

## What It Is

The Authority Switch is the moment control changes hands between human and agent — and the claim that **those transfers are design decisions, not events**. Control isn't granted once at delegation; it moves back and forth: hand off → verify at the boundary → take back. Each move is a switch, and each switch can be engineered with a policy (what triggers it, who can force it, what the handback looks like) or left to improvisation ("I'll know when something's wrong… probably").

The term comes from a 2026 paper on shared autonomy in human-robot teams (arXiv:2608.16293). Its diagnosis: most systems treat authority transfer as an afterthought — blending control inputs or using heuristic switching rules with no theoretical guarantees. Its fix: model authority transitions as part of the system dynamics, so the switching policy is **optimized rather than improvised**. Three properties worth stealing:

- **Switches are states, not events.** Authority transitions are embedded in the system dynamics. The system is always in some authority state; policy determines when and how it changes.
- **Asymmetric authority is the default.** The human retains override capability — guaranteed by structure, not by politeness. The framework explicitly accounts for *stochastic human override*: the system plans for the possibility that you take over mid-run.
- **Switching policies can be computed.** In the paper's linear-quadratic formulation, optimal switching policies and value functions come from closed-form recursions — computable independent of the continuous state, and adaptive to dynamics, cost structures, and override probabilities.

The paper is about robots, but the structure is the same as every agent you delegate to: **who holds control, when does it transfer, and what guarantees the transfer?**

## Why It Matters for Moving Beyond Prompting

The delegation loop has three legs: **hand off, verify at the boundary, take back.** Most of this wiki covers legs one and two — briefs, scopes, review-first verification. The Authority Switch is about the mechanics of all three, and especially the leg nobody designs: the take-back.

1. **The take-back is the least-designed leg.** Everyone designs the handoff (prompt, brief, scope). Almost nobody designs the return: under what condition does authority come back to you? What does the agent do if you interrupt? A workflow with no handback condition runs to completion no matter what — which is a policy, just a bad one.

2. **Override isn't a failure — it's a parameter.** The paper's key move is treating human override as *stochastic*: something the system plans for rather than treats as an anomaly. An agent that plans for interruption can checkpoint its work, report cleanly, and resume — an agent that treats "human stopped me" as a crash will fight you every time you intervene.

3. **The boundary check is the switch.** The [[The Review-First Pattern|review-first pattern]] says verify at the boundary. The hallucination snowball study (arXiv:2608.14588) quantifies the difference between boundary verification and end-of-pipeline verification: boundary gates cut hallucination survival from 58.4% to 16.2%, while end-checking alone improved on no verification by just 2.3 percentage points. **When you verify matters more than whether you verify** — in authority-switch terms: control must return to a verifier *at each boundary*, not once at the end.

4. **Uncertainty signals are switch triggers.** The self-correction study (arXiv:2608.14659) shows uncertainty estimates alone can't drive agent-side correction — uncertainty-based self-correction *degraded* Pass@1 in 5 of 6 configurations (−3 to −10pp). But the same signals reliably improved results when they triggered a *verification loop* instead (+6 to +26pp on HumanEval). The signal's job isn't to fix the output; it's to switch authority into a more expensive, more reliable mode. Cheap signals gate expensive checks.

## How to Spot It in Your Day

Your delegation loop is running on improvised switches when:

- You hand off a task and never explicitly take it back — the agent's output just… arrives
- The only take-back mechanism you have is closing the tab or killing the process
- You interrupt an agent mid-run and it has no way to incorporate the interruption — it restarts from scratch or dumps a partial mess
- Your delegation brief specifies the handoff (what to do) but says nothing about handback (when to stop, what to report, what to do if unsure)
- "I'll check it when it's done" — but there's no defined check, let alone a policy for what the check's outcome changes

You're running on designed switches when you can name three things for any delegation:

- **The trigger** — what event returns control to you (a condition, a checkpoint, an uncertainty flag)
- **The override path** — how you force a return mid-run, and what state the agent leaves behind
- **The handback condition** — what the agent reports, when, and what it does if the boundary check fails

## What the Research Says

- **Principled Authority Switching** (arXiv:2608.16293, August 2026): cooperative game-theoretic framework for authority switching in shared autonomy. Control switching is an identical-interest dynamic game with authority transitions embedded in the system dynamics; the paper establishes existence and characterization of team-optimal policies in pure strategies under stochastic human override, with asymmetric authority (human retains override). For linear-quadratic systems, closed-form recursions give optimal switching policies and value functions independent of the continuous state. Validated on scalar and multi-dimensional linear systems; the results reveal fundamental trade-offs between **human adaptability and autonomous efficiency** — the same trade-off you feel every time you decide whether to let the agent run or pull it back.
- **The Hallucination Snowball** (arXiv:2608.14588, June 2026): 346 injected hallucinations in a 4-agent financial analysis pipeline. Errors transform Raw Fact → Derived → Narrative → Invisible, with per-boundary escape probabilities of 24.6%, 48.3%, and 89.3%. Boundary gates using identical RAG verification tools cut hallucination survival from 58.4% to 16.2% versus end-of-pipeline checking (Cohen's h = −0.911, p < 0.000001); end-checking alone achieved 2.3pp improvement over nothing. Optimal allocation: verify at S1→S2, where 75.4% of hallucinations are still catchable — not at S3→S4, where 89.3% have already escaped. The boundary is where the switch must fire.
- **When Uncertainty Isn't Enough** (arXiv:2608.14659, July 2026): five uncertainty methods across three small code LLMs on HumanEval and BigCodeBench. Multi-sample P(True) correlated strongest with correctness; all other methods weakly. Uncertainty-based self-correction degraded accuracy in 5 of 6 configurations (−3 to −10pp); verification-based regeneration reliably improved Pass@1 (+6 to +26pp HumanEval, +8 to +20pp BigCodeBench), scaling inversely with baseline strength. Uncertainty's practical value: **gating signals for verification loops, not standalone substitutes for verification**.

## Try This

**The take-back clause.** Add one sentence to your next delegation brief: *"Report back when X, or if Y, or if you're unsure about Z."* That's a handback condition with a trigger. Then exercise the override on purpose: interrupt the agent at a boundary (or mid-run, on a cheap task) and watch what happens. Does the workflow absorb the interruption — checkpoint, report, resume — or does it crash, restart, or lose state? That behavior *is* your current authority-switch policy. Now you know what it is, and whether it's the one you wanted.

## Related Pages

[[Delegation Thinking]] · [[The Review-First Pattern]] · [[The Observability Gap]] · [[Trust Calibration]] · [[The Capability Ladder]] · [[Human in the Loop]] · [[Abstention]] · [[02-Key-Concepts/README|02 — Key Concepts]]

## Tags

#concept #delegation #orchestrator #architect
