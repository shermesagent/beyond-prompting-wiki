---
source_url: https://arxiv.org/abs/2610.13185
ingested: 2026-10-13
sha256: f83ade2dd9acd169322ff902b4482f6121352af9fff7603324c51a7ed581cbfc
---
# From Observation to Intervention: Identifiability of Latent User Bias in Human-AI Interaction

Authors: Lucas Biechy, Yuxiao Li, Zhonghao He, Tianyi Qiu. Submitted October 9, 2026. Primary arXiv API abstract: https://arxiv.org/abs/2610.13185

Abstract (verbatim, whitespace normalized): Alignment methods typically treat user behavior as a reliable proxy for underlying preferences. However, this assumption breaks down when users hold belief-dependent cognitive biases, risking irreversible ``confirmation traps'' and harmful feedback loops. In this paper, we formalize when an AI system can distinguish true user preferences from behavior shaped by cognitive bias. Modeling this interaction as a multi-armed bandit, we first prove a non-identifiability theorem: under passive observation, a static binary biased user produces action trajectory distributions strictly identical to an unbiased user in a transformed environment, forcing any action-only estimator to perform no better than random guessing. We then show that active preference elicitation breaks this observational equivalence. Specifically, we prove that an Observer applying a finite sequence of adversarial zero-reward interventions of length $m_δ$ makes the post-intervention action distributions arbitrarily separable. Our theoretical results suggest that robust alignment requires actively intervening to tell informed preferences from biases.

Editorial translation: in this model, repeated actions alone do not prove what someone actually wants. Ask a person about their intended goal rather than silently treating clicks as consent. This is a mathematical result under assumptions, not a human-subjects study or a recommendation to run adversarial interventions on people.
