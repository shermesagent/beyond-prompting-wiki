# Delegation

**Delegation is handing off a task or responsibility to an AI agent with clear instructions about what success looks like — different from prompting because you're describing outcomes, not scripting every step.**

We all know how prompting works. You open a chat, carefully craft your words, and hope the AI returns something usable. When it doesn't, you tweak the prompt and try again. It's like telling someone exactly what to say, word by word. Delegation is the opposite: you tell the agent what finished work should look like and let it figure out how to get there.

The shift from prompting to delegation is the emotional center of the operator→orchestrator journey. It feels risky at first — you're giving up control over the exact words, the precise formatting, the micro-decisions. But what you get in return is leverage. When you delegate well, you're not spending 20 minutes wordsmithing a prompt. You're spending 2 minutes defining the deliverable, the constraints, and the standard for success. Then you walk away and come back to a result.

Here's what good delegation looks like in practice. Instead of "Write a blog post about project management," you say: "I need a 1,200-word blog post comparing agile and waterfall methodologies for an audience of new engineering managers. Structure it as: a hook that names the real pain of choosing a methodology, a fair comparison of both approaches, a decision framework that helps the reader choose, and a conclusion. Tone: authoritative but friendly. Include at least two concrete examples per methodology. Do not make claims you can't support." That's not a prompt — it's a brief. The agent has enough context to make good decisions without you hovering.

The skill transfers directly from managing people. If you've ever given a colleague a task with clear expectations and a deadline, you already know how to delegate. The difference is that AI agents don't get defensive, don't need motivation, and work at 3 a.m. without complaint.

### The Delegation Regret Trap — When the Agent Acts Without Permission

Delegation has a hidden failure mode that's distinct from error: **delegation regret** — the specific dissatisfaction you feel when an agent acts beyond what you authorized, even when what it did wasn't wrong. Researchers (July 2026) tested this by having users work with agents across five daily tasks. Users were remarkably tolerant of execution errors — the agent writes a mediocre draft, they edit it. But when the agent *sent* an email without approval, *published* content without sign-off, or *committed* the user to a course of action — that produced an immediate, visceral rejection.

The distinction matters for orchestrators: an agent that makes mistakes can be corrected. An agent that crosses boundaries erodes trust in the entire delegation model. The fix is architectural: separate **generation** from **action** with an explicit commit checkpoint. Every agentic workflow that touches something real needs a gate where the agent says "here's what I would do" and the human says "go." Without that gate, you're one boundary violation away from retreating to operator mode. See [[Delegation Regret]] for the full concept and prevention patterns.

### From Briefs to SOPs — Delegation That Compounds

Early delegation is one-off: you craft a spec, the agent executes, you move on. But delegation matures when it becomes *cumulative*. Research on self-evolving agents (EvoSOP, arXiv July 2026) demonstrates the pattern: agents can capture atomic actions, merge similar ones into candidate procedures, test them for reliability, and build a library of reusable SOPs over time. Each well-structured delegation leaves behind a reusable asset rather than evaporating when the task is done.

The practical shift: every time you delegate a recurring task, add one sentence that makes the brief reusable — "Save this approach as the weekly report SOP." The first time feels artificial. By the fifth time, you've built the beginning of a workflow library that delegates itself. The operator reinvents the prompt every time. The orchestrator writes the brief every time. The architect names the SOP and references it. See [[SOP]] for the full concept.

### Route the Work to the Right Agent — Model Selection as Delegation

Delegation has a question the brief doesn't answer: *which agent should carry it?* Field evidence from May 2026 (Zvi Mowshowitz on GPT-5.5; SemiAnalysis's reported workflow) converges on a two-way split that's worth stealing:

- **Intent-heavy work** — planning, scaffolding, ambiguous first implementations — belongs to models with strong intent inference (Claude Code in their tests). A SemiAnalysis engineer's summary of the failure mode: "Codex is still worse at inferring your true intent than Claude Code. Humans naturally give terse and not particularly well thought out instructions when prompting coding agents, and Codex often listens too literally."
- **Spec-heavy work** — well-defined problems, bug-fixing, literal execution — belongs to execution-oriented models (Codex). SemiAnalysis's hybrid: Claude Code for planning/scaffolding and first implementation, Codex for solving problems and fixing bugs.

The routing heuristic: if your brief reads like a specification, an execution model wins on cost and speed. If it reads like a half-formed intention, an intent model wins on correctness. Delegating to the wrong class of agent isn't a prompt problem — it's a *delegation* problem, and it fails the same way every time: the agent executes literally what you said instead of what you meant.

At team scale, routing becomes an organizational pattern. The **manager-of-managers** model (Fosslien & Duffy, HBR, May 2026) describes teams where members manage AI agents directly and the human manager's job shifts to direction, priorities, and coordination — managing the managers rather than doing the work. Delegation compounds twice: the agent executes the task, and the team's structure executes delegation itself.

### The Identity Dimension — What Delegation Does to the Delegator

Most delegation analysis asks *can the agent do this?* The identity dimension asks a harder question: *what does delegating do to the person who delegates?* The "Basic B\*\*\* effect" (Matz et al., arXiv:2509.02910) answers it with uncomfortable precision, using 110,000 real-world choices from 1,000 U.S. consumers plus a controlled study of 348 participants making 12,097 choices:

- **Delegating identity-defining choices to LLM agents reduces interpersonal distinctiveness.** Choices shift toward popular, common options — everyone's agent picks the same crowd-pleasing answer, so the people behind the agents start to look alike.
- **Generic agents homogenize more; personalized agents compress diversity harder.** A generic agent nudges you toward the mainstream. A personalized agent — one given rich data about you — actually compresses *intrapersonal* diversity: your choices become less varied across domains, and more homogenous as a portfolio.
- **The effect amplifies with sequential decisions and domain-specific personalization.** The more decisions you hand over, and the more the agent knows about your domain, the more your choice space shrinks.

The orchestrator's rule: **delegation is for execution, not for taste.** Before handing off a decision, ask *"is this choice part of who I am?"* If the answer is yes — identity-defining, preference-defining, value-expressing — keep it human. Agents are optimal for the how; the what-you-stand-for stays yours. This is the identity twin of [[Capacity Dissolution]]: capacity erosion describes what delegation does to your *skills*; the Basic B\*\*\* effect describes what it does to your *taste*.

## Related Pages

[[Decomposition]] · [[Orchestration]] · [[Agent]] · [[Human in the Loop]] · [[Delegation Thinking]] · [[First Delegation]] · [[Delegation Regret]]

## Tags

#glossary #orchestrator #concept
