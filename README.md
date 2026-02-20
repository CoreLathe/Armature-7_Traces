# Armature-7: Cognitive Hygiene as AI Infrastructure

Armature-7 generates training data for cognitive process supervision from resource-aware procedural executions. The traces are compiled records of reasoning navigating uncertainty, contradiction, and resource limits without external validation: not curated success stories, not failure dumps, but the mechanical process of reaching conclusions under operational constraint.

## What This Is

Process supervision research needs training data that captures how reasoning handles uncertainty and error detection, not just correct answers. Standard chain-of-thought datasets show what a model claims to think. Armature-7 traces document the procedural structure that generated the conclusion.

Each trace is produced under epistemic isolation: no retries, no external tooling, no empirical grounding. The model validates its own steps through operational state transitions rather than post-hoc justification. The visible prose is the compiled output; the training signal is the constraint navigation underneath.

## What This Looks Like

A raw fragment from a trace designing bronze-age trade protocols. Note the self-correction emerging mid-generation, not added afterward:

> Wait — I'm already reaching toward protocol design and I haven't even mapped the failure modes yet. Let me get specific about what actually collides.
>
> [failure mode taxonomy]
>
> A dimensional signature. Not names, not units, not scales — just the dimensional exponents of what's being measured... This is not an ontology — it's physics itself. It's 7 small integers. 7 bytes.
>
> Am I hand-waving the distinction between "shared physics" and "shared ontology" here? Let me check.
>
> [later]
>
> Quick check on the dim_sig packing: 7 × 4-bit values = 28 bits, fits in 4 bytes... That works.
>
> [later]
>
> ```
> STATIC (compiled in):
>   Own channel descriptors:     8 channels × 14 bytes  =  112 bytes
>   Protocol state machine:      ~200 bytes code-resident state
>   Subtotal:                    ~312 bytes
>
> PER-NEIGHBOR (dynamic):
>   ...
>   At 4KB budget: floor((4096 - 312) / 147) = 25 neighbors max
> ```

The trace catches itself rushing to build a solution, stops to list five specific ways devices can clash, then discovers that 7 bytes of basic physics data replace complex negotiations. Fifty lines of reasoning later, it verifies the exact math against that original 64KB limit, calculating precisely 25 devices max. Typical AI forgets the budget after paragraph one; this remembers it from start to finish.

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
