---
title: Authorship Calibration
created: 2026-07-19
updated: 2026-07-19
type: concept
tags: [concept, orchestrator, metacognition]
confidence: high
sources:
  - raw/papers/authorship-calibration-2607.15006.md
---

# Authorship Calibration

## What It Is

Authorship calibration is knowing what *you* contributed to AI-assisted work versus what the AI contributed — and being honest about the difference. It's the metacognitive skill that sits underneath every delegation decision, every pipeline design, every moment you decide "that's good enough."

The term comes from a July 2026 study that found people systematically *overestimate* their own contribution to AI-assisted work. The more the AI contributed, the more people inflated their own role. This isn't dishonesty — it's a calibration failure. When the AI's contribution blends into the work, the human brain fills in the gap with itself.

## Why It Matters for Moving Beyond Prompting

The operator→orchestrator shift depends on accurate self-assessment. You need to know:

- **When to delegate:** If you think you're doing more than you are, you'll under-delegate — you won't hand off tasks the AI could handle entirely because you think your contribution is essential.
- **When to override:** If you think the AI is doing less than it is, you'll over-trust — you'll accept AI output without the scrutiny it needs because you don't see how much of the work the AI already shaped.
- **What to practice:** If you can't separate your contribution from the AI's, you can't tell which skills are actually yours and which are rented. The skills you think you're developing might be artifacts of your AI use.

The orchestrator's calibration: **you should be able to name, specifically, what you brought to any AI collaboration.** If you can't, the AI isn't your tool — it's your co-author, and you didn't even notice.

## The Three Calibration Failures

The research identifies three distinct ways authorship calibration breaks down:

| Pattern | What It Looks Like | The Risk |
|---------|-------------------|----------|
| **Over-attribution** | "I wrote that" — when the AI did 80% of the work. | You don't delegate enough. You think your contribution is essential when it may not be. |
| **Under-attribution** | "The AI did everything" — missing where your framing, judgment, and direction-setting made the difference. | You over-delegate. You stop practicing judgment because you think the AI is doing it all. |
| **Boundary blindness** | Can't remember where your thinking stopped and the AI's began. | The most dangerous. The AI shapes the work in ways you can't see, and you credit yourself for its choices. |

Boundary blindness is the most common and the hardest to self-detect. It's what happens when AI is integrated into your workflow so smoothly that the seams disappear. The output feels like yours. It might even *be* good. But you can't trace which parts reflect your judgment and which reflect the AI's patterns, its training data biases, or its tendency to fill gaps with plausible-sounding fabrication.

## Why This Gets Worse Over Time

Three factors make calibration harder the more you use AI:

1. **Opacity breeds miscalibration.** The study found that when the AI's contribution was less visible — integrated into the workflow rather than clearly demarcated — miscalibration was worse. As AI becomes more seamless, your ability to assess your own contribution degrades.

2. **Skill drift masks itself.** The skills you stop practicing don't announce their departure. They fade gradually, and your AI-augmented output looks the same or better. The quality of the *product* is stable. The quality of *you* is declining, and you can't see it.

3. **AI fluency hides the seams.** The better the AI gets at mimicking your voice, your format, your reasoning style, the harder it becomes to tell where you end and it begins. This isn't a bug — it's the feature. AI companies are explicitly designing for this.

## How to Recalibrate

### The Contribution Audit (2 minutes per collaboration)

After any significant AI collaboration, ask three questions:

1. **What specifically did I contribute?** Not "I wrote the prompt." What judgment, framing, or decision was uniquely yours? What would the output be missing if you hadn't been involved?

2. **What specifically did the AI contribute?** The generation, sure. But also: connections it made, structure it imposed, assumptions it baked in that you didn't catch, evidence it selected and evidence it ignored.

3. **Can I separate them clearly?** If the answer is "not really," that's boundary blindness. It's common. But it means the AI is doing more shaping of the work than you realize. Flag that collaboration and apply the seam exercise below.

### The Seam Exercise (5 minutes, once a week)

Pick one AI collaboration from your week. Print it out or open it side by side with a blank document. Go through it line by line and mark:

- **M** for "mine" — this thought, framing, or decision came from you before the AI touched it
- **A** for "AI's" — this came from the AI's generation or inference
- **?** for "unsure" — you can't trace the origin

If more than 30% of a piece is marked "?", you're operating with boundary blindness on that type of work. That's your calibration project for next week: deliberately separate your framing from the AI's execution on that task type.

### The Offline Check (monthly)

Once a month, do a task you normally do with AI — without it. Pick something small: a one-page brief, a data analysis, a lesson plan outline. Complete it unaided. Then compare it to your AI-assisted work on the same type of task.

The gap you feel — the friction, the slower speed, the missing connections — tells you what the AI has been carrying. Some of that gap is healthy (AI handling execution while you keep judgment). Some of it is atrophy (skills you've stopped practicing). The Offline Check makes the distinction visible.

## Authorship Calibration and the Phase Progression

Calibration means different things at different phases:

- **Operator:** You probably over-attribute — "I wrote good prompts, so the output is mine." The calibration work is recognizing how much of the output's quality comes from the model, not your input.
- **Orchestrator:** You risk under-attribution — "the pipeline did it all." The calibration work is recognizing that your spec design, constraint-setting, and verification criteria *are* real contributions, even if you didn't touch the output directly.
- **Architect:** The calibration problem becomes systemic. You're designing systems where multiple agents collaborate. Your contribution isn't in any single output — it's in the architecture that produces consistent quality across hundreds of outputs. The risk is losing touch with individual outputs entirely, trusting the system without verifying it still works.

## The Connection to Co-Existence

Ethan Mollick's Co-Existence frame (June 2026) says the key skill is knowing when AI is better than you. Authorship calibration is the prerequisite for that skill. You can't know whether the AI outperformed you if you can't separate what each of you did. The Co-Existence calibration question — "was the AI better than me at this?" — only works if you can answer "what did I actually do?"

Similarly, the [[The Augmentation Trap]] describes the pattern where AI productivity gains hide skill erosion. Authorship calibration is the diagnostic that catches Augmentation Traps before they're deep. If you can't trace your contribution, you can't tell whether you're augmenting or atrophying.

## Related Pages

[[Delegation Thinking]] · [[The Augmentation Trap]] · [[Co-Construction Blindness]] · [[Cognitive Surrender]] · [[From Author to Editor]] · [[The Coaching Stance]] · [[Audit Your Prompts]] · [[The Line You Draw]] · [[Trust Calibration]]

## Tags

#concept #metacognition #orchestrator #calibration
