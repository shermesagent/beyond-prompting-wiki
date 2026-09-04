---
source_url: https://arxiv.org/abs/2609.02149
ingested: 2026-09-04
sha256: d55741618d59eb80ee2f73922aa0b8cd84020ac12d84c15cfc5436899d39dd37
---
# OmegaUse-SOP: SOP Engineering for Professional Computer Use from Human Demonstrations

**Source:** arXiv:2609.02149 (Xiao, An, Yang, Ma, Chen, Cao, Zhao, Wang, Liu, Bao, Zhou & Wu), published 2026-09-02

**Summary:** Professional standard operating procedures (SOPs) remain hard for GUI agents because they involve implicit domain knowledge, software-specific conventions, and task-level verification requirements. The paper introduces **OmegaUse-SOP**, a human-in-the-loop **SOP Engineering** system for turning human demonstrations of professional computer use into reusable agent skills — explicitly analogized to prompt engineering, but instead of refining words, SOP Engineering iteratively refines demonstrations, execution rules, and domain knowledge.

The system has four modules:

1. **Observe** — records expert operations as multimodal GUI traces.
2. **Reason** — abstracts low-level events into semantic, step-level instructions.
3. **Configure** — incorporates domain rules and task-specific parameters.
4. **Execute** — runs the resulting skill in a live GUI environment through step-wise grounding, action generation, and verification.

Tested with a power-sector client on photovoltaic simulation workflows in PVsyst 7.2, OmegaUse-SOP improved GUI-agent reliability on professional SOP tasks.

**Bottom line:** a written SOP is a lossy copy of expert know-how — the implicit decisions, the software conventions, the "you just know when it's wrong" moments. Capturing a **demonstration** instead (or alongside) preserves the parts words lose. For anyone handing a recurring task to an agent: showing the machine once may beat describing the job a hundred times.
