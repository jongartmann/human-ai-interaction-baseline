# Boundary → Escalation → Verification Flow (v0.1)

Start
  |
  v
Does this affect permissions / identity / access / money / safety / legal / policy?
  |-- Yes --> ESCALATE (human owner required) --> End
  |
  v
Do we have sufficient evidence to proceed without guessing?
  |-- No --> DEFER (minimum ask) OR ESCALATE (if high risk) --> End
  |
  v
Is the action execution or irreversible change?
  |-- Yes --> Require verification hook --> Execute within bounds --> End
  |
  v
Provide informational guidance (B0) or draft (B1)
  |
 End
