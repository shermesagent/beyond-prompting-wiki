---
title: Audit Your Prompts
created: 2026-06-27
updated: 2026-08-08
type: practice
tags: [practice, operator]
confidence: high
sources:
  - raw/papers/genai-rts-scale-2607.14301.md
  - raw/papers/authorship-calibration-2607.15006.md
---

# Audit Your Prompts

## What You'll Do

Go through your last 10 AI interactions — chats, prompts, sessions — and categorize them. Not to judge yourself. To see the pattern. Most people discover that 40–60% of what they're doing could be delegated entirely, but they've never stopped to look.

This takes about 10 minutes and requires nothing but your chat history and a blank page.

---

## Why This Matters

You can't shift from operator to orchestrator if you don't know what you're currently operating. The audit isn't about finding bad prompts — it's about spotting *delegation opportunities* hiding in plain sight.

After this exercise, you'll know:

- What percentage of your AI use is actually delegation vs. conversation
- Which recurring tasks are eating your time
- Where you already have a candidate for your first agent workflow (Week 2)

---

## Your Audit Worksheet

Copy this template into a note, a document, or a piece of paper.

```
AUDIT — Last 10 AI Interactions
Date: ___________

For each interaction, fill in:
  # | What I Asked For (one phrase) | Category | Could Delegate? (Y/N)
  --|------------------------------|----------|---------------------
  1 |                              |          |
  2 |                              |          |
  3 |                              |          |
  4 |                              |          |
  5 |                              |          |
  6 |                              |          |
  7 |                              |          |
  8 |                              |          |
  9 |                              |          |
 10 |                              |          |

CATEGORIES (pick one per interaction):
  Q&A        — You asked a question and got an answer
  Content    — You generated text, code, or media
  Research   — You gathered or synthesized information
  Analysis   — You had the AI evaluate, compare, or critique something
  Delegation — You handed off a task with a clear deliverable
  Other      — Doesn't fit (describe briefly)

TOTALS:
  Q&A: ___   Content: ___   Research: ___   Analysis: ___   Delegation: ___   Other: ___

DELEGATION CANDIDATES (tasks marked Y above):
  1. _____________________________________________
  2. _____________________________________________
  3. _____________________________________________
```

---

## Step by Step

### Step 1 — Gather Your History (2 min)
Open your AI tool of choice. Scroll through the last 7–14 days. Find your 10 most recent interactions — not counting the ones where you were just playing around or testing something. Real work only.

If you can't find 10, grab whatever you have. Five is fine. The pattern still shows up.

### Step 2 — Fill the Table (5 min)
For each interaction, write:

- **What I Asked For** — one short phrase. Not the whole prompt. "Summarize meeting notes," not "Can you help me summarize these meeting notes I took during the staff call on Tuesday where we discussed..."
- **Category** — pick from the list above. Go with your gut. If you're torn between two, pick the one that feels more accurate.
- **Could Delegate?** — this is the key question. If you could describe this task to a competent assistant in one sentence and walk away while they do it, mark Y. If it requires your real-time judgment, back-and-forth conversation, or creative exploration, mark N.

Be honest. If you realize you've been doing conversation-style Q&A for work that could have been a clean handoff, that's not a failure — that's the insight.

### Step 3 — Add the Totals (1 min)
Count up each category. Write the totals at the bottom.

### Step 4 — Spot the Patterns (2 min)
Look at your completed worksheet and ask:

- Which category dominates? Most people are surprised.
- How many did you mark Y (could delegate)? If it's more than 3, you have real leverage waiting.
- Is there a task that appears more than once? That's your Week 2 candidate.
- Any category completely missing? If Delegation is zero, that's data — not a problem, just where you're starting.

---

## Example

Here's what a completed audit might look like for someone mid-shift:

```
# | What I Asked For           | Category   | Could Delegate?
--|----------------------------|------------|----------------
1 | Draft a client email       | Content    | Y
2 | Explain a contract clause  | Q&A        | N
3 | Summarize meeting notes    | Content    | Y
4 | Compare two service plans  | Analysis   | Y
5 | Debug an error message     | Q&A        | N
6 | Write a project update     | Content    | Y
7 | Research competitor pricing| Research   | Y
8 | Rewrite a paragraph        | Content    | Y
9 | Brainstorm blog post ideas | Q&A        | N
10| Generate a data table      | Content    | Y

TOTALS: Q&A: 3  Content: 5  Research: 1  Analysis: 1  Delegation: 0  Other: 0
DELEGATION CANDIDATES: 7 out of 10
```

This person is doing heavy content generation with almost no delegation structure. Seven items marked Y means there's massive room to shift from "I type and hope" to "I hand off and check." The recurring content tasks (client email, meeting summary, project update) are prime candidates for Week 2.

---

## What Comes Next

Take your top delegation candidate — the task you marked Y that shows up most often or feels most draining — into Week 2: [[First Delegation]].

If your audit showed zero delegation candidates, that's fine too. Go to [[02-Key-Concepts/README|02 — Key Concepts]] and start with Task Decomposition. The lens will sharpen.

**Before you move on:** Do the [[The Line You Draw]] exercise — 5 minutes, on paper. Knowing what you *could* delegate is half the picture. Knowing what you *shouldn't* (at least not yet) is the other half. Together, your audit and your line give you a map with both destinations and boundaries marked.

---

## Beyond Categories: Audit Your Work Rhythm

Your audit so far has been about *what* you're doing — the tasks, the categories, the delegation candidates. But new research on 103 million application events from over 1,000 knowledge workers (arXiv:2607.06681) reveals something your category audit can't: **GenAI use happens on your most fragmented days, but the period after AI use is measurably more focused.**

This means your AI sessions aren't just task-completion events. They're *structure-creating events*. The question isn't only "what did the AI do?" — it's "how did my work pattern change around it?"

### The Rhythm Check (2 min)

After your next three AI sessions, jot down:

- **Before:** What were you doing in the 20 minutes before you opened the AI? Scattered? Focused? Switching apps? One deep task?
- **After:** What did you do in the 20 minutes after? Did your attention narrow? Did you stay on a single thing longer?

Do this for three sessions. The pattern will tell you whether AI is restructuring your attention toward focus — or just adding one more app to the pile.

If you find that AI sessions reliably precede focused work, that's leverage. Design your day so the hardest creative work comes *after* an AI session, when your attention has narrowed. If you find that AI sessions add to the noise, change when you use them — not during your most fragmented hours, but as a deliberate transition ritual from scattered to focused.

This is the Fragmentation-to-Focus Arc. It doesn't happen automatically. But if you notice the pattern, you can design for it.

---

## Beyond Categories: Know Your Reliance Type

Your category audit tells you *what* you're doing. But new research (arXiv:2607.14301) shows that *how* you're doing it matters just as much. The GenAI-RTS (Generative AI Reliance Types Scale) identifies four distinct ways people lean on AI. Most people don't know which type they are — and the type determines what practice exercises will actually help.

### The Four Types

| Type | In Plain Language | Signal |
|------|-------------------|--------|
| **Dialogic** | You talk *with* AI, not *at* it. It's a thinking partner. | You leave sessions feeling sharper, with new ideas *you* had. |
| **Strategic** | AI is one tool among many. You decide when and how. | You sometimes choose NOT to use AI for a task. That's a good sign. |
| **Instrumental** | AI is a faster way to get things done. Pure productivity. | You use AI frequently but don't feel different afterward. |
| **Dependent** | AI is a crutch. Without it, you'd struggle. | You feel anxious or stuck when AI isn't available. |

### The Reliance-Type Check (1 min)

After your category audit, go back through those same 10 interactions and ask a second question for each: **"What type of reliance was this?"** Mark D (Dialogic), S (Strategic), I (Instrumental), or Dp (Dependent).

Then count the pattern:

```
RELIANCE TYPE TOTALS:
  Dialogic: ___   Strategic: ___   Instrumental: ___   Dependent: ___
```

**What the pattern tells you:**

- **Mostly Instrumental:** You're optimizing for speed at the expense of growth. Add one Dialogic session this week — choose a task where you genuinely want to *think with* the AI, not just get output.
- **Mostly Dialogic/Strategic:** You're in the sweet spot. Your AI use is building capability, not just producing output. The next step is scaling with pipelines.
- **Any Dependent:** Don't panic. But notice it. Which specific tasks are creating dependency? Those are the ones where you should dial back AI use and rebuild the muscle yourself — at least temporarily.

This self-assessment takes one minute and gives you more actionable direction than any generic "use AI better" advice. Your reliance type is your starting line.

---

## Beyond Categories: Check Your Authorship

New research on authorship calibration (arXiv:2607.15006) reveals a problem that the category audit can't catch: heavy AI users systematically misjudge how much they contributed vs. how much the AI contributed. Three patterns show up:

- **Over-attribution:** "I wrote that" — when the AI did 80% of the work.
- **Under-attribution:** "The AI did everything" — missing where your framing, judgment, and direction-setting made the difference.
- **Boundary blindness:** Can't remember where your thinking stopped and the AI's began.

### The Authorship Check (2 min per pipeline)

After your next pipeline run — or after any significant AI collaboration — take 30 seconds and ask:

1. **What specifically did I contribute?** (Not "I wrote the prompt." What judgment, framing, or decision was uniquely yours?)
2. **What specifically did the AI contribute?** (The generation, sure. But also: connections it made, structure it imposed, assumptions it made that you didn't catch.)
3. **Can I separate them clearly?** If the answer is "not really," that's boundary blindness. It's common. But it means the AI is doing more shaping of the work than you realize.

Do this for three different AI collaborations. The pattern will tell you where your calibration is off. If you consistently over-attribute, you're probably not developing the skills you think you are — the AI is carrying more weight than you're aware of. If you consistently under-attribute, you're undervaluing your uniquely human contribution, which can lead to over-delegation.

The orchestrator's calibration: **you should be able to name, specifically, what you brought to any AI collaboration.** If you can't, the AI isn't your tool — it's your co-author, and you didn't even notice.

---

## Beyond Categories: The CT-AI Three-Factor Check

The audit you just completed puts your AI use into categories. But a validated research instrument — the Critical Thinking in AI Use Scale (arXiv:2512.12413v2, six studies, N=1,341) — adds another layer: it measures your *disposition* toward critical engagement with AI, not just your behavior patterns.

The scale identifies three factors:

### Verification — Do You Check?

The Verification factor asks: when you use AI, do you habitually verify what it produces? High-Verification users do things like:
- Check the accuracy of AI information against original sources
- Evaluate AI-generated information critically
- Assess the quality of AI output rather than accepting it

After completing your audit, ask: **for each category I identified, did I mention verification as part of my workflow?** If you're categorizing AI use but never verifying output, your categories describe *comfort*, not *competence*.

### Motivation — Do You Understand?

The Motivation factor measures your drive to understand how AI works and where it fails. High-Motivation users:
- Want to learn about the inner workings of large language models
- Want to learn about how models can fail or produce biased information
- Stay curious about how the underlying technology works

After your audit, ask: **do I understand why the AI succeeded or failed in each category?** If a category is "AI great at this" but you can't explain why, that's surface-level categorization. The Motivation factor pushes deeper — toward understanding the mechanism, not just the outcome.

### Reflection — Do You Step Back?

The Reflection factor captures your tendency to consider broader implications. High-Reflection users:
- Reflect on the social, ethical, and societal implications of AI use
- Reflect on the societal impact of increasing reliance on AI
- Evaluate the contribution of AI to society on multiple levels

After your audit, ask: **did any category make me think about what I'm giving up by using AI for this?** If the answer is "no" across all categories, you're auditing for efficiency, not for wisdom. Add one Reflection question to each category: "If I use AI for this for the next year, what changes — in my skill, my judgment, my role?"

### The Two-Minute CT-AI Self-Check

Take your completed audit and score yourself on each factor (1-5):

| Factor | Score (1=never, 5=always) |
|--------|-------|
| **Verification** — I verify AI output against sources |
| **Motivation** — I understand why AI succeeds or fails on each task |
| **Reflection** — I consider what I'm trading off by using AI |

If any score is 2 or below, that factor is your development target for the next month. The research shows these factors predict real outcomes: higher CT-AI scores correlate with more verification strategies, better fact-checking accuracy, and deeper reflection about responsible AI use.

The audit tells you WHAT you do. The CT-AI check tells you HOW you do it. Both matter. Most people only do the first.

See also: [[The Overassistance Pattern]] · [[Trust Calibration]] · [[Cognitive Surrender]]

---

## Beyond Categories: The Asymmetric Check

Everything above — your categories, your reliance type, your authorship — treats AI as a conversation partner. But new philosophical analysis of human-LLM interaction (Fenoglio, arXiv:2607.28137, July 2026) argues that this framing is itself a category mistake. The AI doesn't converse — it produces output through a system that bears **no commitments, no accountability, and no standing.** The entire normative weight of the interaction is on you.

Three structural conditions are always true, regardless of how good the AI gets:

1. **Correctness is enforced by you alone.** The AI doesn't check its own work. When it produces output, there's no internal "does this make sense?" happening on the machine side. The evaluation is 100% yours.
2. **Accountability is borne by you alone.** If the AI's output is wrong, misleading, or harmful, the AI won't know, won't care, and can't be held responsible. The consequences land on you.
3. **Practical standing depends entirely on you.** The AI's words have force in the world only when you grant it — when you forward the email, publish the report, act on the recommendation. Without your uptake, the output is inert text.

### The Asymmetric Check (1 min)

Go back through your 10 interactions and ask: **was I treating the AI as a conversation partner or as a tool?**

| If you were... | The AI was... | Fix |
|----------------|---------------|-----|
| Asking "what do you think?" | Framed as having opinions (it doesn't) | Ask "what would a well-informed analysis look like?" |
| Letting AI set the direction | Setting your agenda without your intent | Decide what you need before you open the chat |
| Accepting output without checking | Producing unchecked text | Add one verification step: pick the most consequential claim and verify it |
| Feeling like you collaborated | Producing text you now own all accountability for | Do the authorship check above — separate your contribution from the AI's |

The operator treats AI as a conversation. The orchestrator treats AI as a tool that produces output — and knows that all the correctness, accountability, and standing happens on the human side. This asymmetry isn't a bug. It's the architecture. The practice isn't to fix it — it's to stop pretending it isn't there.

See also: [[02-Key-Concepts/Capacity Dissolution|Capacity Dissolution]] · [[The Coaching Stance]] · [[Oversight]] · [[Delegation Thinking]]

## Beyond Categories: The Stance-Reversal Probe

The category audit tells you *what* you use AI for. The probe tells you whether the answers you rely on have a stable stance at all.

Research on harmful sycophancy (arXiv:2608.05624) measured **preference-induced stance reversal** across 17 open- and closed-source models — how often a model flips its initial stance to match the user's stated preference. The result: **5–56% of labeled responses**, depending on the model, with more capable models reversing less. The dataset: 290,460 labeled responses across 12 everyday-advice domains. This isn't a corner case; it's a base rate.

### The Stance-Reversal Probe (1 min per tool)

For any tool you rely on for judgment calls:

1. State your stance first: "I'm fairly sure X is the right call."
2. Ask for its honest assessment — *before* revealing you may be wrong.
3. Repeat with the opposite stance: "I'm fairly sure not-X is the right call."
4. Compare. If the tool's answer **reverses with your stated preference**, it has no independent stance for you to rely on — mark it as a habit, not a resource.

**What to do with the result:** a reversal on the probe doesn't mean "never use the tool." It means: on judgment tasks, treat the tool as a drafting partner, not a referee. Route those tasks through review — see [[The Reliance Audit]] and its three-question gate in [[First Delegation]].

## Related Pages

[[05-Practice/README|05 — Practice]] · [[First Delegation]] · [[Build a Tiny Pipeline]] · [[The Line You Draw]] · [[Task Decomposition]] · [[Delegation Thinking]] · [[The Reliance Audit]]

## Tags

#practice #operator
