# Small Business Automation

## What It Is

A story about a two-person bakery in Austin, Texas, that turned its entire back office into a set of agent workflows: inventory tracking and ordering, customer follow-ups, scheduling, and bookkeeping prep. Total setup time: three afternoons. No custom software. No engineering background. Just a willingness to stop doing assembly-line work by hand.

This is a fictionalized composite drawn from real patterns observed across multiple small businesses in 2025-2026. The names are invented. The numbers are honest.

---

## The Before

Em runs the front of house — counter, customers, social media. Jules runs the back — baking, ordering, books. Together they own Rise & Rye, a sourdough bakery that does about $340K in annual revenue and ships nationwide twice a week.

In spring 2025, their week looked like this:

- **Inventory and ordering**: Every Tuesday, Jules sat down with last week's sales data, this week's wholesale orders, the walk-in inventory, and three supplier websites. She'd cross-reference everything in a spreadsheet, place orders, and hope she hadn't missed anything. Time: ~4 hours.
- **Customer follow-ups**: Wholesale customers (coffee shops, restaurants) got irregular check-ins. Some went six weeks without contact. Em felt guilty about it constantly but didn't have a system. Time: ~2 hours/week, inconsistently.
- **Scheduling**: Two employees, plus Em and Jules. Weekly schedule done on Saturday morning in a Google Sheet. Time: ~90 minutes.
- **Bookkeeping prep**: Receipts, invoices, expense categorization — everything got dumped into a folder and handed to their accountant quarterly, who charged them extra for the cleanup. Time: ~3 hours/week of Jules's time.

Total backend hours: roughly **10-12 hours per week** for a two-person business. That's time not spent baking, not spent with customers, not spent sleeping.

Em put it this way: "We opened a bakery because we love bread. We spend more time in spreadsheets than in front of the oven."

---

## The Shift

The shift started when Em heard about the review-first pattern from a small business Meetup. The idea: AI produces a draft. You review and approve. No prompting back-and-forth. No starting from scratch.

She and Jules spent three afternoons building workflows — one for each pain point. Not custom software. Task descriptions fed into an agent tool that could read from spreadsheets, search the web, and write to Google Docs.

### 1. Weekly Inventory and Ordering

**The task description:**
*"Here is last week's sales data and current walk-in inventory. Check what we have. Check what we sold. Calculate what we need for next week's wholesale orders plus walk-in demand. Generate a purchase order for each supplier: flour, butter, eggs, packaging. Flag anything that's running lower than the 2-week safety threshold. I will review and approve before anything is ordered."*

**What it replaced:** Four hours of Jules cross-referencing spreadsheets and supplier sites.

**What it produced:** A complete purchase order draft with quantities, supplier links, and one flagged item (croissant butter running below threshold). Jules reviewed it in 15 minutes, adjusted one quantity, and approved.

### 2. Wholesale Customer Check-Ins

**The task description:**
*"Here is the wholesale customer list with last contact date and order history. For any customer we haven't contacted in 3+ weeks, draft a short, personal check-in email: how's it going, anything we can do better, here's what's new on the menu. Use the customer's name, reference their last order, and keep it to three sentences. Do not send — draft only. I will personalize and send."*

**What it replaced:** Guilt and irregular check-ins.

**What it produced:** Five draft emails every Monday morning. Em spent 10 minutes personalizing each — adding a specific memory, a joke, a genuine note. The check-ins became consistent without becoming robotic.

### 3. Weekly Schedule

**The task description:**
*"Here is employee availability, last week's schedule, and projected busy periods based on order volume. Generate a draft schedule that covers all shifts, respects availability, avoids back-to-back closing/opening shifts, and distributes weekend shifts evenly. Flag any coverage gaps."*

**What it replaced:** 90 minutes of manual scheduling every Saturday.

**What it produced:** A draft schedule in under two minutes. Jules reviewed it in 5 minutes, swapped one shift, and posted it.

### 4. Bookkeeping Prep

**The task description:**
*"Here is a folder of receipts, invoices, and bank transactions for the week. Categorize each expense (ingredients, packaging, shipping, equipment, marketing, utilities, rent). Summarize by category. Flag anything that doesn't fit or looks unusual. Output a weekly P&L summary."*

**What it replaced:** Three hours of Jules sorting through a shoebox.

**What it produced:** A categorized expense report with a weekly profit-and-loss summary. Their accountant's cleanup fee dropped by 60%.

---

## The After

| Metric | Before | After |
|--------|--------|-------|
| Weekly backend hours (combined) | 10-12 | 2-3 |
| Inventory ordering errors per month | 2-3 | ~0 (one flagged, caught in review) |
| Wholesale customer check-in consistency | Irregular | Every Monday |
| Accountant cleanup fee | Full rate | Reduced 60% |
| Time spent baking per week (Jules) | ~20 hours | ~28 hours |
| New wholesale accounts (6 months) | 3 | 7 |

But the number that mattered most to Em: "We stopped dreading Tuesdays. Tuesdays used to mean spreadsheets. Now they mean we both get to be in the kitchen together."

---

## What Made It Work

**They automated the assembly line, not the art.** Jules still creates every recipe. Em still decides which wholesale partnerships to pursue. The workflows handle the cross-referencing, the drafting, the categorization — the parts that feel like data entry. The parts that require taste, relationship, and creativity stay human.

**They used the review-first pattern for everything.** No workflow takes action without a human review step. The purchase order is a draft until Jules approves. The customer emails are templates until Em personalizes. The schedule is a proposal until someone checks it. This isn't just safety — it's what made them trust the system enough to use it.

**They started with the most painful thing.** Jules didn't try to automate the whole business at once. She automated inventory first — the thing that ate her Tuesday and made her resent her own spreadsheet. When that worked, the momentum carried them to the next workflow.

**They didn't buy anything new.** The agent tool was a $20/month subscription. Everything ran through Google Sheets and Docs, which they already used. Total technology spend: $20/month. Total time saved: ~35 hours/month.

This is the small business version of what happened at Farmersville ISD in [[The School District Shift]] and what Mara experienced in [[From Prompt to Pipeline]]. Different scale. Same pattern: stop doing assembly-line work by hand. Build a review-first workflow. Get your time back for the parts of the job that actually need you.

---

## The Real Numbers Behind the Story

Rise & Rye is fictional, but the numbers track with what's being reported across the small business AI landscape in 2026:

- A vendor running AI agents in production (Viktor, April 2026) reported replacing **~18 hours/week** of cross-tool work for their own team with review-first workflows
- Gartner expects 30% of generative AI projects to be abandoned after POC — but the ones that succeed share a common pattern: **scoped, repeatable tasks with defined inputs and outputs, reviewed before execution**
- Small business AI adoption in 2026 is shifting from "ask ChatGPT for help" to task-specific delegated workflows — with the review-first pattern as the default architecture

The 2-person bakery isn't an edge case. It's the sweet spot. Small teams have less process inertia, fewer approval chains, and a clearer picture of what's tedious and what matters. When a 2-person team saves 35 hours a month, that's not efficiency improvement. That's almost a full work week — returned to the work they started the business to do.

---

## You Can Do This Too

If you run a small business or team of 1-10 people:

1. **List everything you do in a week that feels like data entry.** Not the creative work. Not the customer conversations. The cross-referencing, the template-filling, the number-checking. That's your workflow roadmap.
2. **Pick the most painful one.** The thing that makes you dread a specific day of the week. Build a workflow for that one thing first.
3. **Write it as an outcome, not a process.** "Here's the data. Here's what I need. Produce a draft. I'll review it." Don't write step-by-step instructions. Describe what "done" looks like and let the agent figure out the steps.
4. **Review, don't rewrite.** When you get the draft back, mark what needs changing. Don't do it yourself. Give it back to the agent with your annotations and ask it to incorporate them. You're the editor, not the co-author.
5. **Run it for two weeks before judging.** The first few outputs will feel wrong — not because they're bad, but because you're not used to reviewing instead of producing. Give yourself time to adjust to the new role.

The shift from operator to orchestrator doesn't require an engineering team. It requires the willingness to let go of the middle — the part where you do the assembly — and invest your attention in the beginning (the spec) and the end (the review). That's a mindset shift, not a budget line item.

---

## Related Pages

[[The School District Shift]] · [[From Prompt to Pipeline]] · [[The Review-First Pattern]] · [[Delegation Thinking]] · [[Task Decomposition]] · [[03-Real-World/README|03 — Real World Stories]]

## Tags

#story #orchestrator #workflow
