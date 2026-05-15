# RICE Prioritization Framework

**Formula:** RICE Score = (Reach × Impact × Confidence) / Effort

---

## Scoring Definitions

### Reach
Estimated number of users affected per quarter.

- Count only users who hit this feature, not total user base
- Use data where possible; estimate conservatively where not

### Impact
How much does this move your key metric per user who encounters it?

| Score | Meaning |
|---|---|
| 3 | Massive impact |
| 2 | High impact |
| 1 | Medium impact |
| 0.5 | Low impact |
| 0.25 | Minimal impact |

### Confidence
How confident are you in your Reach and Impact estimates?

| Score | Meaning |
|---|---|
| 100% | Strong data backing |
| 80% | Some data, some assumption |
| 50% | Mostly assumption |
| 20% | Pure guess |

### Effort
Estimated person-weeks across all functions (design, eng, PM).

---

## Template

| Feature | Reach | Impact | Confidence | Effort | RICE Score | Priority |
|---|---|---|---|---|---|---|
| [Feature 1] | | | % | | | |
| [Feature 2] | | | % | | | |

**Formula reminder:** `(Reach × Impact × Confidence%) / Effort`

---

## Worked Example

| Feature | Reach | Impact | Confidence | Effort | RICE Score |
|---|---|---|---|---|---|
| Checkout progress bar | 800 | 1 | 80% | 1 | **640** |
| Guest checkout | 300 | 3 | 90% | 3 | **270** |
| Saved payment methods | 500 | 2 | 70% | 4 | **175** |
| Social login | 400 | 0.5 | 60% | 3 | **40** |

**Decision:** Checkout progress bar first (highest RICE), then guest checkout.

---

## When RICE Fails

RICE is a useful first filter. It breaks down when:

1. **Existential risks** — A feature that prevents a catastrophic failure (security, trust) should be P0 regardless of score
2. **Strategic bets** — Some features matter because of *what you learn*, not just metric impact
3. **Dependencies** — A low-RICE feature might be required to unlock a high-RICE one
4. **Asymmetric downside** — A low-cost, high-catastrophe-prevention feature always wins

**Rule:** RICE is an input, not a verdict. Use it to structure the conversation, not end it.

---

## Common Mistakes

- Overconfidence — Most estimates deserve 50–60% confidence, not 90%
- Ignoring effort — A 10-point RICE score for 1 week of work beats a 50-point score for 10 weeks
- Comparing features at different stages — Don't score a well-understood feature against an undefined one
- Using RICE to justify decisions already made — If you're working backwards from a conclusion, the exercise is theater