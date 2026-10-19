---
source_url: https://arxiv.org/abs/2610.22465
ingested: 2026-10-19
sha256: 51b4dbaf6d8f8a7c068c13d655a4f4ca2a3b7a93f9c3f2cffc8e74a74b5b7576
---
# Author-in-the-loop Agentic Reproducibility Auditing for a Machine Learning Conference

Publisher: arXiv (preprint, version 1)
Published: 2026-10-15
Authors: Yukun Dong, Linjun Zhang, Tian Zheng

## Publisher abstract (full text not reviewed)

Reproducibility checks during peer review require a shared understanding of what authors' code is expected to reproduce. We present an author-in-the-loop collaborative audit that makes author declarations explicit inputs to an AI agent's investigation and assessment. A structured checklist records reproduction instructions and limitations; a two-stage workflow on GitHub connects agent checks to author clarification, revision, and agent reassessment. The agent separately assesses whether results have been reproduced and whether authors need to provide clarification or make repairs, while human reviewers approve requests and decide whether concerns are resolved. We deployed the system across 36 conference papers and 133 experimental tables and figures, raising 20 issues after human review. Further checks supported closing all the issues, although full reproduction remained unverified in some cases. We further compared repeated audits with complete and blank checklists to examine how author declarations shaped the agent's investigation and assessment. Our work contributes a collaborative workflow and agent design that use author knowledge to guide reproducibility auditing. The conference deployment provides empirical evidence that this approach can help identify and address reproducibility problems through collaboration among authors, agents, and reviewers.

## Curator note (interpretation, not source text)

Conference deployment across 36 papers and 133 tables and figures used author checklists, agent investigation, author clarification, and human reviewer decisions; 20 issues were raised after review and later closed, while full reproduction remained unverified in some cases. Try a draft checklist of expected outputs and known limits before asking an assistant to audit public artifacts; closure is not proof of full validation.
