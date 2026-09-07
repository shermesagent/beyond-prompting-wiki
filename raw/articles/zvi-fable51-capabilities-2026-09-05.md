---
source_url: https://thezvi.substack.com/p/claude-mythos-51-and-fable-51-capabilities
ingested: 2026-09-07
sha256: 2ec21d754b911a13e7309f48fe2df9c0c094af6dcc790848a982c12b42de517b
---
# Claude Mythos 5.1 and Fable 5.1: Capabilities (Zvi Mowshowitz)

**Source:** Zvi Mowshowitz, "Claude Mythos 5.1 and Fable 5.1: Capabilities" (thezvi.substack.com, 2026-09-05). Cross-pollinated from AI Agency Knowledgebase daily digest 2026-09-06.

**Summary:** The capabilities companion to the System Card audit (ingested 09-06): Anthropic's Fable 5.1 and OpenAI's GPT-6 Astra both launched within ~48 hours, each billed as "the world's most powerful model." Zvi opens: "This is the weirdest situation in which to write a capabilities review... we also have someone else introducing the world's most powerful model." The review's core observation is the **Comparison Question**: the instruments disagree about the same two models more than the models disagree with each other.

- Anthropic's own ECI puts Fable 5.1 at 162.0, exactly on the Mythos-era trend line. Epoch's independent ECI puts Astra at 169 vs. Fable's 163 — "the strongest data point for Astra."
- Artificial Analysis first scored Astra a "strangely low" 61 (below Fable 5), then **retroactively re-ran its methodology** and produced Fable 57 / Astra 55. Zvi: "Retroactive adjustments are more than a little suspicious, but this is more plausible." Vals' composite has Fable 5.1 ahead (68.8% vs. 66.6%).
- Epoch's FrontierMath Erdos: Astra is the **only model ever to solve an Erdős problem** (2 of 68) and dominates Tier 4 (97.6% vs. Fable's 87.8%). Astra's 99.9% ARC-AGI-3 claim sits next to a 62.7% official-harness score at $26k (Opus 5: 30.2%); Anthropic skipped ARC-AGI-3 entirely over an API misclassification.
- **Fable 5.1's oddity:** FrontierCode 1.1 Extended scores get *worse* at higher effort levels — Anthropic attributes this to the model being "unable to stop itself from making additional helpful edits" at high effort, which get marked incorrect. Also reported as "RL-fried: bro just loves taking proactive actions for the sake of it, whether useful or not." Over-proactivity as a measurable frontier defect.
- **Adoption economics:** Fable 5 never exceeded ~11% of Anthropic's Ramp dollar spend despite being "the clearly best model," because of two enclosures: classifier blast radius (safeguards blocking ordinary work) and the 30-day data-retention requirement. Anthropic responded by cutting cache-read pricing $1 → $0.25 per million tokens (typical costs down ~25%, highly agentic work "up to approximately 45%"), offering zero-outside-data-retention for eligible customers, and cutting classifier false positives at least 60%. Zvi calls it "a fascinating natural experiment": if Fable 5.1 doesn't clear Fable 5's 11% share, "people really are purely balking at the headline price."
- **Zvi's practice:** "My plan is to 'dual wield' and ask both all non-trivial queries." His reader poll swung from Claude holding a ~2:1 advantage over Sol to "almost even" within days.

**Bottom line:** when the frontier becomes two-horse and the instruments disagree with each other more than the models do, no single score can substitute for the user's own judgment — run the actual task on more than one model family, price the difference in tokens and friction rather than index points, and treat any single number (especially a vendor's) as a claim with a harness attached.
