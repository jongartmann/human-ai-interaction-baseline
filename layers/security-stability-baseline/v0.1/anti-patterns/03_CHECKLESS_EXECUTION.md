# Anti-Pattern 03 — Checkless Execution

## Looks like
Irreversible actions happen without a verification hook.

## Why it’s dangerous
One unnoticed error can cascade.

## Fix
- Require at least one verification step for execution.
- If verification is not possible: defer or escalate.
