---
source_url: https://arxiv.org/abs/2609.04679
ingested: 2026-09-07
sha256: 3e5dacab32111d43eb611707aa6c4c4820ff147f3daff8fbfbbfd2600d9267fe
---
# Beyond Prompt-to-App: Accountable Translation in Teacher-Facing Agentic Authoring

**Source:** arXiv:2609.04679 (Kadir, Liow, Khan & Ang), published 2026-09-04. Preprint; not peer reviewed.

**Summary:** Natural-language app builders let domain experts (teachers) create software by describing it. But their pipelines **transform professional intent** across four stages: compilation, generation, checking, and approval. This bounded trace study of a teacher-facing agentic authoring system found the transformations are where intent gets lost:

- **Compiled specifications added governance requirements** the teacher never asked for, and downstream representations sometimes **normalized case-specific learning relations** — flattening the teacher's actual classroom nuance.
- **Two drafts met a stored package/security threshold despite analyzer reservations and unresolved correspondence to their briefs.** The checks passed; the brief was not met. Passing the pipeline's gates ≠ the artifact does what the teacher wanted.
- **Four attempts in one account produced no usable payload**, and **repair messages did not translate internal terms into domain-legible revisions** — when the system tried to explain what went wrong, it spoke system-language, not teacher-language.

The paper's contribution is the framework of **accountable translation**: making consequential changes (1) **attributable** (who/what changed the intent), (2) **inspectable** (the change is visible), (3) **scoped in validation** (checks validate what actually matters, not just stored thresholds), and (4) **contestable** (the domain expert can push back and be understood). It extends HCI's traceability and end-user debugging work by locating professional authority across technical and organizational handoffs.

**Bottom line:** "prompt-to-app" is not the end of the beyond-prompting story — it is the next chapter. When a domain expert builds with natural language, the pipeline between intent and artifact must be accountable: every change attributable, inspectable, validated against the brief, and contestable in the expert's own language.
