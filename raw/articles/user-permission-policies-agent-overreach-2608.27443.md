---
source_url: https://arxiv.org/abs/2608.27443
ingested: 2026-08-28
sha256: 0bc5691b2f6001dabcee9de8e061187d7b2d871afe107728cc0a86934a6f1fe1
---
# Do User-Authored Permission Policies Improve Protection Against AI Agent Overreach?

**Source:** arXiv:2608.27443 (cs.HC)

**Abstract:** AI agents are poised to become a primary interface to digital products, acting across email, files, payments, and personal data. People without professional software backgrounds need understandable, reusable ways to control actions across services. We examine a mechanism in which a language model maps actions to plain-language consequence categories with user-authored "allow", "ask", or "never" rules. We ask what is gained and lost when decisions are made in advance as reusable rules rather than separately for each action. We analyzed 113 participants without professional software backgrounds across three conditions: per-action human-in-the-loop approval (HITL), automated per-action model review (AUTO), or user-authored consequence policy (POLICY). Participants judged 2 examples in each of 4 consequence categories; POLICY participants then set one rule per category. All supervised an 18-action simulated day, including 7 overreach actions. POLICY blocked less overreach than HITL (-20.1 percentage points, 95% CI [-32.1, -8.1]) and AUTO (-14.5 points, 95% CI [-25.8, -3.2]). POLICY lowered runtime prompts from 18.0 to 10.9, but total intervention time was not reliably lower when rule setup was included. Exploratory analysis showed that participants chose "ask" for 114 of 140 POLICY rules, returning most overreach actions to runtime. Of the 148 overreach actions executed in POLICY, 133 followed human approval and 15 ran automatically under "allow" rules. Across all 7 overreach actions, POLICY had the highest approval rate. Counterintuitively, user-authored rules did not by themselves provide stronger protection: many actions outside users' original requests went through after users approved them. These results reveal a gap between preference and commitment: repeatedly choosing "ask" preserves case-by-case choice but prevents a standing policy from settling decisions in advance.

**Key takeaways for the wiki:**
- Deciding in advance (a standing policy) can be WORSE than deciding at runtime if your rules are all "ask": users chose "ask" for 114 of 140 rules, which just returns the decision to runtime — with no real protection gained.
- "Ask" is the comfortable default and the trap: it preserves case-by-case choice but prevents a standing policy from settling anything in advance.
- The gap between preference and commitment: 133 of 148 overreach actions followed human approval — people approved actions outside their original request in the moment.
- The practice version: your delegation line (allow / ask / never) must be drawn in advance, and "ask" must be reserved for genuinely ambiguous cases — not used as a dodge.
