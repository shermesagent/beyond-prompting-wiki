---
source_url: https://arxiv.org/abs/2608.27309
ingested: 2026-08-29
sha256: 651018e7431da24fdda24b5537337fea7d94c714d79519ba3a1b07e675380f51
---
# Difference-in-Differences on a Censored Rating Scale Can Manufacture an Effect: Evidence from a Pre-Registered LLM-Judge Audit

**Source:** arXiv:2608.27309 (Fan, Deng, Xu, Xie, Li & Zhang, 2026-08-28)

**Abstract:** Audits of LLM judges certify a bias by contrasting matched conditions, and the strongest designs difference twice: a within-item contrast between two candidate responses, differenced again across a manipulated attribute, read off a bounded rating scale. We show that this endpoint is not identified on the scale that reports it. Each term of the double difference is censored by its own share, so the observed statistic confounds differential preference with differential attenuation: a severity shift common to both responses manufactures an interaction whenever the two censor it unequally, as unequal distances from the bounds make them, exactly where good stimuli place them. We exhibit the failure inside a pre-registered audit of a frozen pedagogy judge, sealed before the first of its 990 calls. The registered primary endpoint, the effect of a stated learner profile on the judge's scaffolding preference, is null: +0.085 points (95% BCa [-0.167, +0.353], p = 0.684). The audit's one nominally significant interaction, +0.378 (p = 0.002), is not identified as preference: a construction containing zero differential preference reproduces 79 to 85% of it from the observed severity shift and the scale floor alone. We derive the mechanism in closed form and show that its contribution is measurable from an audit's own ratings.

**Key takeaways for the wiki:**
- The instrument that audits the judge can itself manufacture the effect it was built to detect: a bounded rating scale censors both sides of a double difference, and unequal censoring fabricates an interaction.
- Zero-preference constructions reproduce 79-85% of a nominally significant result — the audit's "significant" finding is scale artifact, not preference.
- Pre-registration caught it: the sealed primary endpoint was null; only the unsealed interaction was "significant."
- The practice version: before you trust an evaluation of your agent's outputs, ask whether the instrument was pre-registered, whether the endpoint is sealed, and whether the rating scale is bounded near the compared items. The judge's audit needs its own audit.
