---
source_url: https://arxiv.org/abs/2609.01202
ingested: 2026-09-02
sha256: fabbbaa389db8c5336e51932e5e9facbae627a675f0feab04998ba43b8589455
---
# Towards AI-Assisted Clinical Trial Matching: TrialGPT 2.0 — Real-World Deployment

**Source:** arXiv:2609.01202 (Fang, Jin, Tian, He & Geer), published 2026-09-01

**Summary:** Clinical trials fail because of insufficient patient enrollment, but prior AI systems mostly did eligibility assessment alone and were rarely evaluated in real oncology workflows. **TrialGPT 2.0** is an AI-assisted trial recommendation system designed for production: it doesn't just ask whether a patient qualifies — it assesses which trials warrant further consideration given the patient's current needs and local workflow priorities, and provides **structured, inspectable explanations for expert review**.

- Retrospective multicenter cohorts (288 cases): retrieved at least one clinician-recommended trial in its top 10 for ~91% of cases, while **reducing clinician screening time by 55.0%**.
- Six-month prospective evaluation embedded in an active precision oncology tumor board: contributed additional trial opportunities missed by the routine workflow, **expanding patient access to clinical trial participation by 90.9%**.
- Introduces NIH-TrialBench: 126 clinician-authored synthetic vignettes from 11 NIH Institutes and Centers.

**Why it matters for the shift:** A production deployment where AI widens the net and humans keep the decision. The system doesn't replace the tumor board — it changes what the board sees (more opportunities, faster screening) while keeping every recommendation inspectable. That is the orchestrator pattern at clinical stakes: the agent proposes, the expert disposes, and the explanation is part of the product. +90.9% access while cutting screening time is the "raise the ceiling" outcome (see The Floor and the Ceiling) measured in patient lives.
