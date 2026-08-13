---
title: No One to Blame
created: 2026-08-13
updated: 2026-08-13
type: concept
tags: [barrier, trust, governance, accountability, orchestrator]
sources:
  - raw/articles/constitutive-ai-unaccountability-2608.12104.md
confidence: medium
---

# No One to Blame

## What It Is

"No one to blame" is the knot in your stomach when you realize that if the agent makes a catastrophic mistake, there is **no person who will be held accountable** — not you, not the vendor, not the model. It's the version of [[Fear of Losing Control]] where the fear is not "I don't know what it'll do," but "even after it does it, nobody answers for it."

A framework paper (arXiv:2608.12104, August 2026) argues this is not a solvable gap. Existing research frames AI accountability gaps as barriers that can be overcome through better standards, transparency, and institutional reform. The paper's claim: **certain configurations of actors, systems, and institutions render accountability conceptually unachievable regardless of effort.** They call it *constitutive AI unaccountability* — unaccountability isn't a defect to be fixed, it's a property of the arrangement.

## Why It's Normal

Through a three-stage qualitative study — concept-centric literature analysis, secondary analysis of 27 expert interviews with AI professionals (technical, legal, sociotechnical backgrounds), and a framework application to the open-source agentic AI system OpenClaw — the researchers identified **nine categories and twenty themes of constitutive unaccountability**, organized across three clusters that reinforce one another:

- **Structural** — who is positioned to answer, and whether anyone is (diffusion of responsibility across many hands, vendor-subcontractor chains, absent principals)
- **Technological** — what the system itself makes impossible to inspect or attribute (opaque internals, non-reproducible behavior, [[Silent Updates]]-style unversioned change)
- **Normative** — what the rules themselves don't cover (no law, no contract clause, no liability assignment reaches the case)

The interdependencies matter: these aren't twenty separate gaps. They fire in chains — a structural void makes the technological opacity worse, which makes the normative gap wider.

The paper's most unsettling finding came from the OpenClaw application: the diagnostic detected 17 of 20 conditions, including an **inverted anthropomorphism** configuration in which the AI agent was the only identifiable actor. Not "the human is blamed for the agent" — the *agent itself* was the only entity anyone could point to. You can't hold a model accountable, but the arrangement left no one else to name.

## The Bridge

If unaccountability is constitutive — built into the arrangement — then the bridge is not "more transparency." The bridge is **naming the accountable actor before you delegate.** The paper operationalizes this as a diagnostic instrument of 20 questions for identifying accountability voids in specific deployments. The distilled version for your workflow:

1. **Name the person.** Before you delegate anything consequential, ask: "If this fails, who specifically answers?" If the answer is a shrug, a team, or "the model," you have a void — fix the arrangement before you run it.
2. **Refuse to be the only identifiable actor** for systems you don't control. The OpenClaw lesson cuts both ways: when you're the only human name attached to an autonomous system's actions, you're holding an inverted anthropomorphism all by yourself. That's not accountability — that's exposure.
3. **Audit the chain of custody.** Can you trace what was evaluated, what was served, and what changed? (See [[Silent Updates]].) No chain → no attribution → no accountability.
4. **Separate propose from approve from audit.** The same structural fix as [[Accountability Asymmetry]]: the entity that proposes an action should never be its sole approver and auditor.

## Try This

**5-Minute Exercise: The Blame Drill**

Pick your most consequential delegated workflow. Ask: "If this goes catastrophically wrong, who can be held to account — by name?"

- If you named a person: good. Add one sentence to the workflow brief naming them as the accountable owner, so the arrangement matches the assumption.
- If you couldn't: write down what's missing — an approval step? A named owner? A versioned artifact? — and add the smallest missing piece. The point isn't bureaucracy. It's that an arrangement with no one to blame is an arrangement that will eventually hurt someone, and it won't be the model.

## Related Pages

[[Accountability Asymmetry]] · [[Silent Updates]] · [[Fear of Losing Control]] · [[Trust Calibration]] · [[The Observability Gap]] · [[Knowledge Debt]]

## Tags

#barrier #trust #governance #accountability #orchestrator
