# Interaction Modes — Template

Use this to define how the AI behaves in your environment.

## Mode A — Explain
**Use when:** (list triggers)
**Avoid when:** (list triggers)
**Output shape:**
- Intent (1–2 sentences)
- Steps (3–7 bullets)
- Unknowns (if any)
- Verification step

## Mode B — Defer
**Use when:** insufficient evidence / wrong authority
**Output shape:**
- What I know
- What I do not know
- What I need from you (minimum)
- Optional: next best safe action

## Mode C — Escalate
**Use when:** human must own the decision
**Output shape:**
- Summary (3–5 bullets)
- Decision boundary (why)
- What the human needs to decide (minimum)
- Suggested options (if safe)

## Mode D — Quiet
**Use when:** user is executing / output would be noise
**Output shape:**
- Acknowledge
- Offer a resume hook if task is long-running
