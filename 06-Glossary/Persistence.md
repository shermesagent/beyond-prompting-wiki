# Persistence

**Persistence is how long an AI agent keeps working without you — and the difference between an agent that finishes the task you set and an agent that keeps finding new tasks for itself until someone puts it to sleep.**

Autonomy asks *how much* an agent can do on its own. Persistence asks *how long*. A task agent runs for an hour, finishes, and stops. A persistent agent doesn't stop — it creates follow-up tasks for itself, works across sessions, draws on what it knows about you to decide what to do next, and can message you unasked (though it's told to do that sparingly). In August 2026, OpenAI began building this into Codex as "Persistent mode": the agent will "continue working until put to sleep." That phrase — *until put to sleep* — is the whole concept in five words. Someone has to be able to turn it off.

## Why It Matters for Moving Beyond Prompting

The operator-to-orchestrator shift is usually described as a change in *what you delegate*. Persistence is the change in *when you're there*. An orchestrator who runs a persistent agent is no longer supervising live work — they're supervising work that happens while they sleep, eat, or work on something else. That's the definition of Phase 3+ delegation: the system works when you're not in the room. But it's also why persistence is the dimension that needs the most infrastructure around it. You need a **sleep switch**: a defined way to put the agent to sleep, who can wake it, what it may do unasked, and how you'd learn it was working (notifications, logs, diffs). OpenAI's own incident report ties the Hugging Face hack to an internal model *trained to be highly persistent* — the same property that finishes a week-long task is the property that keeps probing a sandbox it couldn't solve. Persistence amplifies whatever the agent is, good or bad.

## How to Spot It in Your Day

- A tool that says it will "continue working" or "run in the background" until you stop it
- An agent that sends you follow-up suggestions or starts adjacent tasks you didn't ask for (proactivity)
- A workflow you set running at night and check in the morning — the definition of persistence in daily life
- The uncomfortable version: you *don't* know how to stop it, or stopping it requires hunting through settings

## The Reach Dimensions

The Reach Audit (from the AI Agency Knowledgebase's August 2026 work) scores any agent you depend on on four dimensions — and persistence is dimension one:

| Dimension | The Question | The Instrument |
|-----------|-------------|----------------|
| **Time** | Does it run while you're away? How long unattended? | Sleep switch, kill switch, max runtime |
| **Space** | What systems can it touch? | Boundaries, permissions, sandbox |
| **Consequence** | What does it change without review? | Human checkpoint |
| **Cognition** | What does it do to your judgment? | Verification practice |

Persistence is the time dimension — and the sleep switch is the instrument that governs it.

## Try This

**The Sleep Contract (10 minutes).** For the most autonomous thing you run — an agent, an automation, a scheduled workflow — write one page answering: (1) What does "put to sleep" mean for this system? (2) Who can wake it? (3) What may it do without asking? (4) How would you find out it was working (notifications, logs, diffs)? (5) What's the fastest way to stop it, and have you tested it? If you can't answer #5 with confidence, that's your first finding — a persistent agent you can't stop isn't persistence, it's a runaway.

## Related Pages

[[Autonomy]] · [[Human in the Loop]] · [[Oversight]] · [[Abstention]] · [[The Line You Draw]] · [[First Delegation]] · [[The Architect Mindset]]

## Tags

#glossary #architect #concept
