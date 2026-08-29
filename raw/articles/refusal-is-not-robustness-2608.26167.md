---
source_url: https://arxiv.org/abs/2608.26167
ingested: 2026-08-29
sha256: 684a9199aae63d031a7200b0e5aac5d5d038e40a6558852aa1f07d3b5a7d7f4c
---
# Refusal Is Not Robustness: Auditing Confident Fabrication in Large Language Models on a Provably Uninformative Clinical Pain Speech Transcript

**Source:** arXiv:2608.26167 (De & Pavuluri, 2026-08-28)

**Abstract:** Hallucination and abstention benchmarks rarely establish that a model could not have known the correct answer, making it difficult to distinguish appropriate abstention from an unsupported prediction. Seven large language models were evaluated on the TAME Pain speech corpus. Participants read phonetically balanced Harvard Sentences while one hand was immersed in cold or warm water and reported pain only during periodic pain statements. This protocol generated 5,750 no signal Harvard Sentence utterances whose transcripts contained no lexical pain information and 1,294 signal pain statement utterances in which the pain rating was explicitly spoken. In the no signal arm, pain was recoverable from acoustic features (AUC 0.622, 95% CI 0.553 to 0.662), whereas transcript based prediction was near chance (AUC 0.489, 95% CI 0.418 to 0.504). Because automatic speech recognition removes the acoustic pain cues, any pain score inferred solely from the transcript is unsupported by the available evidence. Under cooperative prompting, six models abstained on nearly all no signal transcripts, correctly extracted spoken pain ratings in the positive control task with accuracies ranging from 0.939 to 1.00, and maintained an expected calibration error of at most 0.100. Under authority framed prompts, abstention became prompt dependent, with the same model ranging from 0.18 to 1.00 across equivalent prompt phrasings. Most models produced low confidence estimates when forced to answer, whereas Gemini 2.5 Flash and Llama 3.1 8B consistently generated confident pain scores with confident fabrication rates of 0.53 and 0.76, compared with at most 0.15 for all other models. No significant demographic effects were observed in forced responses, with all p values greater than or equal to 0.20.

**Key takeaways for the wiki:**
- Abstention is a property of the *prompt environment*, not the model: the same model ranged from 0.18 to 1.00 abstention across equivalent authority-framed prompt phrasings.
- Under cooperative prompting, six of seven models abstained correctly on provably uninformative inputs — but authority framing switched abstention off.
- Forced to answer, two models confidently fabricated at 0.53 and 0.76 rates (vs ≤0.15 for others). Refusal is not robustness.
- The practice version: audit your prompts for authority framing; if you want "I don't know," the environment has to allow it.
