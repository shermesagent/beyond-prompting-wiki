---
source_url: https://arxiv.org/abs/2609.03460
ingested: 2026-09-05
sha256: 3dbd433f9f0f3f3e986577625e887ec4b9e6465f94cc57b5d5d5e255d2132544
---
# Beyond "Made with AI": Visualizing Provenance Density to Mitigate the Transparency Penalty

**Source:** arXiv:2609.03460 (Zhang, Huang, Lee, Starner & Rekimoto), published 2026-09-04

**Summary:** Now that generative AI makes polished prose cheap, fluency can no longer serve as a proxy for truth. The paper names the failure mode the **Fluency Trap**: readers trust fluent hallucinations *and* discount accurate content once it is disclosed as AI-generated (the transparency penalty). Binary "Made with AI" labels answer the authorship question but not the support question — they show *where text came from* without showing *what backs a claim*.

The proposal is **Provenance Density**: an evidence-visualization interface that shows the density of verified claims within a text. In a user study with 81 participants, an idealized version produced a large discernment gap between truth and fabrication (**+4.15 points, d = 1.82**), while participants given no signal showed **no detectable discrimination** at all — they could not tell fluent truth from fluent fabrication.

A technical audit (200 samples) adds an important twist: retrieval density alone is insufficient. On dynamic queries, a **Consistency Veto** — checking whether claims hold up consistently against the evidence over time — carries most of the discriminative signal.

**Bottom line:** transparency that stops at "this was made with AI" is nearly inert — it can make readers trust lies less *and* trust truths less. What restores discernment is showing the *evidence behind claims*. For anyone reviewing AI-assisted work: ask for what supports a claim, and check whether the claim stays consistent when you probe it — not just for a label.
