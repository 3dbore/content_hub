---
name: legal-doc-library
description: The list of legal documents 3D BORE needs, in priority order, with what each must cover and which facts are needed from the owner. Use to plan which policy or terms to draft first and to build the "Facts needed" list.
---

# Legal document library (Harvey)

Starting points come from the Drive strategy doc (compliance section), the Instagram plan (Universal Disclaimer) and the brief (permission, credit, safety rules). All are inputs to check, not legal conclusions. Verify any law with a current source before citing it (see `policy-drafting` section 3).

## Priority 1: needed before orders grow
| Document | Slug | Must cover | Starting point |
|---|---|---|---|
| Terms of Service for custom orders (WhatsApp and DM) | `tos` | What is offered (FDM printing in PLA, PETG, TPU), how a quote works and how long it is valid, price basis, payment, production time, file requirements, customer's promise that they have rights to the file, revisions and reprints, fit and tolerance notes, shipping and packaging, cancellation, refunds, liability limits, confidentiality, IP, how to complain | Strategy doc sections 5 and 6; register sections 1 to 3 |
| Privacy policy and data consent | `privacy` | What data is collected (name, phone, address, files, chats, photos), why, who sees it (courier, Shopee), how long it is kept, how it is protected, how a person can ask to see, correct or delete it, who to contact, what happens if there is a breach | UU PDP topic list in the strategy doc (to verify) |
| Product and use disclaimer | `disclaimer` | FDM parts are for prototypes and functional validation. Final strength testing for higher-risk uses is the customer's responsibility. No safety-critical parts | Proposed wording in `ops-playbook` section 4 and brief 6.6 |

## Priority 2: needed when content or Shopee goes live
| Document | Slug | Must cover | Starting point |
|---|---|---|---|
| IP and license policy | `ip-license` | Which third-party files can be made or shown (CC0, CC BY, CC BY-SA, CC BY-NC), credit rules, customer warranty, what happens on a rights complaint | Strategy doc license table; brief 3.2 |
| Permission and release form | `permission` | Written permission to show a customer project, what may be shown, credit, the Universal Disclaimer, how to withdraw | Brief 3.2 and 5.5; Instagram plan disclaimer text |
| Shopee shop policy text | `shopee` | Shop description, order and production time, returns and cancellation as the platform allows, packaging, contact route | Shopee's current seller policy (check the live page). Owner will brief the shop details |

## Priority 3: when the offer exists
| Document | Slug | Must cover | Starting point |
|---|---|---|---|
| Mutual NDA (template) | `nda` | Confidential information, use limits, duration, return or deletion of files, exceptions | Strategy doc risk table |
| Collaboration and barter agreement | `collab` | Deliverables, approval, usage rights, #Endorse or #Iklan disclosure, free parts as payment, termination | Strategy doc community section (EPI rule to verify). Needs an owner-approved offer |
| Student discount terms | `student-terms` | Who qualifies, proof, what the discount covers, dates | Strategy doc proposes 15%. The owner has not approved it |
| Giveaway or promo terms | `promo` | Only if the owner runs one | No promo is planned (no 11.11 promo; 12.12 undecided) |

## Facts needed from the owner (ask Acturus to collect them)
| Fact | Needed for | Register status on 20261106 |
|---|---|---|
| Legal form and name of the business (individual, CV, PT), address, registration number | all | Not in the register |
| Price basis (per gram of finished part), setup fee, minimum order, rush charge, packaging cost | `tos`, `shopee` | Range confirmed; formula open |
| Payment methods and when payment is due | `tos` | Proposed |
| Production time promise and quote reply time | `tos`, `shopee` | Open (reply time proposed) |
| Cancellation, refund and reprint rules | `tos`, `shopee` | Not in the register |
| What counts as a defect and the claim period | `tos` | Not in the register |
| Liability limit the owner wants | `tos`, `disclaimer` | Not in the register |
| Shipping partners and who pays | `tos`, `shopee` | Open (Shopee details later) |
| Data collected, where it is stored, who can access it, how long it is kept | `privacy` | Not in the register |
| Place of dispute resolution and governing law wording | `tos`, `nda` | Lawyer to advise |
| Whether the price can be public | `tos`, `shopee` | Open |

## Suggested drafting order
1. `disclaimer` and `privacy` consent line (short, needed first).
2. `tos` (main document, uses the other two).
3. `shopee`, `ip-license`, `permission`.
4. `nda`, `collab`, `student-terms` when asked.
