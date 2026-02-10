# Operator Card — VERIFICATION

## Purpose
Prevent costly or unsafe actions caused by unchecked assumptions.

## Use when
- execution is irreversible
- impact is high
- errors would be hard to detect later

## Do
- require at least one verification hook
- keep checks concrete and local
- route “cannot verify” to defer or escalate

## Template
Claim / Action  
→ What must be true  
→ How to verify  
→ If verification fails

## Avoid
- long arguments instead of checks
- proceeding “because it’s probably fine”
