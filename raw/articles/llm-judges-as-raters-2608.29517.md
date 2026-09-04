---
source_url: https://arxiv.org/abs/2608.29517
ingested: 2026-09-04
sha256: 9cf083659b6c707d390728f510f05e70403e8c6427d27f2b8cf4617a4559c8d8
---
# LLM Judges as Raters: A Pre-Registered Audit of Severity, Halo, Reliability, and Version Instability in LLM Essay Scoring

**Source:** arXiv:2608.29517 (Veerendra Kumar Sunkavalli), published 2026-08-30

**Summary:** LLMs are increasingly used as essay graders in learning analytics — and they are evaluated almost exclusively with agreement statistics. Educational measurement has long warned that human raters also differ in **severity**, show **halo**, and **drift as instruments**; this paper treats LLM judges as raters and runs a pre-registered rater-effects battery on public corpora in two languages (ENEM/Essay-BR; ASAP): 2,377 essays, 12 judges, 4 providers, 5 version contrasts, replicated cells, released as a score tensor.

Key findings:

- **Severity spans 219 points** on ENEM's 0–1000 scale; on ASAP the panel spread is **15–33% of the score range** — against a between-trained-human gap near 1%.
- **Judge-human correlations sit in an undiscriminating .47–.56 band** — enough to look reasonable in a correlation table, not enough to agree with a human grader on any particular essay.
- **All five version contrasts shifted severity** beyond a family-wise permutation null (up to 133 points), and one judge was deprecated mid-study, caught by identity canaries.
- Two pre-registered tests returned honest nulls: severity-adjusted leaderboard reversals did not survive a permutation null, and "silent drift" was refuted — agreement moved with severity in four of five contrasts.
- Replication yields self-consistency (φ ≥ .80 at k ≤ 2) but not human-level accuracy — the judges agree with themselves, not with humans.
- A same-instrument check overturned the paper's own halo comparison: matched on instrument and calibration, there is no credible evidence that judge halo exceeds the trained-human range.

**Bottom line:** an AI essay grader can be highly self-consistent and still be a different grader than any human — stricter by hundreds of points on some scales, unstable across model versions, and invisible to agreement statistics. If you grade with AI, calibrate the judge against human-scored anchors — and re-check whenever the model version changes.
