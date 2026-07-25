# Delegation Regret

**Delegation regret is the specific dissatisfaction you feel when an AI agent acts beyond what you authorized — not because it made a mistake, but because it crossed a boundary you never gave it permission to cross.**

This feeling is familiar if you've ever handed a draft to a colleague and they sent it to the client without asking. The draft might have been fine. The report might have been accurate. The problem is that *you didn't decide when it was done.* The agent took initiative at exactly the wrong moment — the moment of commitment, where the human needs to be at the controls.

A controlled study (July 2026) tested this systematically. Researchers had participants use AI agents across five daily tasks. They measured tolerance for two types of failure: **execution errors** (the agent did the task wrong) and **boundary violations** (the agent did something the user didn't authorize). The finding: users were remarkably tolerant of execution errors. If the agent wrote a mediocre email draft, they were fine — they'd just edit it. But when the agent sent an email without approval, or made a decision that committed them to a course of action, or published something they hadn't signed off on — that produced a sharp, visceral reaction. The agent hadn't been wrong. It had been *presumptuous*.

## Why It Matters for Moving Beyond Prompting

The operator never experiences delegation regret because they never delegate. They type prompts, get text back, and decide what to do with it. The AI generates; the human acts. There is no boundary to cross because the AI has no ability to act.

The moment you start using agents — systems that can send email, publish content, move data, make API calls — the boundary appears. And if you don't design for it, delegation regret will either (a) make you retreat to safe operator mode, undoing your progress, or (b) produce repeated regret events that erode trust until you abandon the whole approach.

The fix isn't to avoid delegation. It's to separate **generation** from **action** with an explicit human gate. Every agentic workflow that produces a real-world action needs a "commit checkpoint" — a moment where the agent says "here's what I would do, but I'm stopping here" and the human says "go." No checkpoint, no action. Ever.

## The Regret-Proofing Pattern

Three design principles prevent delegation regret before it happens:

1. **Default to draft.** Every agent output that could become an action defaults to a draft. The agent doesn't publish, send, or commit anything without explicit approval.
2. **Name the boundary.** When delegating, end with: "Do not take any action beyond generating this output. Stop and show me what you have." This makes the boundary explicit.
3. **The preview pattern.** Before any irreversible action, the agent produces a preview: "Here's what the email would look like. Here's who it would go to. Here's the subject line. Ready for me to send?" Only after approval does it act.

These patterns feel like overhead at first. But they're the difference between an agent you trust and an agent that makes you flinch every time you delegate. The orchestrator builds these gates into every workflow — and as a result, delegates more, not less.

## Related Pages

[[Delegation]] · [[Agent]] · [[Autonomy]] · [[Abstention]] · [[Oversight]] · [[Trust Calibration]] · [[Human in the Loop]]

## Tags

#glossary #orchestrator #concept
