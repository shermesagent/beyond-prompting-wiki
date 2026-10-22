---
source_url: https://arxiv.org/abs/2610.29216
ingested: 2026-10-22
sha256: 3aeca0c7c0281488a69958591379c2c10529061c671404cbddbf6c501e70ea30
---
# Preference Is Not Permission: Personalizing the Auto-Purchase Line in Agentic Commerce

Publisher: arXiv RSS, version 1; announced 2026-10-22
Authors: Ryotaro Shimizu, Sai HtaungKham, Mo Fan
URL: https://arxiv.org/abs/2610.29216

## Publisher abstract (RSS markup and whitespace normalized)
Personalized shopping benchmarks ask which item fits the user; we ask how far an agent may commit on that item, and pose learning the individual's auto-purchase line as a task. The boundary is evidence-conditioned and three-valued: whether committing is appropriate depends on the sufficiency of product information (warrant), reversibility, price against the user's norm, and urgency, not only on fit; and the natural output is don't buy, confirm first, or buy automatically. Across sixteen instruction-tuned models, autonomous commitment is misaligned with a human authorization reference in which fifteen annotators, role-playing the delegating principal from a given profile, choose the furthest action they would allow without confirmation: models commit even when fit is low and when their own evidence flag reports the warrant missing. This is overreach. The line is individual: these raters disagree, yet the disagreement is structured and partly predictable from a person's own other labels. A shallow learner on a few dozen of a person's own labels predicts their held-out auto-purchase line at a median of 0.79 by 30-40 labels, outperforming every evaluated prompt×model configuration, including a per-annotator oracle over 80 configurations; the learned boundary does not transfer across domains. We release the counterfactual benchmark, human authorization reference, and annotation protocol after acceptance.

## Curator reading boundary
Publisher RSS abstract and arXiv title inspected; full text not appraised. The 15 annotators role-played from profiles, not live purchasers; the benchmark is not evidence that any deployed shopping agent made real unauthorized purchases.
