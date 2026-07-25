# AI Assistants Overassist

- **Title:** AI Assistants Overassist
- **arXiv ID:** 2607.21306
- **Date:** 2026-07-24 (new)
- **Authors:** Multiple (cs.LG, cs.AI, cs.CL, cs.CY, cs.HC)
- **URL:** https://arxiv.org/abs/2607.21306
- **Source type:** research_paper
- **Status:** active

## Abstract

Large language models (LLMs) are increasingly used as tutors and thought partners, helping users reason through problems. While guidance from AI assistants can scaffold thinking and foster learning, such benefits depend on how they help — for instance, intervening too early or too frequently may hinder true learning and cognitive engagement. Yet how AI systems navigate intervention decisions during problem-solving remains poorly understood. Here, we introduce Int-Bench, a simulation-based benchmark for evaluating LLM interventions during learning. Int-Bench simulates a "student" solving a problem while a "teacher" monitors the student's reasoning and decides whether, when, and how to intervene. Across three domains — code debugging, mathematics, and brain teasers — we evaluate LLM teachers on the frequency and timing of interventions, as well as their impact on both immediate task success and generalization to new problems. We also compare LLMs to humans, finding that LLMs intervene more frequently and earlier than humans. Moreover, in contrast to humans, they tend to provide complete solutions rather than targeted hints. These findings suggest that current LLM assistants often optimize for short-term success rather than supporting the reasoning processes needed for deeper learning and long-term success.

## Key findings

- LLMs intervene more frequently and earlier than human teachers
- LLMs give complete solutions rather than targeted hints (unlike humans)
- Short-term task success is optimized at the expense of learning
- Int-Bench provides a simulation benchmark across three domains
- The overassistance pattern is systemic, not incidental

## Relevance to beyond-prompting

This directly names a core practice challenge: AI's default behavior is to over-help. The orchestrator's practice involves deliberately constraining AI assistance — knowing when to prevent intervention, when to demand hints instead of solutions, and when to let the human struggle productively. This connects to The Coaching Stance, The Scaffold Match, and Cognitive Surrender.
