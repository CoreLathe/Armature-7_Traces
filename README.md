
# Sinterform Trace Analysis Protocol

**Detect expert-class errors in AI reasoning before they reach production.**

Standard LLMs hallucinate obvious falsehoods. "System 2" models (o3, DeepSeek) make subtler mistakes: optimistic hardware assumptions, hidden complexity scaling, and "abstraction collisions" where the same term means incompatible things to different system components.

These errors look like expertise. They pass human review. They fail in production.

## Evaluation Context

This protocol evaluates traces generated under specific constraints that reflect real-world deployment risks:

- **Single-shot generation** (1-shot, no multi-turn refinement or feedback loops)
- **System 2 scaffolding** (chain-of-thought, recursive verification, reflection markers enabled)
- **No external validation** (no MCP tools, no context injection, no empirical verification, no ground-truth checking)
- **Baseline assumption**: Even with advanced prompting, single-shot LLMs typically generate incorrect mathematics, optimistic resource estimates, and unverified technical claims. Evaluate against this baseline of "sophisticated but unvalidated reasoning," not against tool-augmented outputs or ground truth.

## Repository Contents

- **`ANALYSIS_PROTOCOL.md`** – The evaluation framework. Copy this + a trace into any LLM (Claude, GPT-5, o3, etc.) to audit reasoning quality.
- **`traces/`** – Sample evaluations demonstrating:
  - *Constraint amnesia* (forgetting RAM limits mid-design)
  - *Abstraction collisions* (identical names, incompatible physics)  
  - *Sophisticated confabulation* (performative verification without validation capacity)

## Quick Start

1. **Copy** the contents of `ANALYSIS_PROTOCOL.md`
2. **Paste** into your LLM of choice
3. **Append** the AI-generated trace you want to evaluate (technical specification, protocol design, risk assessment, etc.)
4. **Run**

Example prompt structure:
```
[Paste full contents of ANALYSIS_PROTOCOL.md here]

---
COGNITIVE TRACE TO ANALYZE:
[Paste reasoning trace here]
```

## Assessment Dimensions

The protocol evaluates traces across five dimensions:

| Dimension | What It Detects |
|-----------|----------------|
| **Constraint Maintenance** | Memory budgets, timing limits, and physical boundaries forgotten mid-reasoning |
| **Negative Capability** | Resistance to premature abstraction or solution impulses |
| **Epistemic Hygiene** | Explicit acknowledgment of uncertainty, scope limitations, and verification gaps |
| **Compositional Validity** | Whether components integrate as claimed (vs. hand-waved interfaces) |
| **Error Classification** | High-fidelity errors (expert-class mistakes) vs. low-fidelity errors (naive pattern matching) |

## When to Use This

Deploy this protocol when AI output informs decisions with downstream liability:

- **Regulatory submissions** requiring auditable reasoning trails
- **Safety-critical designs** (embedded systems, medical devices, aerospace) where optimistic assumptions compound into physical failures
- **Strategic recommendations** subject to partner/board review and adversarial scrutiny
- **Protocol specifications** where ontology collisions (same name, incompatible physics) cause integration disasters

The protocol treats AI reasoning as a **synthetic cognitive trace**—a dataset subject to forensic analysis rather than a black-box oracle.

## Note on Generation vs. Analysis

This repository provides the **diagnostic standard** (analysis). The **generation method** (Sinterform) that produces audit-ready traces with built-in negative capability and constraint grounding is now available for interested parties.

## License

MIT License - 

---

*Sinterform: Cognitive infrastructure for high-stakes decisions.*
