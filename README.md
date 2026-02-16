# Sinterform Cognitive Traces

Raw synthetic reasoning trajectories generated under adversarial constraints. These are cognitive stress-tests captured in single-pass generation with explicit epistemic scaffolding and are not polished.

**Quick Evaluation**

1. Open `trace_analysis_protocol.md`—this is the evaluation rubric
2. Open any trace file (e.g., `embedded_protocol_design.md`)
3. Copy both contents into your LLM (Claude, GPT-5, Gemini, etc.)
4. Ask: *"Evaluate this trace against the protocol"*

**Generation Context**
- **Mode:** Single-shot (1-shot), no retries
- **Scaffolding:** Advanced System 2 architecture (recursive verification, reflection markers)
- **Post-Processing:** Raw protocol output translated to prose (non-generative formatting)
- **Constraints:** No MCP validations, no external tools, no empirical verification, no context injection
- **Baseline:** Standard LLM behavior under identical constraints typically yields incorrect mathematics, optimistic resource estimates, and unverified technical claims
- **Target:** Expert-class error detection (sophisticated confabulation vs. naive hallucination)

**What to Look For**
- **Negative capability**: Does it resist the solution impulse long enough to map constraints? (Look for explicit halts before abstraction.)
- **Epistemic hygiene**: Are uncertainty and verification gaps marked explicitly, or buried in confident prose?
- **Constraint maintenance**: Does it suffer "constraint amnesia" mid-reasoning?
- **Grounding discipline**: Concrete instantiation (specific sensors, byte counts) preceding every abstraction.
- **Error mode sophistication**: Distinguishing naive confabulation (category errors) from expert-class mistakes (optimistic resource assumptions that look like competence).
- **Process over outcome**: The architecture of the search matters more than the final answer.


**Contact**

Website: www.corelathe.com  
Email: nick@corelathe.com

