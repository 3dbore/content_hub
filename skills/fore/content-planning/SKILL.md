---
name: content-planning
description: How Fore plans the content calendar, runs the sheet, STATUS.md and handoffs, and reviews work before the owner approves. Use for any planning, scheduling, status or review task.
---

# Content planning (Fore)

## 1. Planning
- Keep at least 4 weeks planned in the Content Plan tab, following the Series tab's posting days and cadences.
- Weekly slots: Mon WTR, Tue MAF, Wed NOS, Thu BY or BP (alternating), Fri BN. One-offs sit in open days and need an owner decision.
- Sheet time zone is Asia/Jakarta. Locale is Indonesian (formulas use semicolons).
- Fill every new row: ID, publish date, series, working title, status, priority, platform, format, audience, hook direction, key message, proof needed, CTA, notes. Do not type into grey-blue calculated columns.
- A new series needs a row on the Series tab first, because the dropdown reads column A.
- Lead times on the Series tab are planning assumptions in calendar days before publish.

## 2. Handoffs
Name: `handoff/<STATE>_<EPISODE-ID>_<FROM>-to-<TO>_<YYYYMMDD>.md` (states OPEN, WIP, BLOCKED, DONE). Keep under about 25 lines, link instead of pasting.
- Create an `OPEN_<ID>_FORE-to-SUDO_<date>.md` for each episode entering Research, in script-due order.
- Decisions only the owner can make go to `FORE-to-OWNER`.
- Fore does not hand off to the designers. Sudo does, after the script. Designers hand off to each other for review, then to Fore.
- To change state: write the same content under the new name, add a log line, then delete the old file.

## 3. STATUS.md
- Overwrite, never append. Under about 40 lines.
- Weekly: set "This week", each agent's "Next up" line and "Blocked". Others edit only their own line and add one log line (keep 8).
- Remove decisions that no longer apply.

## 4. Chasing
- Watch overdue episodes and scripts due within 3 days (pink dates in the sheet).
- Chase blocked items and owner questions. Customer projects need written permission (BP).
- If a Bedah Proyek has no customer project by the script due date, swap in a Benerin Yuk.

## 5. Review before approval (brief section 8)
- [ ] Hook or slide 1 lands in 3 seconds.
- [ ] Facts verified is ticked only when every claim has a source.
- [ ] No invented numbers, prices, lead times, tests or customer details (placeholders used).
- [ ] Creator and license credited. Customer permission confirmed (BP). No safety-critical repair (BY).
- [ ] Material choice matches use, with the reason stated.
- [ ] Voice direct, open, precise, friendly. Plain Indonesian (anak SMA test) and carousels read as one story.
- [ ] Design follows `DESIGN.md` section 12.
- [ ] One graphic device, one idea, one soft CTA.
- [ ] [ASSUMPTION] and draft items flagged.
- [ ] Owner approval received before Scheduled.

## 6. After publishing
- Fill Post link and performance numbers in the sheet.
- Write the weekly `work/GENERAL_report_v<N>.md`: published, late, top performer, next week's plan.
- Weekly cleanup: delete `DONE_` handoffs older than 7 days and superseded work versions, trim the log.

## 7. Never
- Write full scripts or design visuals.
- Approve customer projects, promos or prices for the owner.
- Publish, send or spend without asking first.
- Let the sheet and the context files disagree. If you change one, change or flag the other in the same session.
