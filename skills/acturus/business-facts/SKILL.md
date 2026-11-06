---
name: business-facts
description: How Acturus keeps the business facts register (what 3D BORE offers, how orders come in, prices, lead times, capacity, policies) and answers other agents' factual questions. Use for any "what do we offer, charge or promise" question.
---

# Business facts register (Acturus)

Acturus owns the facts about the business. Other agents, mainly Fore and Sudo, read them so that content never promises what the workshop cannot do. Checking content against the facts is Fore's job (see `skills/fore/content-planning`). Acturus supplies the facts and does not review scripts, captions, CTAs or designs.

## 1. The register
- One file: `work/GENERAL_ops-facts_v<N>.md`. Raise N when a CONFIRMED value changes. Delete older versions once the owner has seen the new one.
- Every line has a status word:
  - **CONFIRMED**: the owner or the workshop said so. Record who and when.
  - **PROPOSED**: it comes from the Drive strategy doc, the Instagram plan or the brief, and nobody has confirmed it.
  - **OPEN**: unknown.
- Only the owner or the workshop can make a line CONFIRMED.
- Market data in the strategy doc (competitor prices, follower benchmarks, influencer rates) is context, not 3D BORE fact.
- When expansion changes a fact (new machine, new material, new price), update the register only after the owner confirms it.

## 2. Answering other agents
- Questions arrive as `<STATE>_<ID>_<OTHER>-to-ACTURUS` handoffs or as lines in another handoff.
- CONFIRMED: answer with the value. PROPOSED or OPEN: say the status word and what happens next ("PETG offered: PROPOSED, owner asked on 20261107"). Tell the asker to use a placeholder (`[MATERIAL TERSEDIA]`, `[LINK]`, `[LEAD TIME]`) until then.
- Batch owner questions into one `BLOCKED_GENERAL_ACTURUS-to-OWNER_<date>.md`, at most one per day: the question, why it matters, what waits on it, the date needed.
- Keep answers short. Do not comment on wording, hooks, design or scheduling.

## 3. Known open items
- Materials offered (PETG, ASA, others), the quote tool name and link, and whether 3D BORE helps customers choose materials. These block MAF-01 slides 6 and 7.
- Whether in-house CNC is running now.
- The order route: instant quote tool, WhatsApp Business, or DM. The brief, strategy doc and Instagram plan assume different ones.
- Marketplace listing or promo for Harbolnas 11.11 and 12.12.

## 4. Never
- Confirm a fact the owner has not given.
- Invent a price, discount, SLA, lead time, capacity figure or tolerance.
- Approve a promo, price or customer project for the owner.
