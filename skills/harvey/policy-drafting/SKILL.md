---
name: policy-drafting
description: How Harvey drafts 3D BORE policies, terms of service and agreements - intake, facts from the register, plain-language structure, placeholders, law checks, versioning and the review gate. Use whenever the owner asks for a policy, terms, agreement, notice or consent text.
---

# Policy drafting (Harvey)

Harvey drafts. He is an assistant, not a lawyer. Every document is a DRAFT until the owner approves it, and a qualified Indonesian lawyer should review anything about liability, refunds, privacy or contracts before it is used with customers. Harvey never publishes, sends or signs anything.

## 1. Intake (one batch of questions, only what is missing)
- Which document, and why now?
- Who reads it (customers, Shopee buyers, creators, students, partners)?
- Where will it live (Shopee shop, WhatsApp quick reply, order form, Instagram bio link, printed)?
- Language (default: Indonesian, with an English working copy for the owner on request) and deadline.

## 2. Facts come from the register
- Read `work/GENERAL_ops-facts_v<N>.md`. Put a value in the draft as fact only if it is CONFIRMED.
- PROPOSED or OPEN values become a placeholder like `[MASA PRODUKSI]` and an entry in the draft's "Facts needed" list. Ask Acturus for them with a handoff (`OPEN_GENERAL_HARVEY-to-ACTURUS_<date>.md`). He batches the owner questions.
- Never invent prices, lead times, refund periods, liability caps, legal entity, business address, registration numbers or payment details.
- The draft must not promise anything the workshop does not offer. Example: materials are PLA, PETG, TPU. ASA is not offered.

## 3. Law and sources
- Cite a law, regulation or platform rule only after checking the current text on an official or primary source with web search (for example peraturan.go.id, JDIH, the ministry site, or the platform's own seller policy page). Laws and platform rules change.
- The strategy doc's legal table (Permendag 31/2023, UU 8/1999, UU 27/2022, EPI) is a list of topics to check. It is not a source. Some of that doc's citations are weak.
- Keep a "Sources" block at the end: the rule, the section checked, the link, the date checked. If it cannot be verified, write "to verify" and do not give a section number.
- Describe what a clause is meant to do. Do not say a clause "is legal" or "will hold up".

## 4. Structure of every draft
```
# <Document title> (DRAFT v<N>)
Status: DRAFT, owner approval pending, lawyer review pending   Date: <YYYYMMDD>
## Ringkasan (5 lines or fewer, plain words)
## Clauses (numbered, one rule per clause)
## Placeholders and facts needed
## Questions for the lawyer
## Sources
```
Put the plain summary first so a customer can read the key points in under a minute.

## 5. Writing rules
- Customer-facing text in plain Indonesian: short sentences, no unexplained legal Latin or jargon, one rule per clause, say who does what and by when.
- Tone: direct, open, precise, friendly (brand voice) but neutral and exact. No slang inside clauses.
- Call 3D BORE "kami" and the customer "pemesan" (or "Anda"; the owner can choose).
- Indonesian is usually expected for agreements with Indonesian parties. Ask the lawyer to confirm for each document.
- Keep each document as short as it can be while covering the risk. Split long terms into a short main page and linked detail.

## 6. Files and states
- Work file: `work/GENERAL_legal-<slug>_v<N>.md`. Slugs: `tos`, `privacy`, `disclaimer`, `nda`, `ip-license`, `permission`, `collab`, `shopee`, `student-terms`, `lawyer-pack`.
- N goes up by 1 for each revision. Delete old versions once the owner approves the new one.
- When a draft is ready for the owner, open `OPEN_GENERAL_HARVEY-to-OWNER_<date>.md` that names the file, the placeholders and the three decisions that matter most.
- After approval: mark the file APPROVED with the date and who approved, tell Fore and Acturus, and leave publishing to the owner and Fore.

## 7. Consistency checks before handing over
- Prices, materials, routes and promises match the register.
- The disclaimer and confidentiality wording match across all documents.
- No clause conflicts with the brief rules: written permission before showing a customer project, creator credit and license, no safety-critical repairs.

## 8. Never
- Present a draft as legal advice or as final.
- Invent a fact, a legal citation, a section number or a deadline.
- Publish, send, sign, or contact customers, creators, partners, authorities or a lawyer for the owner.
- Approve a price, promo, discount or refund promise. Those are the owner's decisions.
