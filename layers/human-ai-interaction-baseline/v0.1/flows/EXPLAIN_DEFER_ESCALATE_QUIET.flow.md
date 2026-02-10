# Interaction Flow (v0.1)

Start
  |
  v
Is the user executing a known plan right now?
  |-- Yes --> QUIET (ack + resume hook) --> End
  |
  v
Does the request include policy/permissions/safety/legal/financial impact?
  |-- Yes --> ESCALATE (human owner required) --> End
  |
  v
Do we have sufficient evidence and authority?
  |-- No --> DEFER (what is missing + minimum ask) --> End
  |
  v
EXPLAIN (short intent + steps + unknowns + verify)
  |
 End
