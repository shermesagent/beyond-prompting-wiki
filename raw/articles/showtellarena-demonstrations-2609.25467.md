---
source_url: https://arxiv.org/abs/2609.25467
ingested: 2026-09-23
sha256: bada02ceff4e421debe32a7ff2d77f2cdb71e39062f4c70cdb190bc96a4145ee
---
# Source capture — ShowTellArena

Title: ShowTellArena: Evaluating Business Workflow Understanding from Demonstrations
Authors: David Garg, Ritobrata Sarkar, Ehsan Azarnasab, Siddhartha Borah
URL: https://arxiv.org/abs/2609.25467
Announced: 2026-09-23 (arXiv cs.AI RSS); v1. This is an abstract-grounded summary, not a full-text review.

The authors propose a benchmark for testing what an AI agent understands after watching a narrated business-workflow demonstration. The release contains 50 workflow tasks and 502 questions covering rules, boundaries, exceptions, and proposed-automation errors in finance, hiring, procurement, customer decisions, inventory, and logistics. They report 218 selected pilot attempts across 39 cases, including 28 cases attempted by all three evaluated systems. The pilot is exploratory, not a controlled ranking of products; coverage, exclusions, and grading limitations are explicit.

Practical takeaway: after showing an agent a task, do not treat completion as proof it understood the rules. Ask it what it would do at an exception, what it must not do, and what evidence supports each step; then test an intentionally wrong proposed automation before granting access.
