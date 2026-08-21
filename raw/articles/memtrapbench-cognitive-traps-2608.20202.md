---
source_url: https://arxiv.org/abs/2608.20202
ingested: 2026-08-21
sha256: 03c6178ad01d2be8d94c28896c545ddd37f01466cf4e6bcc56d7cb99dbe27a8a
---

# MemTrapBench: Benchmarking Cognitive Traps in LLM Memory Use

arXiv:2608.20202v1, 2026 (published 2026-08-20)

**Authors:** Mengru Wang; Haozhe Luo; Zhenqian Xu; Zhixiang Cui; Haoming Xu; Qu Yang; Jizhan Fang; Junfeng Fang; Ningyu Zhang

**Full abstract:**

Memory has become a key component of large language models, enabling them to retain information and learn from long-term interactions. However, existing memory benchmarks mainly evaluate whether information is correctly extracted, stored, and retrieved, while largely overlooking how retrieved memories reshape model reasoning and affect performance on the current task. We identify memory-induced cognitive traps: even faithfully recorded and semantically relevant memories can distort model reasoning or beliefs and degrade current task performance. To systematically evaluate these failure modes, we introduce MemTrapBench, which covers two forms of cognitive traps: Reasoning Fixation and Belief Distortion. Experiments across two model families and five representative memory frameworks show that MemTrapBench is challenging: all evaluated memory strategies underperform the no-memory setting, with even the strongest methods suffering drops of more than 10%. To mitigate these cognitive traps, we propose AdaptiveMem, a simple yet effective inference-time method that instructs LLMs to avoid memory traps. AdaptiveMem mitigates cognitive traps on MemTrapBench while preserving or improving performance on standard memory benchmarks across diverse memory frameworks.

**Key terms:** LLM memory · cognitive traps · reasoning fixation · belief distortion · no-memory baseline · AdaptiveMem
