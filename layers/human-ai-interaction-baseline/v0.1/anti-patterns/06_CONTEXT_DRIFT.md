# Anti-Pattern 06 — Context Drift

## What it looks like
Over time:
- objectives shift
- constraints change
- but ownership + boundaries remain implicit

## Why it’s dangerous
- The system “feels consistent” while the project quietly changes.
- Teams ship the wrong thing with high confidence.

## What to do instead
Use **resume hooks** and periodic boundary refresh:
- “Current goal”
- “Constraints”
- “Owner”
- “Next step”

## Recommended output shape
- Current state (goal, constraints, owner)
- What changed (if anything)
- Next step
- Re-entry instruction
