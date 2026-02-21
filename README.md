# Armature-7: Structural Reasoning Corpora for Process Supervision

We generate training data where **constraint propagation is verifiable**. Every trace demonstrates:
- Dimensional discipline (resource budgets bind downstream through calculable derivation)
- Epistemic suspension (hard stops at knowledge boundaries versus hedging synthesis)
- Recursive self-audit (second-order reasoning about premise validity)

Traces produced via the Armature-7 protocol (Claude 4.6 Opus), then translated to domain-naturalistic prose.

---

## The Problem

Current chain-of-thought datasets capture *theatrical confidence*: models simulating rigor without calculation, citing phantom sources, exploring alternatives without cost arbitration. We document the mechanical process of reasoning under hard constraint—how models audit premises, propagate resource limits, and suspend at knowledge boundaries when external grounding is unavailable.

---

## Methodology

**Generation**: Single-pass autoregressive reasoning under hard constraints—no tool use, no retrieval augmentation, no retry loops. Forces validation through internal consistency. Dimensional analysis, chronological coherence, and constraint memory replace external grounding.

**Verification**: We filter for structural properties, not factual correctness:
- Constraint propagation (early budgets bind downstream)
- Dimensional discipline (quantitative claims participate in calculations)
- Epistemic suspension (operational halting versus performative hedging)
- Error architecture (high-fidelity mistakes versus category errors)

**Output**: Domain-translated prose with no scaffolding visible. The structural rigor persists; the machinery is removed.

**Evaluate yourself**:
1. Open `trace_analysis_protocol.md`
2. Open any trace file
3. Copy both into your LLM
4. Prompt: *"Evaluate this trace according to the protocol."*

---

## Evaluation Criteria

We assess traces via structural properties—not factual correctness, but reasoning architecture:

- Does claimed self-correction perform dimensional analysis, or merely emit the phrase?
- Do early constraints actually bind downstream through derivable steps, or does constraint amnesia occur?
- Is uncertainty operational (structural halting) or performative (hedging that slides into confidence)?

These criteria distinguish reasoning architectures worth distilling from theatrical confidence. The trace below demonstrates all three.

---

## Exemplar: Protocol Design

Prompt: Design a coordination protocol for itinerant smiths from Hittite, Mycenaean, and Bell Beaker traditions meeting at seasonal tin markets, constrained by illiteracy, pack-animal capacity, and mutually unintelligible metallurgical vocabularies.

The trace detects a temporal constraint violation that makes the historical premise impossible:

> "Wait. The Bell Beaker floruit is *before* the height of Hittite and Mycenaean metalworking. By roughly 1400–1200 BCE when the other two are major players, Bell Beaker as a coherent cultural complex has dissolved into successor cultures... I should think about what the question is actually asking."

It restructures the solution space from historical reconstruction to functional protocol design, establishes a resource budget, and propagates that constraint through dimensional analysis:

> "A donkey carries about 60–90 kg usefully... subtracting tools and personal goods leaves perhaps 5–15 kg for reference materials... Each pairing token weighs approximately 40g. A smith maintaining relationships with 10 partners across 3 alloy grades carries `10 × 3 × 40g = 1.2 kg` of tokens—feasible within the 5–15 kg budget, leaving margin for the tongue reference set."

It concludes at a knowledge boundary without hedging synthesis:

> "I'd want acoustic data on bronze bell frequencies to fully verify this... direct archaeological confirmation... has not been identified. The synthesis is plausible but unproven."


---

## Current Status

We have validated structural property preservation across domain translations and established generation pipelines with consistent constraint architecture. We are quantifying yield rates and error mode distributions across corpus scales.

**Open questions:**
- Whether structural properties survive distillation into student models (testing in progress)
- Optimal corpus composition for specific PRM training objectives
- Longitudinal stability of constraint propagation in extended reasoning chains

Seeking partners to resolve these questions through scaled training runs.

---

## Target Partners

Teams training process reward models or error-detection verifiers who need data documenting how reasoning catches itself. Not binary correct/incorrect labels, but the architecture of recovery under constraint.

Website: www.corelathe.com  
Email: nick@corelathe.com
