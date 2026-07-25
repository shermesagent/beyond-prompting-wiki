# Trust Calibration

**Trust calibration is the skill of knowing — specifically, not vaguely — when to trust an AI agent's output and when to verify. It's not a yes/no switch; it's a sliding scale you adjust based on the task, the stakes, and the agent's track record.**

If you've ever used an AI tool and felt torn between "wow, this is amazing!" and "wait, can I actually trust this?", you've experienced poor trust calibration. The two extremes — blind trust and blanket skepticism — are both wrong, and they both cost you. Blind trust leads to [[Cognitive Surrender]]: you stop thinking critically and just accept whatever the AI produces. Blanket skepticism defeats the point of delegation: you second-guess everything, which takes as much effort as doing it yourself.

Good trust calibration lives between those poles. It's the ability to say: "For this specific task — writing a meeting summary from a transcript — the AI is reliable about 90% of the time, and the 10% it gets wrong are usually names and dates. So I'll trust the structure and flow, spot-check the names, and verify any date that matters." That's not a prompt. That's judgment.

## Why It Matters for Moving Beyond Prompting

Operators have a crude relationship with AI trust: trust everything or trust nothing. Neither works at orchestrator scale.

When you're delegating multiple tasks across multiple agents, you need **granular trust** — trust that lives at the level of specific task types, not at the level of "the AI" as a whole. You learn that one agent is reliable at data extraction but mediocre at analysis. Another agent writes beautifully but hallucinates statistics. A third is great at structure but needs human polish for tone.

The orchestrator doesn't think in terms of "do I trust AI?" They think in terms of: "For this task type, with this model, under these conditions, where do I put my verification attention?" That's trust calibration — and it's a learnable skill, not a personality trait.

The research backs this up. A 2026 ACM study found that AI systems can be highly accurate yet provoke low user confidence because they don't communicate their uncertainty well. Users trust more when the AI says "I'm 85% sure about this" than when it says "Here's the answer" — even when the answer is identical. The transparency itself builds trust, even when the revealed confidence is lower than expected. That's a counterintuitive finding with huge practical implications: **showing weakness builds trust.**

## Growing Your Calibration

Trust calibration isn't something you have or don't have. It's something you build, task by task, by paying attention to when the AI surprises you. Surprise is the calibration signal.

When the AI does something better than you expected: your trust was too low. When the AI does something worse than you expected: your trust was too high. Each surprise is data — it tells you where your mental model of the AI's capabilities is wrong. Over time, those corrections accumulate into accurate calibration.

A practical pattern: keep a running "trust journal" for a week. Every time you use AI for something consequential, note what surprised you. After a week, you'll have a map of where your calibration is sharp and where it's off. Most people discover that they over-trust AI on factual recall (names, dates, statistics) and under-trust it on creative synthesis and structure — the exact opposite of where AI is actually strongest. That single correction transforms how they delegate.

## Related Pages

[[Agent]] · [[Delegation]] · [[Oversight]] · [[Autonomy]] · [[Cognitive Surrender]] · [[Co-Construction Blindness]] · [[Delegation Regret]]

## Tags

#glossary #orchestrator #concept
