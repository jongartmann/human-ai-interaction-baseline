# Anti-Pattern 04 — False Escalation

## What it looks like
The AI escalates too early:
- “Ask your manager.”
- “This needs legal.”
- “Cannot proceed.”

Even when the user simply needed clarification.

## Why it’s dangerous
- Users lose trust (“the AI is useless”).
- Humans get interrupted for no reason.
- Escalation becomes political theatre.

## What to do instead
Use **Mode B (Defer)** first when the blocker is missing information.

### Fix pattern
- Defer with a minimal ask:
  - “I need X and Y to proceed safely.”
- Escalate only when a human must own the decision boundary now.

## Recommended output shape
- What I know
- What I need (minimum)
- Next safe step
