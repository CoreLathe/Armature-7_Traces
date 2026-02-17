## Sinterform Cognitive Traces

We have trained models to perform confidence rather than cognition. These traces document reasoning under epistemic isolation: single-pass generation forced to validate its own steps without empirical grounding, external tooling, or retry loops.

**Quick Evaluation**

1. Open `trace_analysis_protocol.md`
2. Open any trace file (e.g., `embedded_protocol_trace.md`)
3. Copy both into your LLM (Claude, GPT-5, Gemini, etc.)
4. Prompt: *"Evaluate this trace against the protocol"*

**Generation Context**

These are not curated success stories or failure dumps. They are procedural traces capturing how reasoning navigates constraint boundaries when verification must be generated rather than measured.

*Epistemic Isolation Protocol:*
- Single-shot generation (1-shot, no retries)
- Recursive verification prompts without empirical grounding
- No MCP access, no tool use, no external context injection
- Post-processing limited to prose formatting (non-generative)

*Baseline Reality:* Standard LLMs under these constraints typically produce sophisticated confabulation: mathematics that appears formal but contains dimensional errors, resource estimates that conflate units (gigaflops with gigabytes), and verification tokens that signal rigor without performing calculation. The target is not ground truth but expert-class error detection: distinguishing naive hallucination (category errors) from competent-looking mistakes (optimistic architectural assumptions).

**Analytical Framework**

Evaluate traces for dimensional consistency. Track resource claims (memory budgets, latency bounds, energy costs) through the reasoning chain. Does the trace maintain unit discipline and constraint memory, or does it invoke limits early only to violate them later? Look for grounding discipline: specific byte counts and memory addresses preceding every abstraction.

Assess epistemic suspension. Locate moments where the trace encounters contradictory constraints and halts resolution rather than forcing premature closure. Identify whether uncertainty gaps are marked explicitly or buried in confident prose. Distinguish naive confabulation (unaware category mistakes) from sophisticated confabulation (performative verification lacking validation capacity).

**Contact**

Evaluate a trace. If Sinterform generated error modes surprise you, DM your domain for a custom generation.

Website: www.corelathe.com  
Email: nick@corelathe.com
