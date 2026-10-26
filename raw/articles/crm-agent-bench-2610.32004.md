---
source_url: https://arxiv.org/abs/2610.32004
ingested: 2026-10-26
sha256: 7d4b2138a66036c13561f0bd12f330e7cd64cd8deed2dbe9ad45b6dc9da7f725
---
# CRM-Agent-Bench: Benchmarking Tool-Using Agents in Stateful Enterprise Environments

Publisher: arXiv (preprint, version 1)
Published: 2026-10-23 (publisher Atom metadata; announced 2026-10-26)
Authors: Monojit Banerjee, Zhujun Lan, Defu Cao

## Publisher RSS abstract (full paper not appraised)

Deploying language agents in real applications demands more than the right answer: an agent must execute a multi-step business process correctly, follow domain-specific rules, and interact with a user across a dialogue, where the gap between saying and doing is the gap between a satisfied customer and a real loss. We argue that a deployable-agent benchmark should jointly assess four facets: the outcome an agent reaches, the trajectory it takes, its operational viability, and its policy compliance. Customer relationship management (CRM), where mutable records meet operational rules and consequential effects, exercises all four. We introduce CRM-Agent-Bench, an execution-grounded benchmark of 555 stateful, multi-turn tasks across nine business domains and 36 capability tags. Each task supplies a task-specific executable contract drawn from checks over actions, arguments, order, response, target state, and protected state; success is the strict conjunction of the checks declared for that task. We evaluate the complete agent system through these contracts and report scored coverage, latency, and cost. Across sixteen systems evaluated on the audited final release, strict success spans 64.32% to 83.60%; the closely grouped leading systems nonetheless diverge sharply in cost and per-domain reliability. CRM-Agent-Bench offers an auditable framework for measuring contract-grounded business-transaction integrity and adherence to task-declared benchmark policies, with a portable structure designed for extension as models improve. Github repository: https://github.com/salesforce-misc/crm-agent-bench

## Curator note (interpretation, not source text)

The authors introduce 555 stateful, multi-turn customer-management tasks with checks on actions, ordering, response and protected records. Sixteen evaluated systems achieved strict success rates ranging from 64.32% to 83.60% on the audited release; this is a benchmark, not a workplace deployment or district result. Try an on-paper public-data handoff that checks outcome, steps taken and what must stay unchanged before considering more autonomy.
