# Foundational Architecture Patterns (v0.1)

**Purpose:**  
Provide a small set of **foundational patterns** that make AI systems stable, extensible, and governable over time.

This layer does not define behavior or security controls.  
It defines **how systems should be shaped before those concerns appear**.

Artifact-only. Interface-neutral. Pattern-driven.

---

## Pattern 1 — Structure before control
Do not start with policies, guardrails, or constraints.  
Start with **clear structure**: components, boundaries, and responsibilities.

Control applied to an unclear structure amplifies confusion.

---

## Pattern 2 — Explicit boundaries over implicit rules
Implicit rules drift.  
Explicit boundaries can be inspected, discussed, and revised.

A boundary should answer:
- what is allowed
- what is forbidden
- who owns decisions beyond it

---

## Pattern 3 — Evidence before authority
Authority without evidence creates brittle systems.

Prefer systems where:
- actions require minimal evidence
- decisions reference observable state
- escalation happens because evidence is missing, not because confidence is low

---

## Pattern 4 — Design for drift, not perfection
All systems drift.

Stable architectures:
- expect drift
- surface it early
- make correction cheap

Perfect initial designs fail silently.

---

## Pattern 5 — Modularity beats central intelligence
Large, central reasoning systems are hard to audit and hard to evolve.

Prefer:
- small, composable units
- explicit handoffs
- clear ownership per module

---

## Pattern 6 — Calm systems outperform clever ones
Clever systems impress early.  
Calm systems survive contact with reality.

Calm systems:
- fail loudly and early
- escalate predictably
- avoid theatrical complexity

---

## Pattern 7 — Evolution via layers, not rewrites
Stable systems grow by adding layers, not replacing cores.

Layering allows:
- gradual improvement
- local experimentation
- preserved institutional knowledge

---

## How to use this layer
- Apply these patterns before defining interaction or security rules
- Use them as review criteria for new AI initiatives
- Treat violations as architectural risk, not style issues

---

## Related layers
- Human–AI Interaction Baseline
- Security & Stability Baseline

