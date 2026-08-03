---
source_url: https://arxiv.org/abs/2607.29274
ingested: 2026-08-03
sha256: TBD
---

# Language Models Agree With Each Other, Not With Readers

arXiv:2607.29274, August 2026 (measurement study, 2,523 reader mark sets across 120 web documents)

**Full abstract:**

Claims that language models homogenise are usually measured against human judgements collected for the study, which makes the human side an artifact of the design: a crowdworker given the model's instruction is running the model's prompt. We measure convergence against a human reference nobody built for the purpose -- 2,523 reader mark sets across 120 web documents, produced by people highlighting for their own reasons on a platform where the overlay of others' marks is off by default.

Agreement is the overlap between two size-matched sentence sets minus the overlap expected when each is resampled within its own depth-and-length bands. The null's calibration is demonstrated, not asserted: every pair involving a random baseline lands within 0.006 of zero. On the median document each party names 14 sentences of 70; two readers share 4.1 and two models 8.7.

Across 18 model arms spanning 11 vendors, 3 countries and both weight regimes, the median of 153 model pairs is +0.093 against a human yardstick of +0.040, and 99 sit entirely above the human interval. Two frontier models from rival labs reach +0.203, twice what GPT-4o agrees with itself on a second call. The effect is not explained by style, vendor, or weight regime.

**Key terms:** model homogenisation · convergence measurement · reader marks · naturalistic human reference
