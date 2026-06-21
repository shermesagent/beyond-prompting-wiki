# Beyond Prompting Wiki — Schema

## Domain
A living, approachable wiki about **moving beyond prompting** — the shift from Phase 2 (templated prompting) to Phase 3 (autonomous agent orchestration). This wiki distills high-level research into plain-language concepts that help everyday professionals, educators, and managers build an **agentic mindset**.

This is **not** a technical manual. It's a learning companion — meet people where they are and guide them one concept at a time.

## The Core Idea: Operator → Orchestrator → Architect
| Phase | What You Do | The Mindset |
|-------|-------------|-------------|
| **Operator** (Phase 2) | Write prompts, iterate on output | "I tell the AI what to say" |
| **Orchestrator** (Phase 3) | Delegate tasks, chain tools, set constraints | "I tell the AI what to do" |
| **Architect** (Phase 3+) | Design agent systems, define workflows, build memory | "The system works even when I'm not there" |

Every page in this wiki should help someone move one step along this spectrum.

## Folder Structure
- `/Home.md` — front door, navigation, "start here for newcomers"
- `/00-Daily-Digests/` — daily research digests (YYYY-MM-DD.md)
- `/01-The-Shift/` — the core concept: what it means to go beyond prompting
- `/02-Key-Concepts/` — approachable distillations of research into learning concepts
- `/03-Real-World/` — stories, case studies, examples of the shift in action
- `/04-Barriers-and-Bridges/` — what holds people back + how to cross
- `/05-Practice/` — exercises, experiments, weekly muscle builders
- `/06-Glossary/` — plain-language definitions of key terms
- `/raw/` — immutable source material (articles, papers, transcripts)
- `/sources/` — structured metadata, JSONL source records

## Naming Conventions
- File names: Title Case with spaces, matching the page title (e.g., `The Operator Mindset.md`)
- Use `[[wikilinks]]` for internal cross-references
- Daily digests: `YYYY-MM-DD.md`
- Every page must link to at least 2 other wiki pages

## Page Template (Concept Pages)

```markdown
# Concept Name

## What It Is
Explain in one paragraph. Plain language. No jargon unless defined.

## Why It Matters for Moving Beyond Prompting
Connect directly to the operator→orchestrator shift.

## How to Spot It in Your Day
What does this look like in someone's actual workflow?

## Try This
A concrete, 5-minute exercise to feel the concept in action.

## Related Pages
[[Other Page]] · [[Another Page]]

## Tags
#concept #orchestrator #mindset
```

## Daily Digest Requirements
Each digest must include:
1. **Theme Title** — a one-line header that captures the connecting thread
2. **Executive Summary** — 2-3 sentences on the day's big idea
3. **Concepts Discovered** — new learning concepts added or updated
4. **Sources Found** — what was ingested, with key takeaways distilled
5. **For the Operator** — what a Phase 2 person can take away today
6. **For the Orchestrator** — what a Phase 3 person can apply
7. **Pages Created or Updated**
8. **Top Insight of the Day**

## Source Filtering Rules
- Accept: research, case studies, real-world workflows, frameworks, honest failure postmortems
- Reject: pure product marketing, hype without substance, alarmism with no practical insight, academic papers that haven't been distilled for a non-specialist

## Tag Taxonomy
- #concept — a core learning concept
- #mindset — a mental model or mindset shift
- #workflow — a practical how-to
- #barrier — something that holds people back
- #practice — an exercise or experiment
- #story — a real-world example
- #operator — relevant for Phase 2 thinkers
- #orchestrator — relevant for Phase 3 practitioners
- #architect — advanced agent design concepts
- #research — source material or studies
- #glossary — definition entry

## Update Policy
Each daily run must:
1. Save the daily digest to `00-Daily-Digests/`
2. Update at least 2 existing wiki pages with new findings
3. Create at least 1 new concept page if fresh material warrants it
4. Add accepted sources to `/sources/sources.jsonl`
5. Commit changes to Git with message `Beyond Prompting Wiki update — YYYY-MM-DD`

## Tone and Voice
- Warm but direct. Think colleague you respect, not professor lecturing.
- Non-threatening. No one is "behind" — everyone is on a path.
- Concrete over abstract. Every concept needs a "what does this look like at work" moment.
- Short paragraphs. Bullets and tables are your friends. Dense walls of text are not.
- Avoid acronyms without explanation. Avoid academic register.
- When citing research, lead with the practical takeaway, then the source.
