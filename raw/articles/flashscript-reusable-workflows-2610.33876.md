---
source_url: https://arxiv.org/abs/2610.33876
ingested: 2026-10-27
sha256: 62a5f72f68e71d7e026ca1eed9c9df070c86ea96cd64add65019dbca2f3abc35
---
# FlashScript: Compiling Recurring Agent Workflows into Reusable Neuro-Symbolic Programs

Publisher: arXiv (v1 preprint; publisher RSS abstract and Atom metadata)
Submitted: 2026-10-24; announced: 2026-10-27
Authors: Sadra Sabouri, Hosein Hasanbeig, Adam Sage, Shreya Sinha, Cale Darling, Ashish Tiwari, Katie Garms, Souti Chattopadhyay, Sumit Gulwani

## Publisher abstract (retrieved from arXiv RSS)

Many agent tasks recur with new data or small changes, yet agents regenerate their reasoning and actions on each run, producing different results. Distilling a prior run into a skill helps the agent avoid earlier mistakes, but it still re-runs the full process each time, so runs can vary and incur that cost. We compile a successful agent run into a reusable neuro-symbolic program (NSP) with a set of guidelines we call FlashScript. Actions and data transformations become code, instance-specific values become parameters, and decisions that need model judgment become LLM calls. We identify three layers where these calls belong and three techniques that replace most of them with code. The compilation does not remove nondeterminism; it localizes it, so the deterministic program and its neural calls can be reviewed and tested separately. Across 120 WorkBench analytics tasks with Claude Haiku 4.5, the NSPs were correct and made identical tool calls on every run, using about 70 times fewer input tokens and a third of the runtime of a skill-guided agent whose runs were inconsistent. In a composite version of the tasks, the skill-guided agent's accuracy fell to 23%, and its output inconsistency increased, while the NSPs remained correct and identical across all runs. The NSPs successfully generalized to all 108 unseen instances of the same templates. Our findings suggest that NSPs from agent trajectories can be considered cumulative software assets for end-users to test, maintain, and reuse in their recurring workflows.

## Curator translation (not a tested intervention)

For a recurring public-data task, write the steps that never change as a checklist and circle the step that requires judgment. Check whether the fixed steps really repeat before automating anything. These are benchmark results on template analytics tasks, not proof that a workplace workflow is safe or that a human can dispense with review.
