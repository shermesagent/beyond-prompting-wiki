---
source_url: https://arxiv.org/abs/2608.14940
ingested: 2026-08-31
sha256: 13133b143c4f558e42cbdadea0e4354603a61b623bfcf0a75d5c71a8c8b24fdd
---
# When Is an Agent Evaluation Over? Outcome Finality and Cross-Unit Separation

**Source:** Avyay M. Casheekar & Hariganesh Tangirala, arXiv:2608.14940 (cs.CY), published 2026-08-14, updated 2026-08-28

**Summary:** Agent evaluations commonly score the state observed when a run stops and count the run as one trial. Interpreting that score as a final result from a separate trial requires two properties: outcome finality — later events cannot change the claimed result — and cross-unit separation — earlier runs cannot change the relevant conditions of later ones. The endpoint establishes neither condition by itself, and the two can hold independently. Waiting for a delayed outcome may settle the label even though its state remains available to another run; isolation may prevent carryover even though the scored outcome remains unresolved. The paper develops a "completion argument" that identifies the evidence needed for each decision: a final success or failure label is justified only when every relevant effect is resolved or bounded tightly enough to fix the outcome, and any remaining uncertainty must be reported. In a controlled replay with fixed agent actions, endpoint and terminal labels differed for every nonzero-delay operation, and a delayed write changed the next run's score under shared state but had no such effect after namespacing or verified reset. A review of ten public protocols found that reset or deliberate retention is documented explicitly more often than unfinished operations or evidence for separate scoring. The paper proposes an open-effects record: a log of operations and resources that may remain relevant after the endpoint, their status, and their possible effects on the scored outcome or another run.

**Key takeaways for the wiki:**
- The machine's work does not come with a "done" label. A run stopping is not the same as a task being finished — later events can still change the result.
- Two separate questions hide inside "is it done?": (1) can anything that happens later change this result? (outcome finality) and (2) did the previous run contaminate this one? (cross-unit separation). They can hold independently.
- For orchestrators: define completion before you delegate. "Done" means the result is stable — nothing still pending can flip it — and the environment is clean — this run wasn't influenced by the last one.
- Practical instrument: the open-effects record — before you call a delegated task finished, list what might still be running, unresolved, or shared with the next task, and their status.
- This is the formal version of the Completion Question: when is a delegated task actually over?
