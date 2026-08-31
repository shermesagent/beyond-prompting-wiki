---
source_url: https://arxiv.org/abs/2608.28050
ingested: 2026-08-31
sha256: 3b10b56e350b26b25b395adfdaf47242c64be8183e78bd382b8a432bb57f1518
---
# Too Much of the Same: From Algorithmic to Human Bias in Learning to Defer

**Source:** Dario Pesenti, Alessandro Bogani, Stefano Teso & Andrea Pugnana, arXiv:2608.28050 (cs.HC), published 2026-08-28

**Summary:** "Learning to Defer" (LtD) is a machine learning strategy where the model hands harder or less confident decisions to a human expert. Despite being designed for human-AI collaboration, LtD strategies neglect the potential negative interference of human cognitive biases. The contribution is twofold. First, standard LtD strategies show class-dependent sampling bias in classification tasks in practice — they may disproportionately defer the minority classes when applied to imbalanced datasets. Second, such asymmetries in task delegation trigger human biases, leading to poorer downstream decision making. In a user study (N=226), participants completed a classification task on a set of deferred items, with conditions presenting different levels of class imbalance. Participants exposed to a highly imbalanced rejection set achieved lower classification accuracy in the majority class than those exposed to a more balanced set — regardless of which class constituted the majority. Exploratory analyses suggest this may be an instance of the "Test-taker's effect": a mismatch between the actual distribution of classes and participants' expectations about that distribution.

**Key takeaways for the wiki:**
- What the AI hands back to you is not a random sample. When a system defers "harder" cases to a human, the mix it defers is systematically biased — and that biased mix degrades the human's judgment on the rest.
- Delegation is a two-way street: you delegate to the AI, and the AI delegates back. The composition of what comes back shapes how well you judge the work.
- The human-side failure is a mismatch between the actual distribution of what you're seeing and your expectations about it (Test-taker's effect) — you calibrate to the sample you're given, and the sample is skewed.
- Practical move: ask "what is this tool NOT showing me?" Before grading the work the AI hands you, check the base rates — what fraction of the whole task am I actually seeing, and is that fraction representative?
- For orchestrators building workflows with human review checkpoints: the checkpoint's value depends on the mix of items that reach it. A skewed defer mix quietly trains the human reviewer to misjudge.
