# Failure-Path Preservation

**Failure-path preservation is the property of a knowledge system that records what *didn't* work — dead ends, failed approaches, wrong assumptions, corrected claims — alongside what did. Without it, every person, every agent, every project starts from scratch, doomed to repeat mistakes because the record of prior failures evaporated.**

Most systems for capturing knowledge are built to preserve success. A published paper reports what worked. A GitHub repo shows the current state of the code. A Google Doc shows the latest version. The five approaches that didn't work, the dependency that broke everything, the prompt format that produced plausible-sounding nonsense — invisible. At best, they appear in a "limitations" paragraph. At worst, they evaporate.

The term comes from Saboia Moreira & Sweet (arXiv:2607.24759, July 2026), who formalize failure-path preservation as one of three emergent sociotechnical properties of the llm-wiki pattern — an interlinked knowledge base co-maintained by humans and AI agents. The other two are **agent honesty** (the substrate as impartial record, not promotional output) and **appropriation** (humans and agents jointly shaping the knowledge base over time). Together, these three properties make the substrate a compounding asset rather than a disposable scratchpad.

## Why It Matters for Moving Beyond Prompting

The operator writes a prompt, gets an output, and moves on. If it didn't work, they try something else — but they don't record what they tried or why it failed. Next time the same task comes up, they start from zero.

The orchestrator maintains a failure record. When a delegation fails, they capture: what they asked for, what they got, what was wrong, what they changed. The next time that delegation comes up — for them or for anyone else using their workflows — the failure path is visible. The system gets smarter with every failure instead of repeating them.

This connects directly to [[Cognitive Fixed Cost]]: the upfront investment in a workflow pays off only if the workflow's failure paths are preserved. If every person who runs a pipeline has to discover the same failure modes independently, the cognitive fixed cost was never actually paid — it's being paid over and over by different people. Failure-path preservation is what makes the upfront investment compound rather than leak.

## In Plain Language

You've had this experience: you spend an hour trying to get something to work in AI. Three different approaches fail. The fourth one works. You finish the task and move on. Three weeks later, the same task comes up. Do you remember which approach worked? Probably not. Do you remember which three didn't? Almost certainly not. So you spend another hour rediscovering what you already learned. That's the cost of no failure-path preservation.

The fix is embarrassingly simple: when something doesn't work, write down what you tried and what happened. Put it where you'll find it. Date it. Next time, read the log before you start. That's it. A single markdown file called "What Didn't Work" with dated entries. The operator thinks "I'll remember." The orchestrator knows they won't.

## The Everyday Version

1. When something doesn't work, write down **what you tried**, **what happened**, and **when**.
2. Put it somewhere you'll find it the next time you face the same problem.
3. When you fix it, add the fix and the date to the same entry.

The tool doesn't matter — a markdown file, a Notion page, a text file in your project folder. What matters is the *preservation of the negative result.* Every failure path preserved is a failure someone doesn't have to repeat. Over time, that's the difference between an organization that learns and one that loops.

## Related Pages

[[Cognitive Fixed Cost]] · [[Memory]] · [[Memory as Infrastructure]] · [[Delegation Thinking]] · [[Small Business Automation]] · [[The School District Shift]]

## Tags

#glossary #orchestrator #substrate #memory #concept
