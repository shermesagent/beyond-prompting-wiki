---
source_url: https://arxiv.org/abs/2608.28880
ingested: 2026-09-01
sha256: 6eff4a425fa84ac18aafb6b6295d37cb51b84412e512852bdecbfe45b52ebb95
---
# FlowCheck: Helping End-Users Specify and Verify Intent in Vibe-Coded Web Apps

**Source:** arXiv:2608.28880 (cs.HC), published 2026-08-28

**Summary:** Vibe-coded applications often contain **silent behavioral failures**: the interface appears functional even though user-visible information does not flow to the expected state or output. Because vibe coding hands generation to an LLM, the resulting app can look right while quietly doing the wrong thing — and non-developers can't read the code to find out.

**FlowCheck** is a constraint language that lets end-users specify the user-visible information flows they care about **directly through the application interface** — where constraints can also be displayed and inspected without reading code, and are structured enough for reliable LLM generation. FlowCheck translates the constraints into deterministic CodeQL analyses.

Evaluation: across four applications generated via Claude Code, FlowCheck correctly translated and flagged **all 30 injected constraint violations with zero false positives**. In contrast, frontier models (Claude Opus 4.7, DeepSeek V3, Gemini Pro) prompted to find bugs in the same code showed significantly lower accuracy — none achieved full accuracy.

The design point: vibe coders state intent in terms of the interface they understand, and check it deterministically against the code they do not.

**Key takeaways for the wiki:**
- The failure mode of vibe-coded (and delegated) work is silent: it looks done, works at the surface, and fails invisibly underneath.
- Asking another model to find the bug is weak — prompting a frontier model to spot defects underperformed a deterministic check keyed to your stated intent.
- The fix pattern: state your intent in the language of the outcome (the interface), and check against the implementation deterministically. Intent + deterministic check beats "another LLM will catch it."
- For orchestrators: when you delegate generation, the spec you write is the constraint set — the more checkable it is, the more the verification can be automated rather than eyeballed.
