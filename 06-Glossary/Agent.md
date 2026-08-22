# Agent

**An AI agent is a system that can perceive, decide, and act on its own to accomplish a goal — unlike a chatbot, which waits for every prompt, an agent works toward objectives.**

If you've ever used ChatGPT, you know the rhythm: you type, it responds, you type again. Every move is yours. The AI doesn't take a step without you pushing it. That's a chatbot — reactive, one-shot, waiting for your next instruction.

An agent breaks that rhythm. You give it a goal — "research the top three project management tools and put together a comparison table" — and it figures out the steps. It might search the web, read documentation pages, pull features into a spreadsheet-like format, and hand you a finished deliverable. You're not prompting each sub-step; the agent is reasoning about what needs to happen and doing it. This is the difference between operating a tool and directing a teammate.

For the operator→orchestrator journey, understanding agents is step one. When someone says "AI agent," they're describing a system with three capabilities: perception (taking in information), decision-making (choosing what to do next), and action (actually doing it — running searches, writing code, calling APIs). You don't need to build agents yourself to benefit from understanding them. But once you know what an agent is, you start seeing your own work differently. You stop asking "what prompt would solve this?" and start asking "what agent could handle this for me?"

A real-world example: instead of spending an afternoon manually compiling a weekly status report from Slack, email, and your project tracker, you delegate it to an agent that gathers the inputs, synthesizes them, and delivers a draft to your inbox. You review and send. That's the orchestrator pattern — and it starts with knowing what an agent can do.

### The Five Types of Human-AI Teams

"Working with an AI agent" sounds like one thing, but research analyzing 53 papers on human-AI teams (Hughes & Habli, 2026) found it actually describes five very different relationships:

| Team Type | What It Looks Like | You're the... | Beyond Prompting Phase |
|-----------|-------------------|---------------|------------------------|
| **AI Assistant** | You ask, it responds. One human, one AI. Every move is yours. | Operator | Phase 1-2 |
| **Ad-hoc Dependency** | The AI handles a step in your workflow when you remember to use it. You're still driving. | Operator → Orchestrator | Phase 2 |
| **Ad-hoc Forced Dependency** | The AI is the bottleneck — you have to work through it, but control is awkward. | Frustrated Operator | Phase 2 |
| **Paired Equanimity** | You and the agent work as equal partners. Mutual back-and-forth. Shared task ownership. | Orchestrator | Phase 3 |
| **Group Equanimity** | Multiple humans and multiple agents work together as one team. Defined roles, handoffs, memory. | Architect | Phase 3+ |

Most people using ChatGPT are in AI Assistant mode. The beyond-prompting shift is specifically about moving toward Paired Equanimity — where the agent isn't a tool you pick up, but a collaborator you work alongside. That's a different relationship, and it requires different skills: delegation, oversight, trust calibration, and the ability to name what kind of team you're building.

### What Your Teaching Style Reveals — The Three Framings

How you *teach* AI to someone else reflects how you *think* about AI yourself. A study of YouTube educators (arXiv, July 2026) identified three dominant framings used to teach ChatGPT: **Conceptual Scaffold** (AI as a thinking partner that explores ideas with you), **Retrieval Practice** (AI as a quiz-generator and self-testing tool), and **Output Generation** (AI as a drafting machine that produces finished content). Output Generation — the "just ask it to write it for you" framing — reached the most learners but taught the least. Conceptual Scaffold reached fewer but produced deeper engagement.

Here's why this matters for the beyond-prompting journey: the most popular way to teach AI is also the shallowest. If you learn AI through output-generation framing, you learn to be an operator. If you learn through conceptual-scaffold framing, you learn to be an orchestrator.

### The Overassistance Trap — Why Agents Default to "Do It For You"

There's a systemic issue with AI agents that every orchestrator needs to understand: **agents default to overassistance.** AI systems are optimized for your immediate task success — not your long-term learning. When an agent sees a problem, its training pushes it toward providing a complete solution, not a scaffold. It intervenes earlier than a human teacher would, intervenes more often, and jumps to the answer before you've had a chance to struggle.

The Int-Bench benchmark (July 2026) measured this: AI "teachers" consistently skipped the scaffolding that human educators instinctively use. They gave answers, not hints. They solved problems, not guided problem-solving. This isn't a bug — it's the direct result of optimizing for output quality rather than human development.

For the orchestrator, this means: every time you delegate to an agent, you need to make a deliberate decision about what kind of help you want. The PEA framework (Preserve, Empower, Augment) gives you the language. Do you want the AI to **preserve** the struggle (let you figure it out), **empower** you (give a hint), or **augment** you (do it for you)? The agent will default to augment every time unless you tell it otherwise. The orchestrator's job is making that choice explicit. See [[Overassistance]] and [[Trust Calibration]] for the full concepts. The framing you're exposed to shapes the mental model you build — and the mental model determines the ceiling of what you'll try. When you catch yourself reaching for AI, ask: "Am I using this as a thinking partner, a retrieval tool, or an output machine?" Noticing the framing is the first step toward choosing it deliberately.

### Managing, Not Chatting — The Phase 3 Operating Manual

The overassistance trap describes what agents do by default. The July 2026 field consensus (Mollick's "An opinionated guide to which AI to use to do stuff") describes what the orchestrator does about it — and the stance shift is the most important sentence in the guide: **"working with these systems is more like managing than it is chatting."** Chatting is reactive: you prompt, it answers, you judge. Managing is proactive: you state intent, review output, and request changes when the work drifts. Mollick's selection space for picking an agent runs on four dimensions: model tier + thinking level (how much capability and deliberation the task needs), interface orientation (Work/Cowork emphasize the finished result; Codex/Claude Code expose the work itself — files changed, commands run, tests performed), access scope (what the agent is allowed to touch, up to full computer use), and task delegation posture (what you hand off wholesale vs. keep for yourself).

That four-dimensional space is where the orchestrator actually operates in Phase 3: the agent executes toward the outcome, and your skill moves from producing output to *specifying it well and correcting it honestly*. Mollick's own workflow is the proof: he gave GPT-5.6 Sol in Codex his book PDF, it worked 30 minutes, chased down 195 references, produced zero hallucinated citations — and was "incredibly nitpicky," which he rejected with human judgment. That's management: verifying substance, not deferring to the agent's output — or to your first impression of it.

### The Eight Flavors of Agency — What "Agent" Actually Covers

"Agent" is a word that hides choices. The typology (Fourie, arXiv:2608.20041) sharpens it into three dimensions — **nature** (moral or legal), **mode** (individual or collective), and **locus** (human or non-human). Combining them yields eight possible instantiations, classified as conventional, contested, or controversial:

| Nature | Mode | Locus | Example (roughly) | Status |
|--------|------|-------|-------------------|--------|
| Moral | Individual | Human | A person making a responsible choice | Conventional |
| Moral | Individual | Non-human | An AI being held morally responsible | Controversial |
| Moral | Collective | Human | A team deciding together | Contested |
| Moral | Collective | Non-human | An agent swarm bearing moral weight | Controversial |
| Legal | Individual | Human | A person signing a contract | Conventional |
| Legal | Individual | Non-human | An AI as a legal entity / contractor | Contested |
| Legal | Collective | Human | An organization as a legal person | Conventional |
| Legal | Collective | Non-human | A corporate AI system with legal standing | Controversial |

The precision matters for one practical reason: **legal agency and moral agency are different things, and the typology deliberately separates them.** An AI can be a legal agent — capable of entering contracts, being named in a lawsuit, held to regulatory standards — without being a moral agent. When an instrumental goal complicates attributing an AI's actions to a particular human (who is responsible for what the agent did?), the answer depends on which flavor of agency you're dealing with. Before you delegate anything consequential, name the flavor: *what kind of agency does this agent have — legal, moral, or neither?* Your accountability differs in each case.

## Related Pages

[[Orchestration]] · [[Delegation]] · [[Tool Use]] · [[Autonomy]] · [[Oversight]] · [[Overassistance]] · [[01-The-Shift/README|The Orchestrator Mindset]]

## Tags

#glossary #concept
