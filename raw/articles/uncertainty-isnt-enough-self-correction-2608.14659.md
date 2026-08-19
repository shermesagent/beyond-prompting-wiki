---
source_url: https://arxiv.org/abs/2608.14659
ingested: 2026-08-18
sha256: 0708842624eff88b4a07c1a4fae89f167c8c51bedafd21cff8ab2122248e8590
---

# When Uncertainty Isn't Enough: An Empirical Study of Self-Correction in Code Generation

arXiv:2608.14659v1, 2026 (published 2026-07-31)

**Authors:** Pranav Rakasi; Maanas Lalwani; Arnav Srivastava; Arya Palanivel; Tinuade Adeleke; Ruizhe Li; Sean Wu

**Full abstract:**

Large language models for code generation often produce incorrect solutions without reliable indicators of failure. We study whether uncertainty estimation methods developed for natural language transfer to code generation, and whether such signals can improve code generation via selective self-correction. We evaluate five uncertainty methods: mean token entropy, verbalized confidence, P(True), entropy ensembles, and semantic entropy probes, across three small code LLMs on HumanEval and BigCodeBench. We find that multi-sample P(True) achieves the strongest correlation with correctness, while all the other methods, including semantic entropy probes, yield only weak correlation. We then use these uncertainty signals to drive three self-correction policies: adaptive decoding, uncertainty-based regeneration, and verification-based regeneration. Our results reveal a stronger negative finding than anticipated: uncertainty-based self-correction fails to reliably improve Pass@1, degrading accuracy in 5 of 6 configurations across both benchmarks (−3pp to −10pp), and adaptive decoding degrades accuracy in 4 of 6 configurations. Only verification-based self-correction reliably improves Pass@1, with gains of +6 to +26 percentage points on HumanEval and +8 to +20 percentage points on BigCodeBench, scaling inversely with baseline strength. These findings replicate consistently across both benchmarks and suggest that cheap uncertainty estimators are insufficient on their own to improve code correctness, and that their practical value lies in serving as gating signals for costlier execution-based correction loops rather than as standalone substitutes for verification.

**Key terms:** uncertainty estimation · selective self-correction · verification-based regeneration · code generation · P(True)
