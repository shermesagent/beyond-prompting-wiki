---
source_url: https://arxiv.org/abs/2608.04830
ingested: 2026-08-06
sha256: 4e47998562cd17712363d84036c42d600dd377edd2784eacde8ef40cc292a7ae
---

# ContextWeave: A Real-World Workflow Benchmark

arXiv:2608.04830, August 2026 (benchmark; 14 participants, 1,005 executable tasks, six memory components)

**Full abstract:**

Memory is essential as language agents move from isolated tasks to long-horizon, stateful workflows, yet existing evaluations often reduce it to retrieval or question answering. We introduce ContextWeave, a longitudinal benchmark that evaluates whether recalled experience improves downstream agent performance in realistic office-work streams. ContextWeave reconstructs privacy-preserved, multi-month workflows of 14 participants into 1,005 executable tasks, including 568 core evaluation tasks, with instructions, containerized environments, trajectories, and task-specific rubrics. It measures workspace quality and alignment with participant-specific preferences, complemented by diagnostics of relevance, continuity, solvability, and robustness to misleading recall. Across six memory components under a fixed model, the strongest configuration raises Workspace Score from 68.08 to 78.20 and Preference Score from 41.50 to 70.60. With a fixed memory component, recall improves both outcomes for all five tested base models, although gains vary substantially. Our analysis shows that actionable, experience-rich memory supports workflow continuation and reduces redundant exploration more effectively than compact summaries, while it can also be more susceptible to misleading recall. These findings motivate memory systems that optimize not only retrieval relevance but also reliable use during execution.

**Key terms:** agent memory · longitudinal benchmark · real-world workflows · workspace quality · preference alignment · misleading recall · experience-rich memory
