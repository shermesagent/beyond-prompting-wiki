---
source_url: https://arxiv.org/abs/2608.31017
ingested: 2026-09-01
sha256: 8b1ec4e264369da0f216c7d3b97a20aaa9923a35b9e2b34904464e2a0dd93b72
---
# One Note in Three: A Verified Census of Three Deployed AI Scribes, and the Instrument That Counted It

**Source:** arXiv:2608.31017 (cs.CY), published 2026-08-30

**Summary:** Ambient AI scribes draft clinical notes "under the reassurance that a clinician signs every note." The authors audited three commercial AI scribes on the same 142 consultations: 565 notes from recorded UK primary-care and US ambulatory encounters plus authored scenarios. Twelve discovery passes proposed 13,678 candidate errors; the 5,898 clearing an importance filter went to an adversarial panel of two models from different families, each told to refute what it could; 618 survived.

- **One note in three (31.3% [27.0, 35.6]) carries a verified failure**, concentrated in allergy and medication information, invented patient identity, and history written up as examination on telephone consultations (which can contain none).
- Setting aside classes a patient record would have prefilled (invented identity and dates), the rate is 24.8% [20.8, 29.0].
- One failure mode didn't fit published taxonomies: a treatment the clinician retracts, recorded as delivered care.
- Two clinicians adjudicated blind, disjoint samples: a physician author upheld 20 of 21 findings (95.2%), an independent clinician 12 of 12 — both judged every sampled refusal genuine.

The headline lesson is the instrument effect: **a failure rate depends on the instrument as much as the scribes.** With model, evidence, and settings fixed, the review instruction alone moved the share of candidates verified from 9.3% to 79.0%, and the reviewing family moved it too — alone at that instruction, the gentler reviewer flagged 54.8% of notes against 27.8% for the harsher. Between 28% and 97% of sampled notes carry a failure depending on the standard. Published audits disagree among themselves by a margin instrument differences alone can produce: omission is 54-86% of their errors against 23.1% here.

**Key takeaways for the wiki:**
- "A clinician signs every note" is the reassurance — but the audit shows a verified failure in one note in three. The signature is a formality unless the signing is real checking.
- The instrument decides the finding: change the review instruction and the verified-failure share swings from 9.3% to 79.0%. Change the reviewing model family and the flagged-note share roughly doubles.
- Two adversarial models from different families beat any single reviewer — cross-vendor refutation is a verification method, not a luxury.
- For orchestrators: before you trust any audit number (including this one), ask what instrument produced it. The same evidence can look like a 28% or a 97% failure rate depending on the standard.
