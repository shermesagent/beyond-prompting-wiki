---
source_url: https://arxiv.org/abs/2609.01873
ingested: 2026-09-04
sha256: 8ff2c5571c28260c397d4ea86cc22554f43e21dba63168255d30682bd7daabec
---
# Epistemic Sybil Resistance: Multiplying AI Agents Without Multiplying Evidence

**Source:** arXiv:2609.01873 (Marc Bara), published 2026-09-01

**Summary:** Multi-agent AI systems improve inference by spawning agents and synthesizing their reports — but another agent is **not** another observation. Apparently independent reports may all descend from the same evidence, and genuinely independent evidence can produce nearly identical reports. The paper formalizes this as an **epistemic Sybil problem**: a report adds nothing when it carries no information beyond reports already in hand, and **no report-only aggregator can generally distinguish replication from independent corroboration** — identical reports can warrant different conclusions under unobserved ancestry.

Key findings from more than 20,000 controlled LLM-agent report and extraction calls on synthetic evidentiary documents:

- **One evidence root, many copies:** holding one evidence root fixed while report multiplicity rises from 1 to 32 collapses naive posterior coverage from **0.940 to 0.263** — 32 copies of the same evidence feel like 32 witnesses.
- **Independent roots fix it:** holding report count fixed while evidence-root multiplicity rises from 1 to 16 closes the gap entirely — aggregators are statistically indistinguishable at k = 16.
- **Shared models corrupt copies:** replicate extraction errors among agents sharing a base model are correlated (γ_cal = 0.719, estimated out of sample); a correlated-extraction aggregator restores calibration accordingly.
- **Similarity tools mistake copies for corroboration:** a controlled manipulation shows report-space deduplication mechanisms track *representation similarity* far more than *evidential ancestry* — changing similarity moved the inferred cluster count by 1.425, while a fourfold change in true ancestry moved it by only 0.040.

**Bottom line:** collective inference should track evidential ancestry and dependence — not agent count, report count, or how similar the reports look. Five agents agreeing is a consensus only if five independent evidence roots stand behind them; otherwise it is an echo.
