---
title: First Delegation
created: 2026-06-26
updated: 2026-08-28
type: practice
tags: [practice, operator, orchestrator]
confidence: high
sources:
  - raw/articles/you-shall-not-pass-2607.00533.md
  - raw/articles/retry-switch-abstain-2608.11977.md
  - raw/articles/constitutive-vs-corrective-2603.19213.md
  - raw/articles/user-permission-policies-agent-overreach-2608.27443.md
---

# First Delegation

## What You'll Do

Take one recurring task from your audit — something you're currently doing by typing a prompt every time — and design a simple, repeatable agent workflow for it. Then test it once. That's it.

This takes about 10 minutes. You'll walk away with a delegation template you can use every time that task comes up again.

---

## Why This Matters

The operator types a prompt. The orchestrator hands off a task with clear instructions, checks the result, and moves on. The difference isn't complexity — it's clarity. This exercise builds the muscle of defining work *before* you hand it off, which is the single habit that separates Phase 2 from Phase 3.

You're not building a system yet (that's Week 3). You're learning to think like someone who builds systems.

---

## The Delegation Template

For any task you want to delegate, answer these five questions. Write your answers down — don't just think about them.

```
FIRST DELEGATION — Template

GOAL:
  What outcome do I want? (One sentence. Not "help with…" — the finished thing.)

TOOLS:
  What does the agent need access to? (Search? A file? A style guide? Nothing?)

STEPS:
  What are the 2–5 specific things the agent should do, in order?
  1.
  2.
  3.

SUCCESS CRITERIA:
  How will I know this worked? (Be specific. "The output includes X, excludes Y, and fits format Z.")

REVIEW CADENCE:
  When do I check it? (Every time? Spot-check every 3rd run? Weekly review?)
```

---

## Before You Delegate: Draw Your Line

Before you pick your task, take 2 minutes to answer a question most people skip: **what would you *not* delegate, even if the AI could do it perfectly?**

Research on 448 professionals found that people draw boundaries around three kinds of work:
- **Identity work** — tasks that feel like "who I am" professionally
- **Human-facing work** — tasks where someone else will judge *you* for the output
- **Design/taste work** — tasks that require judgment, not just correctness

You don't need to resolve these today. You just need to know where they are. If your audit showed 7 "Could Delegate" candidates but 3 of them cross your identity line, start with one of the other 4. Build confidence on the safe side of the line first. You can always move the line later — but you can't un-burn the trust from a bad first delegation.

**Quick check:** Look at your delegation candidate. Does it cross any of these lines?
- [ ] This task feels like "who I am" — my professional identity
- [ ] Someone else will see this output and judge me for it
- [ ] This task requires taste and judgment, not just accuracy

If you checked any box, that candidate isn't wrong — but it's not your *first* delegation. Pick one you didn't check. Start safe. Grow outward.

For a deeper exercise (5 minutes, reusable), do the full [[The Line You Draw]] boundary audit. It pairs with your prompt audit: one tells you what you *could* delegate, the other tells you where to start.

---

## Step by Step

### Step 1 — Pick Your Task (1 min)
Look at your audit worksheet from Week 1. Pick one task marked Y (could delegate) that:

- Shows up at least once a week
- Has a clear, predictable output (a document, a list, a summary, a draft)
- Doesn't require real-time judgment or deep creative exploration every time

Good candidates: daily news briefing, meeting note summary, weekly status update, email draft, data table generation, research roundup.

### Step 2 — Fill the Template (5 min)
Work through each section. Be specific. Vague goals produce vague output.

- **Goal:** "A daily briefing" is vague. "A 5-bullet summary of the day's top AI news, each bullet under 40 words, with source links" is specific.
- **Tools:** If the agent needs to search the web, say so. If it needs access to your notes, say so. If it can work from scratch, say so.
- **Steps:** Think of these as instructions you'd text a new team member. "1. Search for today's top AI stories. 2. Pick the 5 most significant. 3. Write a one-sentence summary of each. 4. Include the source URL for each. 5. Format as bullet points."
- **Success Criteria:** This is the checkpoint. If you can't describe what "good" looks like before you see the output, you're still in operator mode.
- **Review Cadence:** Delegation doesn't mean abdication. Decide up front how often you'll spot-check.

### Step 3 — Test It (3 min)
Open your AI tool. Paste your STEPS as the prompt. Don't over-explain. Don't add context. Just hand it off and let it run.

When the output comes back, check it against your success criteria. Does it pass? If not, adjust one thing in your STEPS — not the prompt you write, but the *template* — and try again next time.

### Step 4 — Save the Template (1 min)
Copy your filled template somewhere you'll find it next week. A note, a document, a pinned message. The point is that next time this task comes up, you don't rewrite the prompt — you reuse the template.

---

## Complete Example: Daily News Briefing

Here's what a filled delegation template looks like for a common recurring task.

```
FIRST DELEGATION — Daily News Briefing

GOAL:
  A 5-bullet summary of the most important AI news from the last 24 hours.
  Each bullet under 40 words. Each includes a source link.

TOOLS:
  Web search (for current news)

STEPS:
  1. Search for the top AI and tech news stories from the past 24 hours.
  2. Filter to stories with real significance — new research, product launches,
     policy changes, major industry moves. Skip rumors and hype.
  3. Select the 5 most important stories.
  4. For each story, write one bullet: the key fact in under 40 words,
     followed by the source URL.
  5. Format as a clean bullet list. Add a one-line header with today's date.

SUCCESS CRITERIA:
  - Exactly 5 bullets
  - Each bullet is a single, factual statement under 40 words
  - Every bullet has a working source link
  - No opinion, no commentary, no "in a significant development…"
  - I can read the whole thing in under 30 seconds

REVIEW CADENCE:
  Spot-check every 3rd briefing. Full review if a bullet feels off.
```

### Why This Works

- **The goal is specific.** Not "tell me the news" — a defined format with a defined constraint.
- **The steps are executable.** Anyone (or any agent) could follow them in order.
- **The success criteria are testable.** You can run down the checklist in 15 seconds.
- **The review cadence is realistic.** You don't need to check every output. You check often enough to catch drift.

---

## The PEA Governance Layer

Every delegation is a governance decision — whether you know it or not. New research analyzing 90 AI-assisted learning systems (arXiv:2607.21257, July 2026) identified three dimensions of assistance governance that directly apply to your delegation templates:

### Policy — What Help Is Allowed

Before you hand off a delegation, decide explicitly what kind of assistance you're authorizing. Are you asking the AI to:

- **Generate a complete draft?** (Full assistance — most delegation, works for low-stakes, non-developmental tasks)
- **Suggest improvements to your draft?** (Moderate assistance — good for tasks where you need to maintain voice and judgment)
- **Ask you questions that guide your thinking?** (Scaffolded assistance — best for developmental tasks where the struggle builds capability)

The delegation template's Prompt section is your Policy statement. Make it explicit. "Draft this report" is full assistance. "Review my draft for consistency and suggest three improvements" is moderate. "Ask me three questions that would make my draft stronger before you suggest anything" is scaffolded.

### Enforcement — How You'll Catch Oversteps

Policy without enforcement is wishful thinking. For each delegation, name how you'll verify:

- **The three-claim check:** Identify the three most consequential claims in the AI's output. Verify each against an original source.
- **The overassistance scan:** After receiving the output, ask: "Did the AI do more than I asked for? Did it add analysis I didn't request?" If yes, the enforcement boundary was crossed.
- **The voice check:** Did the output sound like you or like the AI? If you can't tell, the enforcement boundary needs tightening.

The Enforcement layer is where most delegation templates fail. People write good Policy (the prompt) and skip Enforcement (the review). Good enforcement doesn't mean reviewing everything — it means reviewing the right things.

### Authority — Who Can Override

The scoping review found that in 90 AI systems, authority to configure assistance levels almost never belonged to the user. It was centralized in system logic. Your delegation is different: **you are the authority.** But authority without practice is performance.

For every delegation template, name who decides:
- **You decide** — on outputs that represent your professional judgment, accountability, or identity
- **You approve** — on outputs where AI does the heavy lifting but you're the final gate
- **AI executes** — on outputs where you've verified the pattern enough times to trust it

The PEA framework isn't extra overhead. It's a vocabulary for what you're already doing — just more intentionally. The orchestrator who designs Policy, Enforcement, and Authority for every delegation is the one who moves beyond prompting. The one who doesn't is hoping the AI behaves well.

See also: [[The Overassistance Pattern]] · [[The Coaching Stance]] · [[The Scaffold Match]]

## Common Pitfalls

**"My first template was too vague."**
Normal. Vague goals produce vague output. Tighten one section — usually the Goal or Success Criteria — and test again.

**"The agent didn't follow my steps."**
Also normal. Agents are literal. If it skipped a step, your instruction probably wasn't explicit enough. Add the missing detail to your template, not to a one-off follow-up prompt.

**"This feels like more work than just typing a prompt."**
It is — the first time. But a template that takes 10 minutes to create saves you 3 minutes every time you reuse it. After four uses, you're ahead. After twenty, you've reclaimed an hour of your life.

**"I don't have a recurring task."**
Look again at your audit. Content generation and research tasks almost always repeat in different clothes. If you truly have nothing recurring, pick the single task that annoys you most and template it anyway. The practice is the point.

**"I let the agent do the thinking and just wait for the output."**
This is the Cognitive Outsourcing Trap — and it's backed by new research (arXiv:2607.07522). In a controlled study of human-AI co-creativity, people who self-reported higher cognitive outsourcing ("I let the other person do the thinking") produced LESS original ideas, even when working with another human. Delegation is task handoff, not thinking handoff.

The fix is simple: before you run your delegation template, write down one sentence about what *you* think the right answer might be. Your guess. It doesn't have to be correct — it just has to be yours. Then compare it to the agent's output. This 10-second check keeps your judgment in the loop and prevents the slide from "I'm delegating tasks" to "I'm outsourcing my thinking."

If you consistently find that the agent's output is better than your guess, that's not a problem — that's the point of delegation. If you find you've stopped making guesses at all, that's the trap. Start again.

---

## What Comes Next

Use this template at least twice before moving to Week 3. Each time you use it, note what worked and what didn't — then adjust the template. After two rounds, you're ready for [[Build a Tiny Pipeline]], where you'll chain two templated tasks together.

---

## The Evaluation Trap: Why Checking Isn't Enough

A randomized N=220 crossover study (Dickey, Mertzanidis & Psomas, arXiv:2607.27586, July 2026) found something that should change how you design every delegation template: **evaluating AI output and solving problems yourself are different muscles.** Students who spent a semester evaluating often-flawed GenAI solutions earned significantly higher homework scores — but showed zero transfer to exams, final grades, or structurally similar problems without AI available. They got better at spotting errors. They didn't get better at solving problems.

This is the evaluation trap: your delegation template asks you to review output against success criteria. That builds evaluation skill — can you spot when something is wrong? But it doesn't automatically build solving skill — can you produce correct output yourself? The two are related but distinct, and confusing them is the most common delegation mistake.

### The Fix: One Unaided Step

After your delegation template runs and you review the output, add 60 seconds:

1. **Pick the most consequential claim or decision in the AI's output.**
2. **Produce your own version — just that one piece.** A sentence, a judgment, a conclusion. Without looking at what the AI wrote.
3. **Compare.** Where do you agree? Where do you disagree? The disagreement points — even small ones — are where your judgment is actually contributing something the AI didn't.

This takes 60 seconds. It's not about double-checking (that's verification). It's about maintaining the solving muscle alongside the evaluation muscle. The N=220 study suggests that without this deliberate transfer step, the evaluation-only approach produces correct homework and fragile understanding. The orchestrator who only checks AI output is building one capacity (contestability) while letting another decay (reason-giving). See [[Capacity Dissolution]] for the full framework.

### The Capacity Check for Your Template

Before you finalize any delegation template, run it through Yao's five capacities (arXiv:2607.28041). Score each 0-2:

| Capacity | 0 (not exercised) | 1 (partially) | 2 (fully exercised) |
|----------|-------------------|---------------|---------------------|
| **End-setting** | AI decides what to produce | You pick the task but AI sets the approach | You define both task and approach |
| **Reason-giving** | You accept output without understanding why | You can explain some decisions | You can explain all key decisions |
| **Contestability** | You never question output | You spot-check occasionally | You challenge every consequential claim |
| **Refusal/revision** | You ship whatever the AI produces | You make minor edits | You reject and redirect when standards aren't met |
| **Participation** | You spectate while AI works | You monitor with occasional input | You're actively engaged throughout |

If your template scores 4 or below (out of 10), it's building dependency, not capability. That doesn't mean don't use it — some tasks genuinely don't need capacity preservation. But know what you're trading. A template that scores 8+ twice a week preserves capacity. A template that scores 2 every day dissolves it.

## The Reliance Gate: Three Questions Before You Delegate

Before a task enters your pipeline, it has to earn its place. The gate is three questions — the same three that define warranted reliance (arXiv:2608.05602):

1. **Humility** — Has this tool shown me where it's weak? (Does it say "I don't know," or does it always know?)
2. **Access** — Can I inspect what it did? (Steps, sources, reasoning — or a black box that hands me an answer?)
3. **Justice** — Does it take my disagreement seriously? (Or does it reverse its stance when I state a preference? See [[Audit Your Prompts]]' Stance-Reversal Probe.)

**Pass two of three on a routine task, and it's a candidate for delegation — with review.** Pass fewer, and it's not ready: keep the task human-side until the tool earns the warrant.

**The replacement rule (from [[The Reliance Audit]]):** if a tool fails all three on the same task twice, it's not a tool you're using — it's a habit you're carrying. Rebuild the workflow with checkpoints, or replace the tool. The AI Agency Knowledgebase's Human Review Checkpoints framework puts it plainly: gates belong *inside* the workflow, not at the end of it — that's why this page's template has a REVIEW CADENCE, not a "check at the end" line.

## The Recovery Drill: Retry, Switch, or Abstain

Your delegation template has a Goal, a Template, and Success Criteria — but what happens when the *delegate* fails? Most people only have one recovery strategy: retry. New work on robust tool-use (Chen et al., arXiv:2608.11977, August 2026) shows that trained agents and humans alike face the same three-way choice when a delegated call fails:

1. **Retry** — run the same path again (the tool call, the prompt, the same template).
2. **Switch** — change paths: a different tool, a different approach, a different template.
3. **Abstain** — recognize no viable path remains and stop — ask you, escalate, or report the failure instead of burning more attempts.

The research (7 models across 4 families, on the BENCH2ROBUST framework) found a **near-universal robustness gap**: agents trained and evaluated in failure-free environments fall apart when tool calls fail transiently, persistently, or silently. The fix that worked was combining *structured recovery knowledge* (what to do when a call fails — retry with what backoff, switch to which alternative, when to stop) with *learned recovery behavior* — together reaching 40.8–45.5% success under injected failures while preserving failure-free performance. Recovery was a designed strategy, not an afterthought.

### The Drill (90 seconds, add to your template)

Before you run your delegation template, add three lines to its header:

```
RECOVERY:
  Retry:   (when does a re-run make sense? e.g. transient error, output truncated)
  Switch:  (what's the alternative path? e.g. different tool, rephrase the Goal, split the task)
  Abstain: (when do you stop? e.g. second failed run, output that fails Success Criteria twice)
```

Then, when a run fails: **execute the drill in order, with a hard cap.** One retry, one switch — then abstain and come back with your own judgment. This is the delegation version of the Reliance Gate's replacement rule ([[The Reliance Audit]]): a task that fails the same way twice is a habit, not a tool.

The deeper point: **abstain is a delegation skill, not a failure.** The BENCH2ROBUST result shows the agents that survived injection were the ones that *knew when to stop*. Your template should make stopping an explicit, planned outcome — not something you do when you're frustrated. Write the abstain line first; the retry and switch lines will behave themselves.

## The Loop Role Check: What Your Slot Actually Is

Your template says what the agent does. The harder question is what *you* are doing while it runs — and the language we use for that has been quietly wrong.

A causal taxonomy of human runtime involvement (Baum & Laux, arXiv:2603.19213) clears it up. The real distinction isn't spatial — "in" or "on" the loop — it's **causal**:

| Role | What it means | Your template line |
|------|---------------|--------------------|
| **Constitutive (HITL)** | A human contribution is *necessary* for the output to exist. No human step, no result. | The GOAL (you set it), the REVIEW (you pass or reject) |
| **Corrective (HOTL)** | The system runs without you, but you're positioned to prevent or modify outputs — synchronously (watching), asynchronously (reviewing later), or anticipatorily (setting guardrails first). | The SUCCESS CRITERIA and REVIEW CADENCE, if the pipeline runs unattended |

The point isn't that one role is better. It's that **your template should say which one you're in** — because they demand different preparation:

- **Constitutive slot:** your job is *being there*. The output can't exist without you, so your attention is load-bearing. Prepare to actually do your step well.
- **Corrective slot:** your job is *preparedness*. The research is explicit that genuine oversight isn't a position — it's **genuine capacity to intervene**: you know what to look for, you have the access to inspect, and you could actually stop a bad output before it ships. A corrective slot without that capacity is theater: you're "on the loop" in name and out of it in fact.

### The Check (30 seconds, add to your template)

In your delegation template header, add one line:

```
LOOP ROLE: constitutive (output requires me)  /  corrective (runs without me — I intervene)
```

If you mark **corrective**, answer the three preparedness questions before you hit run:

1. *Do I know what a bad output looks like for this task?* (Name two failure patterns.)
2. *Can I inspect what it did?* (Access — see [[The Reliance Audit]] Q2.)
3. *Could I actually stop it before it ships?* (Not "would I notice" — "can I intervene".)

The same person often occupies both roles in one workflow — that role duality is a design problem, not a personality trait. Your template is where you design it.

## The Permission Policy: Decide in Advance, Don't Decide at Runtime

Your delegation template's TOOLS and SUCCESS CRITERIA constrain *what* the agent does. But there's a second kind of constraint that most first delegations skip: **the permission policy** — the explicit "allow / ask / never" rules for what the agent may do on its own.

New research on user-authored permission policies (arXiv:2608.27443; 113 non-technical participants supervising an 18-action simulated agent day) found something counterintuitive: **writing your own rules in advance was WORSE at blocking overreach than per-action approval** — 20.1 percentage points worse than human-in-the-loop, 14.5 points worse than automated review. And the reason wasn't the rules' content. It was that **participants chose "ask" for 114 of their 140 rules** — turning their standing policy into a standing decision to defer. Of the 148 overreach actions that ran under a policy, **133 followed a human approving them in the moment.**

The researchers name it the gap between *preference* and *commitment*: repeatedly choosing "ask" preserves case-by-case choice but prevents a standing policy from settling anything in advance. "Ask" feels safe — but it hands every decision back to your tired, in-the-moment self, which approves things your calm self would never allow.

### The Policy Check (3 minutes, add to your template)

For your first delegation, add a PERMISSIONS section and commit to real rules, not "ask" defaults:

```python
PERMISSIONS (allow / ask / never):
  Allow:   (what may the agent do without checking in? e.g. search, draft, summarize)
  Ask:     (what requires a checkpoint? e.g. sending anything, spending, sharing)
  Never:   (what is off the table? e.g. contacting people, final sign-off, irreversible actions)
```

Three rules of thumb:

1. **"Never" is the most important line.** If you can name what the agent may *never* do — no matter what you're asking for — you've drawn the boundary that protects you when you're not paying attention.
2. **"Ask" should be small and named, not the default.** Each "ask" rule is a decision you're deferring to a moment when you're busy. Reserve "ask" for genuinely ambiguous cases — and write what the agent should do *while* asking (wait? draft and hold?).
3. **The policy is a commitment device, not a formality.** The study's punchline — 133 of 148 overreach actions happened because a human clicked approve — means the danger isn't the agent running wild. It's *you* approving things you'd have vetoed in advance. The policy line is how your calm self wins over your busy self.

This pairs with [[The Line You Draw]]: that exercise maps what you won't delegate *at all*; the PERMISSIONS line maps how much rope the delegated task gets. Together they're your delegation constitution.

## Related Pages

[[05-Practice/README|05 — Practice]] · [[Audit Your Prompts]] · [[Build a Tiny Pipeline]] · [[The Line You Draw]] · [[Delegation Thinking]] · [[Task Decomposition]] · [[Capacity Dissolution]] · [[The Reliance Audit]]

## Tags

#practice #orchestrator
