---
source_url: https://arxiv.org/abs/2610.12125
ingested: 2026-10-09
sha256: bc00051c6852bf44407c9b59cb4c5db4c0d57b2edc8cb5f4ef3c9c9be06730b5
---
# The learner who does not learn: when optimizing a pedagogical metric degrades LLM tutoring

Authors: Daniel Domínguez Figaredo, Rafael Fernández De la Cruz. Submitted 2026-10-08; announced in October 9, 2026 arXiv RSS (new preprint). Source: https://arxiv.org/abs/2610.12125

Primary abstract (verbatim except whitespace normalization): It is assumed that a natural way to improve the pedagogical quality of large language model tutors is to define a metric of instructional performance and fine-tune the model against it. To test this strategy, we designed a metric of pedagogical adaptivity that scores each instructional decision in a learning sequence against the conditions of the learning situation, which is the standard used for automated pedagogical scoring. We audited a frontier tutor across 2,000 learner scenarios, corrected its weakest cases by fine-tuning an open-weights proxy, and asked 31 trained educators to rate the pedagogical alignment of the outputs blind, before and after correction. The metric increased from +0.05 to +0.42 for the corrected cases, while the expert ratings decreased from 4.46 to 3.03, with the unmodified controls remaining unchanged and a base-proxy control ruling out the change of model. The tutor performed worse because any metric that scores decisions independently and averages them is maximized by repeating the single best decision, and the fine-tuned model collapsed to that exact optimum in every case, in and out of sample. Educators identified the repetition, which such metrics cannot represent, and preserving the learner's trajectory in the score reduced, but did not reverse, the metric's verdict. Weight analysis traced the correction to the model's output projection, where it had memorized its training strings rather than learned to adapt. We conclude that measurement validity does not imply optimization validity, and we derive design principles for benchmarks that assess or train AI-tutor instruction.

Practical translation (editorial, not a tested intervention): A higher per-turn tutoring metric coincided with lower blind educator ratings in a controlled study; check the sequence.
