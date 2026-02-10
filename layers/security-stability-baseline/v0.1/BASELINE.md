# Security & Stability Baseline (v0.1)

**Purpose:** Provide a practical baseline to prevent **silent failure**, reduce **drift risk**, and keep responsibility visible when AI is part of real workflows.

This is **artifact-only** and **interface-neutral**. It applies to chat assistants, IDE copilots, internal agents, and workflow automations.

---

## 1) The enemy: silent failure
Most incidents are not explosions. They are **quiet degradations**:
- small assumption errors
- boundary creep
- unnoticed responsibility shifts
- “works most of the time” behavior that accumulates debt

A stable system makes failure **loud early**.

---

## 2) The stability triad
A practical baseline needs only three pillars:

1. **Boundaries** — what the system may do (and may not do)
2. **Ownership** — who must decide, approve, and be accountable
3. **Evidence** — what must be true before action is taken

If any of these are implicit, drift is inevitable.

---

## 3) Decision boundaries (make them visible)
Define boundaries as a map, not a paragraph.

### 3.1 Boundary classes
- **B0 — Informational:** advice only, no execution
- **B1 — Drafting:** generates drafts, requires human approval
- **B2 — Execution within bounds:** executes only pre-approved actions under explicit constraints
- **B3 — Autonomous:** not recommended without strong governance & auditing

> Default to B0/B1. Move to B2 only after you can prove control.

### 3.2 Boundary statement
Every risky output should include one line that clarifies boundary & ownership:
- “Draft only — you are the decision owner.”
- “Execution requires confirmation of X and Y.”
- “This crosses a boundary (permissions/policy/safety) → escalation required.”

---

## 4) Escalation paths (remove ambiguity)
Escalation must be **predictable** and **low-friction**.

### 4.1 Escalation triggers (must be explicit)
Escalate when:
- permissions / identity / access are affected
- money / procurement / billing is affected
- safety / legal / compliance impact exists
- policy or operating rules change
- the system lacks evidence (and guessing would be risky)

### 4.2 Escalation output shape
- Summary (3–5 bullets)
- Boundary (“requires human owner because…”)
- Minimum info needed to decide
- Safe options (only if evidence supports them)

---

## 5) Verification hooks (turn risk into checks)
For any action that can cause harm or costly mistakes:
- require **one verification step**
- prefer **simple, local checks** over long arguments

Examples (interface-neutral):
- “Verify by checking X in system Y.”
- “Confirm that Z is true before executing.”
- “If you cannot verify, escalate.”

---

## 6) Failure mode taxonomy (simple and usable)

### F1 — Evidence gap
You do not have what you need to be confident.

### F2 — Boundary creep
System actions expand beyond intended scope.

### F3 — Authority confusion
The AI implies decisions it does not own.

### F4 — Latent drift
Behavior slowly changes, nobody notices.

### F5 — Ambiguity pressure
Inputs are underspecified; system tries to “be helpful” by guessing.

---

## 7) Kill switch (design-only, non-theatrical)
A “kill switch” is not a big red button. It is a clean state transition:
- stop execution
- preserve minimal evidence
- hand off to a human owner
- resume only with explicit confirmation

Kill switch is successful when it is boring.

---

## 8) Rollout baseline (practical)
Start with:
- Boundary map (B0/B1)
- Escalation triggers
- Verification hook policy (what requires checks)
- Monthly sample review (small, consistent)

This baseline ships stability by design—without over-promising.

---

## Next resources
- Templates: `templates/`
- Anti-pattern gallery: `anti-patterns/ANTI_PATTERNS.md`
- Operator cards: `operator-cards/README.md`
- Rollout checklist: `checklists/ROLL_OUT.md`
- Flow: `flows/BOUNDARY_ESCALATION_VERIFY.flow.md`

