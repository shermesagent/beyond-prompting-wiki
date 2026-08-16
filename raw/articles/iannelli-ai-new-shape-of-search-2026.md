---
source_url: https://arxiv.org/abs/2607.04282
ingested: 2026-07-07
sha256: dd72f9b566cb38d7526164fef3cb951ab3b5faad0bba90ee5654f1e9842ef26d
---

# The New Shape of Search: How Conversational AI Recomposes Information Seeking

**Authors:** Michael Iannelli, Alan Ai
**Date:** July 7, 2026
**Source:** arXiv:2607.04282 (cs.HC, cs.CY, cs.IR)

## Abstract

Classic models cast information seeking as iterative foraging: formulate a keyword query, scan results, reformulate, gather across sources, synthesize. The authors ask what happens when a conversational assistant is inserted into that episode. Linking real conversations with major assistants to the same users' searches and browsing in an opt-in cross-surface panel, and reconstructing the full episode rather than a single query, they find conversational AI changes the shape of information seeking, not merely its volume.

**AI episodes bifurcate.** Most terminate in place, with no onward search or content step in the observed trace, while roughly a third scaffold into longer multi-step journeys. Which shape occurs is governed less by task type than by articulation: collapse is statistically indistinguishable across lookup, learning, and comparison episodes, yet falls monotonically with opening-ask length, from 72% at 1-3 words to 48% beyond 20.

Roughly two-fifths of assistant episodes are workbench use — drafting, coding, editing — not information seeking at all, and these collapse most. Conversational AI also does not displace search: search remains woven through roughly three-quarters of within-episode transitions, after reading a page users return to the search box over the assistant 70/30, and within-user search share does not fall.

**Verification is rare.** Searches with explicit verification language follow roughly 1% of episodes, and citation-forward interfaces do not measurably increase checking.

## Key Findings

- **Collapse pattern (majority):** AI answer → user stops. No further search, no content visit, no synthesis
- **Scaffold pattern (~1/3):** AI answer → user continues searching, reading, building. AI is the starting point, not the destination
- **Workbench use (~40%):** Drafting, coding, editing — not information seeking. These "collapse" most often (user gets the draft and stops)
- **Articulation matters:** Longer opening asks (20+ words) are much less likely to collapse. The more you put in upfront, the more you get out downstream
- **Verification gap:** 1% of episodes include explicit verification. Nobody checks the AI's work
- **Search persists:** AI doesn't replace search — users still search 75% of the time within episodes
