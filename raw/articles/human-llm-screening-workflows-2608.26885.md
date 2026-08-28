---
source_url: https://arxiv.org/abs/2608.26885
ingested: 2026-08-28
sha256: 0a641266468a556604a1f4f75622ac39366283b58b9d1dc16854557fa376f3ae
---
# Evaluating Human and LLM Screening Workflows in a Conceptually Complex Scoping Review: Recall–Workload Trade-offs and Run-to-Run Consistency

**Source:** arXiv:2608.26885 (cs.HC / evidence synthesis)

**Abstract:** Background. Large language models (LLMs) are increasingly used for screening in evidence synthesis, where false negatives can remove relevant studies before full-text assessment. We compared human and LLM title-and-abstract screening workflows in a preregistered study embedded in a conceptually complex scoping review. Methods. After a conservative title-only screen, 1,131 records were screened by one review lead, four trained assistants screening non-overlapping subsets, and seven complete LLM runs using different models and processing configurations, including a nominally identical repeat run. We compared retained workload, operational recall against 316 verified eligible records, agreement, run-to-run consistency, and procedural burden. Because eligibility was verified only for records advanced and assessed in the parent review, recall estimates were operational. Results. No workflow recovered all verified eligible records. The human workflows and two GPT-5.4 file-batch runs retained 42.2-45.0% of records while achieving 82.3-82.9% recall. Gemini 3.1 file batches achieved the highest recall (83.9%) but retained 56.7% of records. All-at-once configurations recovered fewer eligible records than corresponding file-batch configurations. Two nominally identical GPT-5.4 file-batch runs agreed on 91.7% of records but differed on 94 records, including 29 verified eligible records retained by only one run. Discussion. LLM screening performance depended on the implemented workflow, not model identity alone. Processing configuration, workload, record-level variation, and human-LLM decision integration are therefore substantive properties of deployed systems. For high-recall tasks, LLMs are better suited to validated, auditable, human-supervised workflows than autonomous exclusion.

**Key takeaways for the wiki:**
- Two nominally identical runs of the same model agreed on 91.7% of records but differed on 94 — including 29 verified-eligible records retained by only ONE run. Run-to-run variance is real and consequential.
- LLM performance depends on the workflow (file-batch vs all-at-once), not just model identity.
- For high-recall tasks (where missing something matters), LLMs belong in validated, auditable, human-supervised workflows — not autonomous exclusion.
- The re-run is the cheapest verification move: a second identical run catches what the first one dropped.
