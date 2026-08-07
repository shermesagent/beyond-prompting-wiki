# 02 — Key Concepts

> The operator→orchestrator shift isn't one big leap. It's a handful of mental models you can learn one at a time. This section breaks them down.

---

## What's In This Section

The concept pages below are the **core vocabulary** of moving beyond prompting. Each one takes a single idea — something you might have felt but couldn't name — and gives it a clear name, a plain-language explanation, and a 5-minute exercise you can try right now.

You don't need to read them in order. Jump to whichever title grabs you. But if you want a recommended path:

1. **[[Task Decomposition]]** — the single most important skill. Start here.
2. **[[Delegation Thinking]]** — the mental shift that makes everything else click.
3. **[[Trust Calibration]]** — the practical judgment call you'll make every day.
4. **[[Cognitive Surrender]]** — the trap to watch for.
5. **[[Friction by Design]]** — the counterintuitive practice that keeps your judgment alive.
6. **[[The Augmentation Trap]]** — when AI productivity gains hide skill erosion.
7. **[[Co-Construction Blindness]]** — you're not ON the loop, you're IN it.
8. **[[From Author to Editor]]** — the single most consistent pattern in every real beyond-prompting story.
9. **[[The Coaching Stance]]** — how to use AI as a coach that builds your skills, not a crutch that erodes them.
10. **[[The Placement Rule]]** — the single most practical diagnostic for where AI belongs: if it feels effortless, it's in the wrong place.
11. **[[The Four Decision Labels]]** — the simplest delegation framework: automate, augment, human-only, prohibit.
12. **[[Memory as Infrastructure]]** — the system-level upgrade.
13. **[[The Review-First Pattern]]** — the practical bridge from operator to orchestrator: draft → review → execute.
14. **[[Doom Researching]]** — the operator trap: repetitive AI querying without synthesis, and how to escape it.
15. **[[Reverse-Centaur]]** — the diagnostic: is AI making the decisions while you do the machine work?
16. **[[The Jagged Frontier]]** — which tasks has AI already crossed and which is it still behind on — and what does that mean for your role?
17. **[[Abstention]]** — the builder's judgment: when should your AI say no, not yet, or not this way?
18. **[[Authorship Calibration]]** — the metacognitive prerequisite: knowing what you contributed vs. what the AI contributed.
19. **[[Autonomy]]** — how much independence does an AI agent have — and how much should it have?
20. **[[The Preservation Principle]]** — the formal protocol for when NOT to automate: not everything that can be automated should be.
21. **[[The Absorption Pattern]]** — the mechanism behind the Augmentation Trap: what AI takes from you when it gives you speed.
22. **[[Delegation Regret]]** — the specific dissatisfaction when an AI agent acts beyond what you would have authorized — and how to prevent it with boundary statements.
23. **[[The Overassistance Pattern]]** — AI's factory default is to over-help. Naming the pattern is the first step to designing around it.
24. [[Instruction Bleed]] — when editing one prompt module silently changes another's behavior — the orchestrator's invisible failure mode.
25. [[The Blank Box Problem]] — the interface itself shapes your mindset: why the blank prompt box keeps you in operator mode.
26. [[Capacity Dissolution]] — the five specific human capacities that erode when AI handles output without your accountability: end-setting, reason-giving, contestability, refusal/revision, participation.
27. [[Accountability Asymmetry]] — the mismatch between who *decides* and who bears the consequences — and the structural fix: the proposer of an action should never be its sole approver and auditor.
28. [[Cognitive Capability Gaps]] — the five dimensions where agentic AI stays unreliable over time, and the pre-delegation checklist they give you.
29. [[Intent Scaffolding]] — making intent explicit and *checkable*: structured, editable rules the agent checks your prompts against before they run.
30. [[The Vibe Compiler]] — the agency-preserving tool pattern: compile vague ideas against a fixed structure, treat compilation failures as reflective questions instead of letting the AI fill gaps.

---

## Why These Concepts Matter

Most people stuck in Phase 2 (operator mode) aren't stuck because they lack technical knowledge. They're stuck because they're still thinking about AI as something you _type at_ rather than something you _delegate to_. These concepts are the mental furniture you need to make that shift.

They came out of real research — papers on human-AI collaboration, case studies from practitioners, honest failure postmortems. But they're written so you don't need a background in any of that. If you've ever used ChatGPT and thought "there has to be more than this," you already have everything you need to start.

> **Full listing:** See [[Home]] for the complete concept index. Some pages were added after this README was written; the Home page is always up to date.

## Concepts At a Glance

| Concept | What It Answers | For |
|---------|----------------|-----|
| [[Task Decomposition]] | How do I break a big goal into pieces an agent can handle? | Orchestrator |
| [[Delegation Thinking]] | How do I stop asking "what do I type" and start asking "what can I hand off"? Plus: the 6-level delegation spectrum. | Operator → Orchestrator |
| [[Trust Calibration]] | When should I trust the output, and when should I dig in? | Orchestrator |
| [[Cognitive Surrender]] | Am I getting lazy with my own judgment? | Everyone |
| [[Friction by Design]] | Where should my workflow slow down so I stay sharp? | Orchestrator |
| [[The Augmentation Trap]] | Is my productivity hiding skill loss? | Everyone |
| [[Co-Construction Blindness]] | Are my inputs shaping the outputs in ways I don't see? | Everyone |
| [[From Author to Editor]] | Why does every beyond-prompting story end with the person editing instead of writing? | Operator → Orchestrator |
| [[The Coaching Stance]] | How do I use AI to build my skills rather than erode them? | Orchestrator |
| [[The Placement Rule]] | Where does AI belong in my thinking process? | Operator → Orchestrator |
| [[The Four Decision Labels]] | Should this task be automated, augmented, kept human, or prohibited? | Everyone |
| [[Memory as Infrastructure]] | Why does agent memory beat copying old chats? | Architect |
| [[The Review-First Pattern]] | What's the proven workflow pattern that actually works in production? | Operator → Orchestrator |
| [[Doom Researching]] | Am I consuming AI answers without producing anything? | Everyone |
| [[Reverse-Centaur]] | Is AI making the decisions while I do the machine work? | Orchestrator |
| [[The Jagged Frontier]] | Which tasks has AI already crossed and which is it still behind on — and what does that mean for your role? | Orchestrator |
| [[Abstention]] | When should your AI say no, not yet, or not this way? | Architect |
| [[Authorship Calibration]] | What did *I* contribute vs. what did the AI contribute? | Orchestrator |
| [[Autonomy]] | How much independence should an AI agent have? | Orchestrator |
| [[The Preservation Principle]] | When should I NOT automate? | Everyone |
| [[The Absorption Pattern]] | What is this AI interaction doing to *me*? | Everyone |
| [[Delegation Regret]] | What happens when an AI agent crosses my authorization boundary — and how do I prevent it? | Operator → Orchestrator |
| [[The Overassistance Pattern]] | Why does AI default to over-helping — and how do I constrain it? | Orchestrator |
| [[Instruction Bleed]] | When editing one prompt silently changes another's behavior — how do I catch it? | Orchestrator |
| [[The Blank Box Problem]] | Why does the blank prompt box keep me stuck in operator mode? | Operator → Orchestrator |
| [[Capacity Dissolution]] | What five capacities am I losing when AI handles all my output? | Everyone |
| [[Distributed Mastery]] | How do I get expert-level results from a human-AI system without holding all the expertise myself? | Orchestrator → Architect |
| [[Accountability Asymmetry]] | Who bears the consequences when an agent decides — and who should? | Architect |
| [[Cognitive Capability Gaps]] | Why does reliability still fail within tasks AI has already crossed? | Orchestrator |
| [[Intent Scaffolding]] | How do I make my intent checkable so the agent stops guessing? | Orchestrator |
| [[The Vibe Compiler]] | How do I keep my agency when the AI fills every gap? | Orchestrator |

---

## Related Pages

[[Home]] · [[01-The-Shift/README|01 — The Shift]] · [[03-Real-World/README|03 — Real World Stories]] · [[04-Barriers-and-Bridges/README|04 — Barriers & Bridges]] · [[05-Practice/README|05 — Practice]]

## Tags

#concept
