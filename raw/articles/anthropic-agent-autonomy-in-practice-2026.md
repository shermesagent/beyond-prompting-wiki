---
source_url: https://www.anthropic.com/research/measuring-agent-autonomy
ingested: 2026-10-03
sha256: b13c9f8f32fbebd6c23d77e356b48631eb6cd0f95d9df630adaa187c7c6f4cca
---
# Source note: Measuring AI agent autonomy in practice

Anthropic, published 2026-02-18. Primary provider analysis of millions of interactions across Claude Code and its public API, using privacy-preserving aggregation. In Claude Code, full auto-approve appears in roughly 20% of sessions among newer users and more than 40% among experienced users; interruption rates also rise from roughly 5% to 9% of turns with experience. On the most complex tasks, the agent asks for clarification more often than humans interrupt it. The authors caution that longer turns are an imperfect measure of autonomy, API traffic cannot be reconstructed as full sessions, and these are observations from one provider, not causal proof that more autonomy is safer. Practical translation: grant freedom only where a stop path and independent check remain available. This source is older than today's curation; not a new October publication.
