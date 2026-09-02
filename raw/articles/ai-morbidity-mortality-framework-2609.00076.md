---
source_url: https://arxiv.org/abs/2609.00076
ingested: 2026-09-02
sha256: cfa4a3132f62c9a8480a428287893e5af65a48dc11c1fe7f1725a90e3cb737fe
---
# AI Morbidity and Mortality: A Framework for Clinical AI Failure Review

**Source:** arXiv:2609.00076 (Mui, Sittig, Labkoff & Basu), published 2026-08-31

**Summary:** Clinical AI is increasingly embedded in real care, but existing safety mechanisms are poorly suited to reconstructing and learning from individual AI-related errors and near-misses. Aggregate model monitoring can flag performance changes; traditional patient safety reporting can capture adverse events. **Neither explains how risk emerges across the interaction among AI systems, clinicians, workflows, and institutional controls.** The paper proposes AI M&M — a structured, blameless framework for case-based review of clinical AI failures.

- Four linked classification dimensions per event: **Trigger** (the condition that exposed a vulnerability) → **Mechanism** (the process that produced the risk) → **Clinical Pathway** (its consequence for care) → **Corrective Action** (the remediation assigned).
- Built on standardized case intake, **evidence preservation** and investigator-level reconstruction, tool-in-loop attribution, and corrective-action tracking.
- Demonstrated on five illustrative outpatient cases: two clinician reviewers independently applied all four axes and agreed on all 20 axis-level classifications.
- Intended to **complement** (not replace) model monitoring, safety reporting, and regulatory oversight — converting individual AI-in-workflow failures into actionable institutional learning.

**Why it matters for the shift:** Any organization running agents in real work will eventually have an AI failure that monitoring doesn't explain. M&M is the institutional ritual for that moment: review the case blamelessly, preserve the evidence, name the trigger and mechanism separately from the consequence, and track the fix. It's the organizational version of the review-first pattern — applied after the fact, so the organization learns instead of just apologizing.
