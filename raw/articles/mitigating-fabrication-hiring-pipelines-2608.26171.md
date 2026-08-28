---
source_url: https://arxiv.org/abs/2608.26171
ingested: 2026-08-28
sha256: af8de63999abdb846a65914fea0f1c569775c73530333be2f92571a57cc4c45d
---
# Mitigating Fabrication in Multi-Stage LLM Pipelines for Hiring: An Empirical Evaluation of Prompt Guardrails and Human-in-the-Loop Checkpoints

**Source:** arXiv:2608.26171 (cs.CY)

**Abstract:** Multi-stage LLM hiring pipelines (resume improvement, interview question generation, answer feedback) can fabricate credentials, inflate qualifiers, and invent experience. We evaluate two mitigations, prompt guardrails and human-in-the-loop (HITL) checkpoints, against a fully automated baseline. In a controlled experiment (10 synthetic resumes x 2 job descriptions x 3 repetitions x 3 conditions; 180 runs), the baseline (C1) produced at least one unsupported claim in 96.7% of outputs (mean 6.80 findings/output). Prompt guardrails (C2) reduced finding density by 86% (6.80 to 0.92/output), but 50.0% of outputs still contained a fabrication, showing prompt-level mitigation alone is insufficient. A human checkpoint after resume improvement (C3) eliminated all identity fabrications, reduced finding density by 59% (6.88 to 2.82/output), reduced item-level fabrication from 96.7% to 75.0% (p=.022), and cut capture of JD-embedded trap requirements from 47% to 2% (vs. 5% under the guardrail). An exploratory analysis of multi-specialty resumes shows contamination rising monotonically with domain distance between specialties, suggesting career changers are especially exposed. The reviewer in this study caught all flagrant fabrications, but subtle qualifier drops and plausible new claims survived review roughly half the time (54.5% removal). Neither mitigation degraded the deliverable: claim retention exceeded 99% under both. The interventions are complementary: the guardrail eliminates unprompted additions and qualifier inflation cheaply, while the checkpoint gives near-categorical guarantees against the most severe failures, invented identities and JD-baited claims. These results support a layered architecture combining guardrails with a human checkpoint. A supplementary run with a newer-generation model (90.0% baseline fabrication rate) suggests the problem is not resolved by model progress alone.

**Key takeaways for the wiki:**
- Verification is a layered system: cheap mechanical guardrails (cut finding density 86%) + expensive human checkpoints (eliminate the severe failure class). Neither alone is enough.
- A human checkpoint is not a cure-all: the reviewer caught every flagrant fabrication but subtle qualifier drops and plausible new claims survived review roughly half the time (54.5% removal).
- Checking does not degrade the deliverable: claim retention exceeded 99% under both mitigations.
- Career changers are especially exposed: contamination rises monotonically with domain distance between specialties.
- Model progress alone does not fix fabrication: a newer-generation model still had a 90.0% baseline fabrication rate.
