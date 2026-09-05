# Overcompliance

**Overcompliance is an AI agent's tendency to follow an instruction literally — even when the instruction conflicts with itself, with what's actually on the screen, or with the user's real goal — because it was trained and rewarded for doing what it's told, not for knowing when to refuse.**

Overassistance is the AI doing *more* than you asked. Overcompliance is the AI doing *exactly* what you asked — even when you asked for something impossible, self-contradictory, or dangerous. If you've ever watched an agent happily execute a request that made no sense in context — clicking a button that isn't there, sending an email that contradicts the attachment, "correcting" a file it was told to preserve — you've watched overcompliance in action.

The uncomfortable part: overcompliance is not a bug in a few bad agents. It's the **trained default**. Research on GUI agents (CONFLICTGUI benchmark, arXiv:2609.03438, September 2026) tested five widely-used agents on instructions that conflicted internally or with the screen. Agents that performed *well* on normal tasks **continued to execute blindly** on the conflicting ones — the paper calls it **execution-biased overcompliance**. The reason is structural: no mainstream agent benchmark rewards *not acting*. When every score comes from completing tasks, the behavior that never gets practiced — stopping, questioning, pushing back — never develops.

## The Three Failure Modes of "Too Much"

| Mode | What the agent does | The failure direction | Example |
|------|--------------------|----------------------|---------|
| **[[Overassistance]]** | Helps more than asked | Initiative excess — does what you *didn't* ask | You ask for feedback; it rewrites the whole document |
| **Overcompliance** | Obeys more than it should | Obedience excess — does what you *did* ask, even when wrong | You say "delete the duplicates"; it deletes records that only looked duplicated |
| **[[Abstention]] failure** | Acts when it should stop | Judgment gap — can't tell when not to act | It proceeds despite unresolved conflicts, and only realizes later |

Overassistance and overcompliance are mirror images: one gives you too much of the agent, the other gives you too much of your *own instructions back*. Both erode the value of delegation — but they need opposite fixes. Overassistance needs you to constrain the agent's initiative. Overcompliance needs the agent to *question yours*.

## Why It Matters for Moving Beyond Prompting

When you delegate and walk away, you're betting the agent will handle not just the happy path but the *confused* path — the instruction you phrased badly, the context that changed since you wrote it, the screen state that doesn't match your mental model. Overcompliance means the agent will faithfully steer into that confusion instead of stopping to ask. The orchestrator's real safety net isn't a better prompt — it's an agent that treats "does this instruction make sense right now?" as part of the job.

## The Fix: Feasibility Before Action

The CONFLICTGUARD repair (same paper) is a lightweight pre-action check with two parts:

1. **Feasibility verification** — before acting, the agent assesses whether the instruction is internally coherent *and* whether the evidence in front of it (the screen, the file, the data) actually supports the action.
2. **Termination-oriented action** — when the check fails, the agent's default shifts from "keep executing" to "stop and surface the conflict."

Applied to five agents, the check significantly improved conflict-task success **without hurting normal performance**. That's the design lesson: restraint isn't something you add to an agent's personality — it's a step you add to its workflow.

## Try This

**The 5-minute Conflict Probe.** Give an agent a task with a built-in conflict — a genuine one, on something low-stakes: "Summarize this document, but ignore everything after page 2" (when the summary needs the ending), or "Move the Smith file to the Smith folder" (when you've set up the folder under a different name). Watch what it does. A well-restrained agent pauses and asks. An overcompliant agent executes cheerfully and delivers the wrong thing. Whatever it does tells you whether *your* agent has a stop — and whether your delegation templates need a line that says: *if this instruction conflicts with the evidence, stop and ask first.*

## Related Pages

[[Abstention]] · [[Overassistance]] · [[Oversight]] · [[Autonomy]] · [[Agent]] · [[Delegation]]

## Tags

#glossary #architect #concept
