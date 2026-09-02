# Failure-Path Preservation

## What It Is

The property of a knowledge system that preserves what *didn't* work — dead ends, failed approaches, wrong assumptions, corrected claims — alongside what did. Without failure-path preservation, every agent deployment, every workflow, every knowledge project starts from scratch, doomed to repeat the same mistakes because the record of prior failures evaporated.

The term comes from Saboia Moreira & Sweet (2026), who formalize it as one of three emergent sociotechnical properties of the llm-wiki pattern (an interlinked knowledge base co-maintained by humans and LLM agents). The other two properties are **agent honesty** (the substrate as impartial record, not promotional output) and **appropriation** (humans and agents jointly shaping the knowledge base over time).

## Why Standard Channels Can't Do This

Publications and code repositories structurally cannot preserve failure paths:

- **A published paper** reports what worked. The five approaches that didn't work — the data pipeline that crashed, the model that converged to a wrong answer, the prompt format that produced plausible-sounding nonsense — are invisible. At best, they appear in a "limitations" paragraph that omits the details.
- **A GitHub repository** shows the current state of the code. The commits that got reverted, the architecture that was abandoned, the dependency that broke everything — they're there if you dig through history, but they're not *preserved* in any structured, searchable, learnable form.
- **A Google Doc or Notion page** shows the latest version. The previous versions are buried in version history that nobody checks.

In all three channels, the failure path — *we tried X, it failed because Y, we switched to Z* — evaporates. The next person who encounters the same problem has no way to know it was already encountered and abandoned.

## What It Looks Like in Practice

The "Beyond Memory" paper's most striking demonstration: a two-author project using the llm-wiki pattern reported two experiments as having 20-of-20 evidence-based answers. A retroactive audit — possible because every claim in the wiki was linked to its supporting evidence — exposed that only 14 and 12 answers were actually evidence-based. The fix brought both to 18-of-20.

Without failure-path preservation, the overclaim would have stood forever. With it, the audit was possible, the correction was made, and — critically — **the full path from overclaim to audit to correction is preserved for anyone who comes after.** The next researcher sees not just "here's the corrected answer" but "here's the original claim, here's what was wrong, here's when and why it was fixed."

## The Operator vs. Orchestrator Difference

| | Operator | Orchestrator |
|---|----------|-------------|
| Records | Only what worked | What worked AND what didn't, with date and reason |
| Process memory | In their head (evaporates when they leave) | In the substrate (persists across personnel changes) |
| Failure visibility | "We used to do it differently" — vague, untraceable | "Tried X on 2026-03-15, failed because Y, switched to Z on 2026-03-22" — specific, searchable |
| What compounds | Nothing. Each cycle is independent. | Every cycle starts smarter than the last one. |

## The Everyday Version

You don't need a wiki or a formal knowledge base to practice failure-path preservation. The minimum viable version:

1. When something doesn't work, write down **what you tried**, **what happened**, and **when**.
2. Put it somewhere you'll find it the next time you face the same problem.
3. When you fix it, add the fix and the date to the same entry.

That's it. A single markdown file called "What Didn't Work" with dated entries. The important property isn't the tool — it's the *preservation of the negative result.* The operator thinks "I'll remember what went wrong." The orchestrator knows they won't, and builds a substrate so they don't have to.

## Related Pages

[[06-Glossary/Failure-Path Preservation|Quick reference]] · [[02-Key-Concepts/Cognitive Fixed Cost|Cognitive Fixed Cost]] (the upfront investment — failure-path preservation is one of the things the investment buys) · [[Doom Researching]] (the consumption pattern where nothing persists — the opposite of failure-path preservation) · [[Task Decomposition]] (breaking work into delegable units — the substrate records what each unit learned) · [[Delegation Thinking]] (deciding what to delegate — failure paths inform future delegation decisions) · [[Small Business Automation]] (concrete example of what a bakery loses without failure-path preservation) · [[The School District Shift]] (concrete example at institutional scale) · [[The Failure Review]] (what to do with the preserved failure when one slips through — blameless review)

## Source

Saboia Moreira, P. & Sweet, C.R. "Beyond Memory: A Templated Substrate for Heterogeneous Collaborative Knowledge Work with LLM Agents." arXiv 2607.24759 (July 2026). Three deployed case studies of the llm-wiki pattern; formalizes failure-path preservation, agent honesty, and appropriation as emergent sociotechnical properties.

## Tags

#concept #orchestrator #substrate #memory #failure-path-preservation
