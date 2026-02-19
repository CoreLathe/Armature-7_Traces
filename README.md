# Sinterform: Cognitive Hygiene as AI Infrastructure

Sinterform generates training data for cognitive process supervision from **constrained procedural executions**. The traces are compiled records of reasoning navigating uncertainty, contradiction, and resource limits without external validation: not curated success stories, not failure dumps, but the mechanical process of reaching conclusions under operational constraint.

## What This Is

Process supervision research needs training data that captures how reasoning handles uncertainty and error detection, not just correct answers. Standard chain-of-thought datasets show what a model claims to think. Sinterform traces document the procedural structure that generated the conclusion.

Each trace is produced under epistemic isolation: no retries, no external tooling, no empirical grounding. The model validates its own steps through operational state transitions rather than post-hoc justification. The visible prose is the compiled output; the training signal is the constraint navigation underneath.

## What This Looks Like

A raw fragment from a trace designing bronze-age trade protocols. Note the self-correction emerging mid-generation, not added afterward:

> Wait. The Bell Beaker floruit is *before* the height of Hittite and Mycenaean metalworking. By roughly 1400–1200 BCE when the other two are major players, Bell Beaker as a coherent cultural complex has dissolved into successor cultures. These three traditions don't straightforwardly walk into the same market simultaneously.
>
> But I should think about what the question is actually asking. The three names function as stand-ins for three distinct, mutually unintelligible metallurgical traditions with different alloy standards. The design problem is real regardless of exact chronological overlap.

The trace detects its own anachronism, discards the current framing, and regroups with a reframed premise, all within a single generation pass.

## Evaluation Protocol

1. Open `trace_analysis_protocol.md`
2. Open any trace file
3. Copy both into your LLM
4. Prompt: *"Evaluate this trace according to the protocol."*

## What to Look For

* **Grounding discipline**: Specific values, named entities, and concrete instances preceding every abstraction
* **Error detection**: Self-correction of category mistakes, anachronisms, or dimensional inconsistencies mid-generation
* **Epistemic suspension**: Halts at knowledge boundaries rather than confident conflation
* **Constraint memory**: Resource budgets or logical premises invoked early that remain respected downstream

## Generation Parameters

* Epistemic isolation: no retries, no external tooling (MCP, search, calculation engines)
* Recursive self-verification without empirical grounding
* Post-processing limited to structural formatting (non-generative)

## Status

Pre-release. Building corpora in mathematics, causal inference, distributed systems, and protocol design. Current focus: high-fidelity error modes, subtle constraint interactions, off-by-one errors in complex derivations, optimistic architectural assumptions that survive initial scrutiny but buckle under dimensional audit.

Seeking design partners working on process supervision or alignment who need training data documenting how reasoning catches itself.

## Contact

Evaluate a trace. If the procedural rigor surprises you, reach out for a custom generation in your domain.

Website: www.corelathe.com

Email: nick@corelathe.com
