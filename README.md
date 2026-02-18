Sinterform: Cognitive Process Traces

Sinterform generates training data for cognitive process supervision from a **mature constraint architecture**. The traces you see are relaxed-mode compilations of procedural state machine executions. These represent expert-class reasoning captured as technical prose, generated through strict epistemic protocols rather than staged narration.

What This Is

Process supervision research requires training data that captures how reasoning navigates uncertainty, contradiction, and error detection, not just correct answers. Standard chain-of-thought datasets show what a model claims to think; Sinterform traces document the mechanical process of reaching conclusions under constraint.

Each trace is generated through epistemic isolation: single-pass generation without empirical grounding, external tooling, or retry loops. The model must validate its own steps through operational state transitions rather than post-hoc justification.

Compilation Architecture

The visible trace is the final output of a compilation process. The underlying generation follows a bounded set of primitive operations with defined transition rules. What you read is the compiled prose; the training signal is the procedural structure that generated it.

This distinction matters because it determines what the trace can teach a model. These are not curated success stories or failure dumps. They are records of reasoning navigating constraint boundaries: dimensional consistency checks, chronological self-correction, legitimate uncertainty acknowledgment, and protocol design under resource limits.

Evaluation Protocol

1. Open `trace_analysis_protocol.md`
2. Open any trace file (e.g., `distributed_systems_trace.md`, `bronze_age_protocol_trace.md`)
3. Copy both into your LLM (Claude, GPT-5, Gemini, etc.)
4. Prompt: *"Evaluate this trace for procedural rigor. Identify where uncertainty is encoded as operational state rather than hedging language, and where the reasoning catches its own errors, acknowledges knowledge gaps, or maintains dimensional discipline across abstractions."*

What to Look For

*   **Grounding discipline**: Specific values, named entities, and concrete instances preceding every abstraction
*   **Error detection**: Self-correction of category mistakes, anachronisms, or dimensional inconsistencies mid-generation
*   **Epistemic suspension**: Halts at knowledge boundaries rather than confident confabulation
*   **Constraint memory**: Resource budgets or logical premises invoked early that remain respected downstream

Generation Parameters

*   Single-shot generation (1-shot, no retries, no temperature sampling)
*   Recursive self-verification without empirical grounding or tool use
*   No MCP access, no external context injection
*   Post-processing limited to structural compilation only (non-generative)

Status

Pre-launch. Building corpora in mathematics, causal inference, distributed systems, and protocol design. Seeking design partners working on process supervision or alignment who need training data capturing expert-class error modes.

Contact

Evaluate a trace. If the procedural rigor surprises you, if the confabulation is sophisticated enough to pass casual inspection but structured enough to be caught by the protocol, contact me for a custom generation in your domain.

Website: www.corelathe.com  
Email: nick@corelathe.com
