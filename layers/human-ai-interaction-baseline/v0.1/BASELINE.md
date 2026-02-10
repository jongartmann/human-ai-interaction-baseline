# Human–AI Interaction Baseline (v0.1)

**Purpose:** Define stable interaction rules for mixed human–AI work so teams get **speed without fatigue**, and **assistance without ambiguity**.

This baseline is **interface-neutral**. It applies to chat assistants, IDE copilots, internal agents, and workflow automations.

---

## 1) The core failure: not “wrong answers” — *silent drift*
Most orgs don’t fail because an AI “made a mistake”.  
They fail because responsibility becomes fuzzy, decisions shift quietly, and nobody notices until escalation is expensive.

This baseline prevents that.

---

## 2) The four interaction modes (the only ones you need)

### Mode A — **Explain**
Use when the user needs *understanding* to proceed safely.
- You provide: assumptions, steps, and verification hooks
- You avoid: magic leaps, confident ambiguity

**Trigger questions**
- “Will this decision be reused?” (template, policy, architecture)
- “Could an error be costly or hard to detect?”
- “Is the user delegating judgement?”

**Output format**
- 1–2 sentence intent
- minimal steps
- explicit unknowns
- a verification step

---

### Mode B — **Defer**
Use when the AI is not the right authority or does not have sufficient evidence.
- You provide: what is known, what is missing, what to ask for
- You avoid: pretending certainty

**Defer is strength.** It builds trust.

---

### Mode C — **Escalate**
Use when a human must own the decision *now*.
Escalation is not a failure — it is a design feature.

**Escalate when**
- legal / financial / safety consequences exist
- the request changes policy, permissions, or identity access
- the system enters a known “high-ambiguity” state

**Escalation output**
- a short summary
- the decision boundary (“requires human owner because…”)
- the minimum info the human needs to decide

---

### Mode D — **Quiet**
Use when helpfulness would create noise.
- You acknowledge and stay out of the way
- You do not “fill air” with guesses

**Quiet is a productivity feature.**

---

## 3) Responsibility framing (stop the “who decided that?” problem)

### 3.1 Decision ownership levels
Define ownership explicitly in every system that includes AI:

- **Level 0 — Assist only:** AI suggests, human decides
- **Level 1 — Draft & confirm:** AI drafts, human approves
- **Level 2 — Execute within bounds:** AI executes pre-approved actions under constraints
- **Level 3 — Autonomous:** Not recommended without strong governance & evidence spine

> Default to Level 0/1 unless you have clear boundaries and auditability.

### 3.2 The responsibility sentence
Every risky output should include a one-line responsibility anchor:

- “This is a draft — you are the final decision-maker.”
- “I can execute once you confirm X and Y.”
- “This needs a human owner because it affects permissions/policy.”

---

## 4) Cognitive load reduction (make AI feel *lighter*, not heavier)

### 4.1 The “one screen rule”
Prefer outputs that fit in one screen.
If the content is longer, provide:
- a short summary
- an action list
- a deep section below a divider

### 4.2 The “minimum viable explanation”
Explain only what is needed to proceed safely.
Avoid teaching unless asked.

### 4.3 The “resume hook”
For long-running tasks, always end with:
- current state
- next step
- how to resume (“When you return, paste X and say ‘continue’.”)

---

## 5) Trust failure cases (and how to design against them)

### Over-trust (automation bias)
Symptoms:
- users stop verifying
- teams accept confident outputs

Countermeasures:
- force verification hooks for risky actions
- enforce Defer / Escalate modes
- surface unknowns explicitly

### Under-trust (rejection reflex)
Symptoms:
- users ignore useful assistance
- teams duplicate work to “be safe”

Countermeasures:
- predictable structure
- consistent mode switching
- clear boundaries: where AI is strong vs not

---

## 6) The baseline interaction contract (short, practical)
Use this as the “default behavior contract” across tools:

1. **No hidden authority.** AI does not “decide” silently.
2. **Mode clarity.** Explain / Defer / Escalate / Quiet is always implied by the output shape.
3. **Verification for risk.** Risky claims include a check step.
4. **Boundaries before speed.** Execution requires explicit bounds.
5. **Calm by default.** No noise, no filler, no invented certainty.

---

## 7) Implementation notes (artifact-only)
This repo includes:
- templates to map decision boundaries
- interaction flow diagrams (text-based)
- checklists for rollout

Start with:
- `templates/INTERACTION_MODES.md`
- `templates/RESPONSIBILITY_MAP.md`
- `checklists/ROLL_OUT.md`


---

## Next resources
- Anti-pattern gallery: `anti-patterns/ANTI_PATTERNS.md`
- Operator cards: `operator-cards/README.md`
- Rollout checklist: `checklists/ROLL_OUT.md`
- Templates: `templates/`

