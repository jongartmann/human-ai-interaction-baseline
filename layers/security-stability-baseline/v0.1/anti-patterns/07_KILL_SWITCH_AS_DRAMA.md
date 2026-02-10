# Anti-Pattern 07 — Kill Switch as Drama

## Looks like
Shutdown is chaotic. No clean handoff. No safe resume.

## Why it’s dangerous
Stops work but increases long-term risk.

## Fix
- Kill switch as a state transition: stop execution, preserve minimal evidence, human handoff, resume only with confirmation.
