---
source_url: https://arxiv.org/abs/2610.35483
ingested: 2026-10-27
sha256: 32a11fa11d5d4fb68b419df7d702824d58904f050279ad9c161c4fa56dcb8bef
---
# Visible Reasoning: User-Facing Decision Transparency for Generative AI Systems

Publisher: arXiv (v1 preprint; publisher RSS abstract and Atom metadata)
Submitted: 2026-10-26; announced: 2026-10-27
Authors: Sanjay Krishna Anbalagan, Xinrui Nie, Anughna Kommalapati, Vijay Kumar Kanamarlapudi, Sreekanth Radhakrishnan, Xiaodan Zhao, Umesh Mohan

## Publisher abstract (retrieved from arXiv RSS)

Across multiple waves of computing, public trust in new technology has followed the emergence of governance mechanisms that made dominant risks legible and manageable. Generative AI shifts this pattern: these systems synthesize across heterogeneous sources, and users increasingly experience them as reasoning systems. The central question changes from "did it perform correctly?" to "can we trust how it arrived at its conclusion?"
  This paper introduces Filtered Decision Logs (FDLs), a user-facing transparency mechanism that makes decision formation visible without exposing raw chain-of-thought. FDLs pair each response with (i) a concise decision rationale, (ii) influence-ordered supporting data points derived from tool outputs, and (iii) relevance indicators showing which sources most shaped the conclusion. To operationalize evidence selection, we propose a trace-based method that reconstructs observability telemetry into a provenance tree and ranks evidence using four deterministic semantic and structural signals - Final Answer Similarity, Average Relevancy, Persistence, and Structural Proximity - combined via adaptive weighted scoring. We demonstrate FDLs across three domains: career advising (5 tools), investment analysis (4 tools), and travel planning (4 tools). In a formative evaluation with 50 participants (25 students, 25 working professionals in AI development), 92% rated the influence-ranked evidence as helpful for understanding and trusting the system's recommendation. Counterfactual tool-removal experiments confirm that removing the top-ranked source changes the answer more than removing a low-ranked source, validating that the ranking tracks decision dependence. We conclude that evidence-ranked transparency helps users identify misleading signals and missing context, enabling more confident acceptance, correction, or re-run of system decisions.

## Curator translation (not a tested intervention)

Ask for a short decision note with the exact source passage and what would change the recommendation. Open the cited source yourself. Perceived helpfulness among 50 people is not a measured improvement in factual accuracy or proof that the ranking is safe in a school setting.
