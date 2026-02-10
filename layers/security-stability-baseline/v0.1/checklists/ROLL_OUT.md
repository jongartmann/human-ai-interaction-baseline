# Rollout Checklist (Security & Stability) — v0.1

## Day 0 — Boundaries
- [ ] Set boundary level (B0/B1 by default)
- [ ] Create boundary map (allowed/forbidden actions)
- [ ] Define explicit escalation triggers

## Day 1 — Verification
- [ ] Define which actions require verification hooks
- [ ] Standardize verification format
- [ ] Ensure “cannot verify” routes to defer or escalate

## Day 2 — Evidence & review
- [ ] Define minimal evidence to preserve
- [ ] Review a small interaction sample monthly
- [ ] Update boundary map on exceptions

## Ongoing
- [ ] Treat boundary creep as a defect
- [ ] Keep escalation boring and usable
- [ ] Keep kill switch as a clean state transition
