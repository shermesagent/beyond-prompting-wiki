---
source_url: https://arxiv.org/abs/2611.19777
ingested: 2026-11-17
sha256: f0762904c7090506cbabb86131a2db1374dc3a06a32ccaf289d452a5b64d72fd
---
# Who May Release, Who Must Repair: Separating Authorization from Report Accountability in Personalized Services

Source: https://arxiv.org/abs/2611.19777
Authors: Chang Xu, Junyuan Tan
Published: 2026-11-15; arXiv preprint. Captured from the publisher abstract, not a full-paper appraisal.

Abstract (publisher): Personalized services often rely on different parties to compute results and decide whether data permissions and service policies allow delivery. The computing party's report may omit permitted inputs, leaving the delivery party to decide whether to wait for correction. Requiring correction first can delay service despite valid input permissions. Delivering first instead requires preserving responsibility for the incomplete report. We design an interface that checks input permissions separately from reporting requirements and records who must correct omissions and who may verify corrections. We evaluate three implementations on scripted histories and generated cases against a design treating omissions as authorization failures. When policy permits delivery before correction, our interface releases results that the alternative withholds while preserving repair assignments. These assignments remain in force through policy changes, so changing delivery rules does not erase earlier obligations. The interface makes the basis for release and outstanding repair responsibilities traceable across cooperating parties.
