# Anti-Pattern 07 — Resume Without State

## What it looks like
Long tasks end with:
- no clear state
- no next step
- no “how to continue”

## Why it’s dangerous
- Users re-explain.
- Sessions fragment.
- Work slows down as “context management” grows.

## What to do instead
Always end long tasks with a **resume hook**:
- current state
- next step
- exact resume instruction

## Recommended output shape
**State:** …
**Next:** …
**Resume:** “Paste X and say ‘continue’.”
