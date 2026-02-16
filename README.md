**Sinterform Traces**

Raw synthetic reasoning trajectories generated under adversarial constraints. These are not polished outputs— they are cognitive stress-tests captured in single-pass generation with explicit epistemic scaffolding.

**Quick Evaluation**

1. Open `cognitive_trace_analysis_protocol.md`—this is the evaluation rubric
2. Open any trace file (e.g., `embedded_protocol_design.md`)
3. Copy both contents into your LLM (Claude, o1, Gemini, etc.)
4. Ask: *"Evaluate this trace against the protocol"*

**Generation Context**
- **Mode:** Single-shot (1-shot), no retries
- **Scaffolding:** Advanced System 2 architecture (recursive verification, reflection markers)
- **Constraints:** No MCP validations, no external tools, no empirical verification, no context injection
- **Baseline:** Standard LLM behavior under identical constraints typically yields incorrect mathematics, optimistic resource estimates, and unverified technical claims
- **Target:** Expert-class error detection (sophisticated confabulation vs. naive hallucination)

**What to Look For**
Constraint maintenance under memory pressure, negative capability (resistance to premature abstraction), explicit uncertainty signaling, and high-fidelity error modes (e.g., implicit complexity scaling, hardware optimism).

**Contact**
Website: www.corelathe.com  
Email: nick@corelathe.com

