---
source_url: https://arxiv.org/abs/2610.21109
ingested: 2026-10-16
sha256: f9c8f74a7302565a3841ee3c135af29545acc29d2ca552d46db33faa6f1f741d
---
# Kolab: Benchmarking Human-Agent Collaboration in Long-Horizon Workflows

Primary source: https://arxiv.org/abs/2610.21109
Authors: Shirley Anugrah Hayati, Patricia Anugrah Setiani, Ruizi Wang, Zhouyi Li, Khanh Chi Le, Young-Jun Lee, Dongyeop Kang
Submitted: 2026-10-15 (preprint; peer-review not verified)
Retrieved from: arXiv API abstract, 2026-10-16

## Author abstract (whitespace normalized)

When humans collaborate with AI agents on long-horizon tasks, what happens to the agents' contributions? For solving long-horizon tasks, humans place greater importance on ongoing interaction with AI agents (e.g., revising plans) than on an agent's ability to complete the task in a single attempt. However, most agentic benchmarks have focused more on automation. Strong performance on such benchmarks does not imply effective real-world collaboration. Professional workflows offer a useful setting, as they often involve interdependent steps. To address this gap, we introduce Kolab, a new dataset of 115+ hours of screen recordings of 50 professionals from 40 occupations collaborating with agents on realistic, long-horizon problems. Kolab also contains participants' collaboration and output quality judgments. Our analysis reveals diverse collaboration patterns, highlighting the importance of when and how professionals coordinate with agents. A collaborative agent must do two things that automation benchmarks never test: anticipate whether experts will adopt, modify, or reject its contribution once it leaves the chat window to guide its next steps, and assess collaboration quality from the unfolding workflow without constant expert feedback. Our benchmark operationalizes both: (1) forecasting how professionals use agent contributions at diverse workflows, and (2) verifying their judgments of collaboration satisfaction and output quality. Findings show that frontier models, both agentic and non-agentic, overestimate collaboration with experts and struggle to distinguish between high- and low-quality collaboration. Longer workflow context does not consistently improve these predictions. As frontier agents cannot yet understand long-horizon collaboration with experts, we position Kolab as a valuable dataset for studying human-agent collaboration grounded in real professional workflows.

## Beyond Prompting takeaway (curator interpretation)

After a task, record whether you used, changed, or rejected the AI contribution; a completed draft is not the same as a useful collaboration.

Evidence limit: The exercise is a suggestion, not a tested district intervention. The abstract, not full text, was reviewed.
