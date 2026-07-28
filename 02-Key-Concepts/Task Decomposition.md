# Task Decomposition

## What It Is

Task decomposition is the skill of taking a big, fuzzy goal — "write a report," "plan the training," "analyze the data" — and breaking it into clear, self-contained subtasks that an AI agent can execute one at a time. Instead of typing a 300-word prompt hoping the AI magically produces something good, you give it one well-defined step, check the output, and hand it the next step. It's the difference between dumping a pile of laundry on a friend's floor and handing them one folded shirt at a time.

## Why It Matters for Moving Beyond Prompting

This is **the** bottleneck skill. Most people who stay stuck in Phase 2 aren't stuck because they need better prompts. They're stuck because they haven't learned to see their work as a chain of delegatable pieces.

Here's what changes when you get good at this:

- **Quality goes up.** Agents make fewer mistakes on small, well-scoped tasks than on giant open-ended ones.
- **You stay in control.** Each subtask is a natural checkpoint. You review, adjust, then proceed — instead of crossing your fingers at the start and hoping.
- **Parallel work becomes possible.** Once you can decompose, you can hand different subtasks to different agents at the same time.
- **You build reusable building blocks.** A well-decomposed task becomes a template you can use again.

Decomposition is what separates the operator — who types and hopes — from the orchestrator — who designs and delegates.

## How to Spot It in Your Day

You're decomposing well when:

- You can describe a complex project as a numbered list of 3–7 steps
- Each step has a **single clear deliverable** (not "work on the report" but "write the executive summary section in 2 paragraphs")
- You know what "done" looks like for each step before you hand it off
- You can hand steps 2 and 3 to different agents without them stepping on each other

You're **not** decomposing when:

- Your prompt is longer than a paragraph and mixes three different requests
- You're "editing" AI output more than you're checking it
- You find yourself re-prompting the same thing over and over hoping for a better result
- You feel like you're just a "better prompt engineer" rather than a designer of workflows

## The Absorption Check

New research on the Absorption Pattern (Zhang, Zhang & Sun, arXiv July 2026) adds a critical question to task decomposition: **is this subtask developmental?**

When you break a task into subtasks, some pieces build your expertise. Others are pure execution. The diagnostic question:

- **Developmental subtasks** — the ones that start with "figure out," "understand," "decide" — build the judgment you need to orchestrate effectively. These should be scaffolded by AI, not solved by AI. Let the AI guide, but keep the productive struggle.
- **Non-developmental subtasks** — formatting, transcription, rote assembly — are safe to delegate entirely. You don't build judgment by formatting tables.
- **Unclear? Assume developmental.** The cost of absorbing a developmental task is permanent (you never build the capability). The cost of doing a non-developmental task yourself is temporary (time you could have saved). Err toward preservation.

The orchestrator's decomposition isn't just about what the task *is*. It's about what the task *does to you*. A well-decomposed workflow preserves the subtasks that build you while delegating the ones that don't. See [[The Absorption Pattern]] for the full framework and the research behind it.

## Try This

**5-Minute Exercise: Decompose One Real Task**

1. Pick one thing you actually need to do this week — ideally something you'd normally ask ChatGPT about.
2. On a piece of paper (or a note app), write the goal at the top.
3. Underneath, list 3–5 subtasks. Each subtask must:
   - Have a single, specific deliverable (a paragraph, a list, a table, a decision)
   - Be something you could hand to a competent but literal-minded assistant with a one-sentence instruction
   - Build on the previous subtask's output
4. Now circle the first subtask. That's the only one you'd hand to an agent. Everything else waits.
5. Bonus: Actually hand that first subtask to an AI agent and see what comes back.

Time yourself. If you're still writing subtasks at the 5-minute mark, pick a smaller original goal next time.

## The Instruction Bleed Warning

There's a hidden cost to how you decompose: **adjacent subtask prompts sharing a context window can silently interfere with each other.** Lin & Liu (arXiv:2606.26356) formalized this as Compositional Behavioral Leakage (CBL), and we call it [[Instruction Bleed]].

Here's the problem. You decompose a big task into three subtasks. Each gets its own prompt template. Everything works. Then you improve subtask #1 — better wording, clearer expectations — and suddenly subtask #2's output drifts. No shared variables. No explicit dependency. Just two prompts occupying the same context window, and one's change subtly warping the other's behavior.

This matters for decomposition because **the closer your subtasks sit to each other in a shared context, the more vulnerable they are to bleed.** The fix isn't to stop decomposing — it's to be intentional about isolation:

- **Same-chat decomposition** (all subtasks in one chat window) is convenient but bleed-prone. Use it for rough drafts, not production pipelines.
- **Separate-window decomposition** (each subtask in its own context) eliminates bleed at the cost of manual handoffs. Use it when output quality matters more than speed.
- **Reset-gated decomposition** (add explicit "ignore all previous instructions" between subtasks) is a middle ground. It helps but doesn't fully eliminate bleed — residual context can still leak.

The orchestrator's decomposition isn't just about what the pieces are. It's about how close they sit to each other, and which ones can leak.

See [[Instruction Bleed]] for the full concept, the isolation test pattern, and the connection to [[Friction by Design]].

## The Context Anxiety Problem: Decompose Small Enough to Prevent Premature Stops

New research on "AI Context Anxiety" (arXiv:2607.21616, July 2026) reveals a structural reason to decompose more finely than you might think: **frontier reasoning models sometimes stop working on a task not because they can't do it — but because they misestimate their token budget and panic.** The model possesses the capability. It just thinks it'll run out of space and quits early.

This creates a decomposition design principle: **if your subtask feels big enough to trigger context anxiety, it's not small enough.** The model that can handle a 10-step analysis may choke on a 10-step analysis described in one delegation — but breeze through 10 separate 1-step delegations. Same work. Different decomposition. Different result.

The practical rule: when delegating to reasoning models, **decompose to the point where each subtask looks completable to an anxious agent.** The subtask should look like something the model *knows* it can finish, not something it has to estimate whether it can finish. The difference between "analyze this dataset" (triggers: how deep? how many tokens?) and "calculate the mean of column A" (no ambiguity, no anxiety) is the decomposition boundary that prevents silent failure.

See [[AI Context Anxiety]] for the full concept and the Continue Prompt Test.

## The Procedural Knowledge Blind Spot: Why LoRA Fails at Multi-Step

Not all training methods are equal when it comes to the kind of tasks you decompose. New research on parameter-efficient fine-tuning (arXiv:2607.21612, July 2026) found that **LoRA — the default method for efficient fine-tuning — fails to match full fine-tuning for procedural (multi-step execution) knowledge at the low ranks where it retains its efficiency advantage.**

In plain language: if you're fine-tuning a model to follow a multi-step procedure, LoRA at the low ranks you'd normally use (the whole point of LoRA) can't internalize the sequential dependencies. The model learns the pieces but not the relationship between the pieces. Full fine-tuning captures the temporal ordering. LoRA captures the vocabulary.

This matters for decomposition because it defines a hard boundary: **the orchestration layer must handle sequencing that the model layer cannot.** If you're using a LoRA-tuned model (common for domain-specific agents), you cannot rely on the model to maintain procedural integrity across steps. You must decompose the procedure into atomic steps and call each step independently — the same way you'd write a script that orchestrates function calls rather than expecting a single function to handle the whole pipeline.

The orchestrator's decomposition doesn't just serve the human's cognitive limits or the model's context window. It serves the model's training architecture. A model that can't learn "first do X, then Y depends on X's output" in its weights needs an orchestration layer that enforces that dependency. Your decomposition is that layer.

## Related Pages

[[Delegation Thinking]] · [[Trust Calibration]] · [[01-The-Shift/README|The Orchestrator Mindset]] · [[05-Practice/README|Practice Section]] · [[Instruction Bleed]] · [[Friction by Design]] · [[AI Context Anxiety]] · [[Lexical Oscillation]]

## Tags

#concept #orchestrator #workflow #delegation-failure
