# Armature-7: Reasoning Traces for Process Supervision

Training data that captures how models handle uncertainty, contradiction, and resource limits. Not curated successes, but the mechanical process of reaching conclusions under constraint.

## The Signal

Current chain-of-thought datasets show what models *claim* to think. We document the procedural structure that generated the conclusion, including the failures.

Consider this unprompted correction from a trace designing bronze-age trade protocols:

> Wait. The Bell Beaker floruit is *before* the height of Hittite and Mycenaean metalworking. By roughly 1400–1200 BCE when the other two are major players, Bell Beaker as a coherent cultural complex has dissolved into successor cultures... I should think about what the question is actually asking.

No external fact-checker triggered this. No retry loop. The model suspended its own solution attempt, discarded the framing, and regrouped within a single generation pass under strict epistemic isolation.

This is the recursive error-detection signal that process supervision requires.

## Methodology

We generate single-pass autoregressive traces under hard constraints: no tool use (MCP, search, calculation engines), no retrieval augmentation, no retry loops. This forces validation through internal consistency. Dimensional analysis, chronological coherence, and constraint memory take the place of external grounding.

We then filter aggressively for structural properties, not factual correctness:

- **Constraint memory:** Resource budgets mentioned early that bind later decisions (for example, donkey load limits calculated at 60-90kg that subsequently bound token weight designs)
- **Dimensional discipline:** Quantitative claims that participate in calculations, not decorative numeracy  
- **Epistemic suspension:** Hard stops at knowledge boundaries versus stylistic hedging
- **Error architecture:** High-fidelity mistakes (subtle off-by-one errors, optimistic assumptions that survive initial scrutiny) versus category errors

The result is not ground-truth verified knowledge. It is reasoning architectures worth distilling. These traces demonstrate how cognition navigates limits when empirical validation is unavailable.

## Evaluation Protocol

We assess traces via the protocol in `trace_analysis_protocol.md`. Key criteria:

- Does claimed self-correction perform dimensional analysis, or merely emit the phrase?
- Do early constraints actually bind downstream, or does constraint amnesia occur?
- Is uncertainty operational (structural halting) or performative (hedging that slides into confidence)?

Try it. Open any trace. Look for the moment where the model audits its own confidence, checks its resource budget, or halts at a knowledge gap rather than confabulating. If the procedural rigor surprises you, the methodology is working.

## Current Status

Pre-release. Building corpora in:

- **Mathematics:** Complex derivations with off-by-one vulnerabilities
- **Distributed systems:** Optimistic architectural assumptions buckling under dimensional audit  
- **Causal inference:** Confounding detection without empirical grounding
- **Protocol design:** Consensus mechanisms under resource constraints

Each corpus targets specific high-fidelity error modes. Subtle constraint interactions. Temporal drift in multi-step reasoning. Premature closure under token pressure.

We do not yet know if this methodology scales beyond boutique generation, or if the structural properties survive distillation into smaller models. The constraints may prove too brittle, or the error modes too idiosyncratic. We are documenting the boundary conditions as carefully as the successes.

Seeking design partners training process reward models or error-detection verifiers who need data documenting how reasoning catches itself. Not binary correct or incorrect labels, but the kinematics of constraint navigation.

Website: www.corelathe.com  
Email: nick@corelathe.com
