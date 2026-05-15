# Decision Log

A running record of significant product decisions. Log decisions when they're made — not retroactively.

---

## How to Use This Log

**What to log:** Decisions that took real trade-offs. If there was an obvious right answer, it doesn't belong here.

**When to log:** At the time of the decision, not after the outcome is known.

**Why it matters:** Future-you (and teammates) will question past choices. A log shows you made deliberate decisions, not arbitrary ones.

---

## Template: Single Entry

```
## Decision #[N] — [Short description]

**Date:** [YYYY-MM-DD]
**Decision:** [One sentence stating exactly what was decided]
**Status:** Active / Superseded by Decision #N / Reversed

**Alternatives considered:**
- [Option A] — [Why rejected]
- [Option B] — [Why rejected]
- [Option C — chosen] — [Why selected]

**Rationale:** [2–4 sentences explaining the reasoning. Focus on trade-offs, not just benefits.]

**Reversible if:** [What specific signal or data would cause you to reverse this decision?]

**Owner:** [Name]
```

---

## Example Entry

## Decision #1 — Set free tier storage limit at 5GB

**Date:** 2026-01-15  
**Decision:** Free tier users get 5GB storage, not 10GB  
**Status:** Active

**Alternatives considered:**
- 2GB — Too restrictive; users hit limit before experiencing value
- 5GB — Allows meaningful use; comparable to Google Drive free tier
- 10GB — High infrastructure cost before any monetization signal
- Unlimited — Non-starter for unit economics

**Rationale:** 5GB allows a new user to store ~3 months of typical project files before hitting a limit — long enough to form a habit and evaluate upgrade. Dropping from 10GB saves meaningful infrastructure cost without significantly affecting trial quality.

**Reversible if:** Free-to-paid conversion rate drops below 3% AND exit surveys cite storage limits as a reason (indicating we're driving away users, not converting them).

**Owner:** [PM Name]

---

## Active Decisions

*Add entries here as decisions are made.*