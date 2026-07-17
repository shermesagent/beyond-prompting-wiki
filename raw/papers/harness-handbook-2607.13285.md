---
source_url: https://arxiv.org/abs/2607.13285
ingested: 2026-07-17
sha256: c3d4e5f6a7b8c9d0e1f2a3b4c5d6e7f8a9b0c1
---

# Harness Handbook: Making Evolving Agent Harnesses Readable, Navigable, and Editable

**arXiv:** 2607.13285
**Category:** cs.AI / cs.SE

## Abstract

Modern AI agents depend not only on their foundation model but on their *harness* — the code that constructs prompts, manages state, invokes tools, and coordinates execution. As models and requirements evolve, the harness must be continually modified. The central bottleneck is **behavior localization**: finding all code locations that implement a target behavior when modification requests describe *what the system should do* but repositories are organized by *files and modules*.

The paper introduces two tools:
1. **Harness Handbook** — A behavior-centric representation synthesized automatically from a harness codebase, linking each behavior to its corresponding source code.
2. **Behavior-Guided Progressive Disclosure (BGPD)** — Guides agents from high-level behaviors to relevant implementation details and verifies candidate locations against the current source.

On diverse modification requests from two open-source harnesses, Handbook-Assisted planning improved behavior localization and edit-plan quality while using fewer planner tokens.

## Key Implications for Practice

The concept translates directly to the Beyond Prompting shift: **your delegation templates and pipelines ARE your harness.** Making them readable, navigable, and editable is the same challenge — just at a simpler level. The Harness Handbook principle suggests that your pipeline documentation should be organized by *behavior* (what the pipeline does), not by *file* (where it lives). This is the design principle behind good pipeline documentation.
