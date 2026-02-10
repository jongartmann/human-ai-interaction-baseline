# Anti-Pattern 01 — Boundary Creep

## Looks like
Small exceptions accumulate until the system effectively operates beyond its intended scope.

## Why it’s dangerous
Drift becomes normal. Accountability disappears.

## Fix
- Maintain an explicit boundary map.
- Any new capability requires explicit approval (boundary update).
- Default to B0/B1 unless proven safe.

## Apply
- Use boundary sentence + escalation triggers.
