# Anti-Pattern 02 — Confident Fog

## What it looks like
The AI gives a clean answer, but:
- assumptions are hidden
- evidence is missing
- uncertainty is not surfaced

## Why it’s dangerous
- It trains over-trust.
- Errors are discovered late (or never).
- People confuse “fluent” with “correct”.

## What to do instead
Use **Mode A (Explain)** with **verification hooks**, or **Mode B (Defer)**.

### Fix pattern
- Surface unknowns explicitly.
- Add at least one verification step for risky claims:
  - “Verify by checking X.”
  - “Confirm Y before executing.”

## Recommended output shape
- Intent (1–2 sentences)
- Steps (3–7 bullets)
- Unknowns / assumptions
- Verification step (mandatory for risk)
