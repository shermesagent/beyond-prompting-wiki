---
source_url: https://arxiv.org/abs/2608.29055
ingested: 2026-09-01
sha256: 748dc45be2f038bb6baaf692e9a98debdad6953f5a51f46448153c7341f0a427
---
# Why Organizational Rules Fail AI: O-I-B-A-R and the Externalization of Decision Boundaries

**Source:** arXiv:2608.29055 (cs.CY), published 2026-08-29

**Summary:** AI systems enter organizations through policies, procedures, playbooks, prompts, and other explicit representations of work. Yet formal descriptions often differ from situated practice. The paper argues that a recurring class of organizational AI failures is partly a **knowledge representation problem**: the AI receives the procedure, while the organization operates on the procedure *plus* negative boundaries (what the rule doesn't cover), runtime judgments (when experts quietly deviate), responsibility assignments, and learning history. Captured know-what omits the contextual know-how experts use when judgments are uncertain.

The authors introduce **O-I-B-A-R** (OPEN, IS, BUT, ACTION, RESULT), a scaffold for externalizing the missing decision boundaries:

- **OPEN** — when a rule applies at all (the triggering condition)
- **IS** — records when a judgment holds (the positive condition)
- **BUT** — records a concrete failure containing information *beyond* the logical negation of IS. Comparable success and failure cases are decomposed toward a minimally sufficient changing variable, which becomes a value-bearing decision dimension.
- **ACTION** — what to do in the current state
- **RESULT** — confirms a boundary, shifts a threshold, or exposes a new dimension

A **suspension** represents the state where a dimension is known to matter but its current value is unresolved — specifying what must be measured, asked, retrieved, or escalated to a human. Incidents can generate new dimensions; unresolved values define human-AI handoffs; feedback expands the decision space.

The paper also identifies a sociotechnical tension: durable and attributable failure histories can suppress the candor on which useful boundary knowledge depends. Externalization must be designed as an organizational intervention with real costs and incentives — people only share their failure knowledge if doing so doesn't hurt them.

**Key takeaways for the wiki:**
- The written rule (prompt, SOP, playbook) is a lossy copy of the job. The organization runs on procedure + negative boundaries + runtime judgment + learning history — most of which never makes it into the prompt.
- This is why "just write a better prompt" hits a ceiling: no prompt can hold the know-how experts use when judgments are uncertain. The fix is externalizing the boundaries — naming the conditions, the exceptions, and what to do when a value is unresolved.
- The BUT clause is the gold: a concrete failure contains more information than "not this." Compare success and failure cases to find the one variable that changed — that variable is a decision dimension worth tracking.
- Suspensions are the design object for delegation: when a dimension matters but its value is unknown, the rule should say what to measure, ask, retrieve, or escalate — not guess.
- The candor problem: teams only reveal the failure knowledge that makes rules work if disclosure is safe and rewarded. Externalizing decision boundaries is an organizational intervention, not a documentation exercise.
