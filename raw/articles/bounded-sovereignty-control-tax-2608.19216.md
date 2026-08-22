---
source_url: https://arxiv.org/abs/2608.19216
ingested: 2026-08-22
sha256: e3f6c0604760527ffc28ba15baf1972a6edf8350971331d6fdb61dd3e18ac6ee
---

# Bounded Sovereignty and the Control Tax: Pricing AI Oversight When the Deployer Does Not Own the Model

arXiv:2608.19216, 2026 (published 2026-07-06)

**Authors:** Zhen Wen Lim

**Full abstract:**

AI control research asks how to deploy models safely even when they may be misaligned, but many control protocols assume that the deployer can instrument the model and its surrounding pipeline. That assumption often fails for regulated organisations using frontier models through APIs or managed endpoints, where the deployer may control the business process but not the model weights, serving infrastructure, internal traces, update process, or full interaction logs. This paper introduces bounded sovereignty: partial technical and contractual access across the data, model, infrastructure, and interaction layers of the AI stack. It argues that these access conditions determine which control protocols can be executed in practice. The paper contributes a four-layer access typology, a protocol-by-layer requirements matrix, and the concept of sovereignty discount cost: the part of the control tax spent substituting for missing access through contracts, architecture, audit, vendor assurance, residual risk, or reduced system scope. It also reports a synthetic access-ablation experiment over 1.35 million synthetic case simulations and interprets the findings through an anonymised national-payments-infrastructure scenario. The experiment is not real-world payment-system evidence; it is a construct-validity exercise. The results show that complete logs improve diagnosis, a pre-execution gateway enables intervention, trace access and model-version control strengthen post-incident explanation, and scope restriction can improve safety while reducing usefulness. Control protocols proposed as general safety solutions should therefore state their access assumptions explicitly.

**Key terms:** bounded sovereignty · control tax · sovereignty discount · four-layer access typology · API deployment · oversight
