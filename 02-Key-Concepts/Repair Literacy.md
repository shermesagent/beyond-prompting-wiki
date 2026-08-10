---
title: Repair Literacy
created: 2026-08-10
updated: 2026-08-10
type: concept
tags: [repair, trust, breakdown, learning, orchestrator, practice]
sources: [raw/articles/2601.20749.md]
---

# Repair Literacy

## What It Is

**Repair Literacy** is the skill of learning from AI breakdowns. Named by Ammari, Chen, Zaman & Garimella (arXiv:2601.20749) after analyzing 10,536 ChatGPT messages from 36 undergraduates across one academic year, it captures their most striking finding: **repair work during AI breakdowns produces substantial learning about AI capabilities** — a crucial and underexplored dimension of AI competence.

The study identified five genres of student-AI interaction: *academic workhorse* (get the output), *emotional companion* (get support), *metacognitive partner* (think with the AI), *repair and negotiation* (fix what broke), and *trust calibration* (test what to believe). Two structural findings frame repair literacy:

- **Competence is negotiated, not adopted.** AI competence does not arrive as a one-time event. It emerges through ongoing relational negotiation — students build "genre portfolios" and match interaction patterns to learning needs over time.
- **Breakdowns are the curriculum.** When the AI fails and the student engages with the failure — diagnosing it, working around it, trying again — that engagement produces the deepest understanding of what the system can and cannot do.

## Why It Matters for Moving Beyond Prompting

The operator experiences an AI failure as an interruption: restart, re-prompt, try again. The orchestrator recognizes a failure as the highest-information event of the day — the moment the system's actual limits surface.

Repair literacy is the practice side of the shift from retrieval to synthesis. Every debugged pipeline, every rewritten verification checkpoint, every "why did it do that?" investigation is a repair-literacy deposit. And it has a neat symmetry with the overtrust engine (Fell, arXiv:2607.21757): effort spent *building* a system produces trust without accuracy — but effort spent *repairing* a system produces understanding. Trust what you test; repair what you learn from.

Repair literacy is also the antidote to the failure-driven failure modes this wiki documents:

- **Against Co-Construction Blindness:** blindly accepting output means the breakdown never surfaces — and neither does the learning. Repair literacy insists you meet the failure head-on.
- **With Friction by Design:** friction is deliberately inserted for reflection; breakdown is friction that arrived uninvited. Repair literacy turns it into the same kind of reflective event.
- **With The Vibe Compiler:** when a compilation fails, the question is reflective ("what did I not specify?"). A repair-literate user asks that question of every failure.
- **Against The Augmentation Trap:** automating around every breakdown bypasses the practice; repairing the breakdown keeps the cognitive work in your hands.

## How to Spot It in Your Day

You are building repair literacy when:

- The AI fails and your first move is *investigation*, not restart — you ask why it broke before you ask it to try again
- You can name your tools' failure modes from memory ("it does this when the context is ambiguous," "it truncates long lists," "it invents citations when asked for sources")
- A crash becomes a spec change — the failure teaches you what to add to your templates, briefs, or verification steps
- You can distinguish a model failure from a prompt failure from a pipeline failure
- You keep a record of what broke, even informally — not to blame, but to map

You are missing repair literacy when:

- Every failure gets the same response: "Let me rephrase that" with no investigation
- You blame the model for everything, or yourself for everything — with no mechanism in between
- You never change your workflow after a failure; the same failure recurs weekly

## Try This: The Breakdown Log

Start a plain file (or a note) titled **Breakdown Log**. For two weeks, every time an AI system fails — wrong output, silent truncation, refused task, invented fact — add one line:

- **What I asked** (one sentence)
- **What broke** (one sentence)
- **What I tried** (one sentence)
- **What this taught me about the system** (one sentence)

After ten entries, read the log top to bottom. You will have a map of your tools' failure modes — and that map is precisely what a good delegation spec is designed to prevent. Turn the top three entries into prevention: add the constraint, the checkpoint, or the verification step to your templates. You have just converted breakdowns into curriculum, and you are no longer prompting. You are orchestrating with repair literacy.

## Related Pages

[[The Orchestrator Mindset]] · [[Trust Calibration]] · [[Friction by Design]] · [[The Vibe Compiler]] · [[The Augmentation Trap]] · [[Co-Construction Blindness]] · [[Distributed Mastery]]

## Tags

#concept #practice #repair #trust #orchestrator
