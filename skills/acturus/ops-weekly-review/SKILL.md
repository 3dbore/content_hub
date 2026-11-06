---
name: ops-weekly-review
description: How Acturus runs the weekly business review - orders and delivery, capacity, cash inputs, compliance, risks, expansion progress and owner decisions. Use every Sunday, or when the owner asks how the business is doing.
---

# Weekly business review (Acturus)

Fore reports on content (published, late, top performer). Acturus reports on the business: orders, delivery, capacity, risk and expansion. Do not duplicate Fore's report. Link to it for the content view.

## 1. Inputs (open only these)
- `STATUS.md` (Blocked, Decisions).
- `work/GENERAL_ops-facts_v<N>.md` and `work/GENERAL_expansion-plan_v<N>.md`.
- Sheet Overview tab: planned vs published, views and engagement (the demand signal).
- Fore's latest `work/GENERAL_report_v<N>.md`.
- Numbers from the owner or the workshop (section 2). If a number was not given, write `[not provided]`. Never estimate.

## 2. Numbers to ask the owner for each week
| Area | Metric |
|---|---|
| Intake | Inquiries (WhatsApp, DM, marketplace), files received, quote requests |
| Quoting | Quotes sent, reply time, quote-to-order rate |
| Production | Orders completed, on time vs promised date, print hours, reprints and reasons |
| Quality | Complaints, parts that failed fit, refunds |
| Machines | Downtime, spare parts, utilization |
| Money | Revenue and cost, only if the owner shares them |

## 3. Checks
1. **Capacity vs demand:** compare provided utilization and backlog with the stage-gate triggers in the expansion plan. Say "trigger reached" or "not reached". The owner decides what to buy.
2. **Delivery risk:** late orders, repeat complaints, single-machine exposure.
3. **Compliance:** customer permission on file, licenses respected, disclaimers and confidentiality in place for orders. Not legal advice.
4. **Calendar:** next 14 days of business dates (Harbolnas 11.11 and 12.12, gajian, school terms, KRI, Ramadan) and any owner decision needed before them.
5. **Expansion progress:** each workstream's next step, date and blocker.
6. **Old blocked items:** any `BLOCKED_` handoff to the owner or Acturus older than 3 days.

## 4. Output
Write `work/GENERAL_ops-review_v<N>.md`, under 40 lines:
```
# Business review <YYYYMMDD>
Health: GREEN / AMBER / RED  (one line why)
## Numbers (owner-provided, [not provided] where missing)
## Capacity vs demand
## Expansion progress
## Compliance and risks (top 3)
## Decisions needed from the owner (with date)
## Next week
```
Use RED only when the business cannot deliver an existing commitment, or a legal or permission gap exists. Then also open a `BLOCKED_GENERAL_ACTURUS-to-OWNER_<date>.md` with the single decision needed.

## 5. After the review
- Update your line in `STATUS.md` and add one log line (keep the last 8).
- Hand register changes to the owner for confirmation. Sheet cell changes go to Fore with the exact cell and value.

## 6. Never
- Estimate revenue, utilization, lead times or conversion.
- Make a purchasing, pricing, promo or hiring decision, or contact customers, suppliers or partners.
