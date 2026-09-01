---
source_url: https://arxiv.org/abs/2608.28631
ingested: 2026-09-01
sha256: fdbff87788e9f4c33e9ca475cc48a57b5f3afb34f152ce6ef6faba4a4d2cd27a
---
# CrossAudit: A Git-Native, Cross-Vendor Audit Loop for Agentic Science

**Source:** arXiv:2608.28631 (cs.CY), published 2026-08-28

**Summary:** "An AI scientist should not grade its own homework." In the systems the authors examined, the agent that reviews the work usually comes from the same model family as the agent that produced it — or at least from the same vendor. Model evaluators are known to favor their own generations; models trained alike may also share blind spots, in which case the reviewer inherits the author's. The record of what was flagged and what was waved through often sits in platform logs nobody outside can replay.

**CrossAudit** is a protocol for supervising autonomous research pipelines built on three commitments:

1. Each increment of work is audited by an agent from a **different vendor** against a rulebook a **human wrote and versioned**.
2. Reports, verdicts, disputes, and rulings are **git commits** — the supervision history can be re-read and cited.
3. Scripted checks run before any model does. Advisory judgment never gates the pipeline: **a model blocks only by citing a rule**, and no model may waive a deterministic failure. Blockers that survive a bounded number of revision rounds go to a person.

The protocol is stated as eight invariants, with a reference implementation built from GitHub Actions and a few hundred lines of Python, and a live deployment in a computational-chemistry pipeline. A seeded-defect trial (30 increments, 43 seeded defects) showed the two vendors read the same rulebook differently — not that either is better. The strongest evidence: the committed, uncontrolled record of cross-vendor audits of the paper itself, which voided the authors' own trial blinding.

**Key takeaways for the wiki:**
- The review-first pattern's independence requirement, made mechanical: reviewer must come from a different vendor than the producer, or the reviewer inherits the author's blind spots.
- The rulebook is human-written and versioned — the standard lives outside both models.
- "A model blocks only by citing a rule" — the veto is constrained to checkable grounds. No model can wave a deterministic failure.
- The audit history is a git log: you can re-read, cite, and learn from every past verdict.
- Same rulebook, two vendors, different readings — the cross-vendor difference is the signal; neither vendor's judgment alone is the standard.
