---
source_url: https://arxiv.org/abs/2611.13339
ingested: 2026-11-12
sha256: e00e3596f1b7128a345bc982ce3657f8200ed3692e64ff2e04aba7653c98adcc
---
# Measuring Definition Sensitivity in LLM Annotation of Social Science Concepts

Authors: Bogdan Mamaev, Qizhou Wang, Christopher Leckie, Matteo Vergani
Published: 2026-11-09
Source: https://arxiv.org/abs/2611.13339

## Publisher abstract (plain-text excerpt from arXiv API)

In social science research, text annotation is a fundamental task that is traditionally a costly, hard-to-scale manual process. Researchers have used large language models (LLMs) to perform annotation by writing a definition of a concept into a prompt - a rule that determines whether a label should be attributed to a text depending on its content. However, concepts such as hate speech, fake news, and terrorism typically have several theoretically defensible competing definitions. It is also unknown whether the model actually applied the definition to provide the label or the label was based on the model's pretrained notion of the concept. To test this, we have the model annotate the same texts twice, each time with a different definition. We call the disagreement between the two sets of annotations definition sensitivity. As a control, we paraphrase one definition but leave its requirements unchanged - the disagreement between the annotations with the two wordings becomes the paraphrase floor. Across six concepts and three LLMs, a swap of competing definitions always changes more annotations, on average, than a paraphrase. This shows that the annotations depend on the prompted definition, so any set of annotations should be interpreted together with the definition that produced it. The LLM annotator's definition sensitivity and its paraphrase floor should both be reported in such work.

## Curator takeaway (interpretation, not a study result)

When a classification rule changes, compare labels from both definitions and keep the rule alongside every result.
