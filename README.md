# 3D BORE Content Making

Knowledge base for the AI agents that run the social media division and the business side of **3D BORE**, an online manufacturing brand (3D printing with a Bambu Lab A1, and CNC). It holds no application code. It holds the roles, brand rules and skills that tell each agent what to do and how to hand work to the next one.

Mission: *making manufacturing more open to anyone.* Content educates and builds trust first. Every piece ends with one soft pointer to 3D BORE's services, never a hard sell.

## The team

| Codename | Role | Model | Owns |
|---|---|---|---|
| **Acturus** | VP of Operations | Claude | Business operations, expansion plan, business facts register, compliance and risk, weekly business review |
| **Harvey** | Legal Team Assistant | Claude | Drafts of policies, terms of service, agreements and consent texts; legal risk notes; lawyer review pack |
| **Fore** | Content Manager (Social Media general manager) | Gemini | Plan, schedule, `STATUS.md`, final review, business claims check |
| **Sudo** | Content Writer | Claude | Research, hooks, scripts, captions |
| **Jarvis** | Graphic Designer (Figma) | Claude | Visuals for Jarvis's series, reviews Comet |
| **Comet** | Graphic Designer (Figma) | Gemini | Visuals for Comet's series, reviews Jarvis |

Fore, Sudo, Jarvis and Comet are the Social Media Division. Acturus and Harvey work with it but do not run it.

The human owner (Reza, 3D BORE) approves anything published, any customer project, any promo or price, any purchase, hire or partnership, any legal document, and any new logo use. Shooting and editing video are done by the human team.

To start a session, tell the agent **"You are `<codename>`"** (for example "You are Sudo"). It reads its own section of `agent-role.md`, then `STATUS.md` and its open handoffs.

## Repository layout

```
agent-role.md                        Agent roles, workflow, shared rules, handoff and status formats
STATUS.md                            Current progress snapshot (overwritten by the agents; see note below)
DESIGN.md                            3D BORE design system (colors, type, spacing, components, agent rules)
skills/
  3dbore-content-series-brief.md     Brief: brand, voice, shared rules, series A/B/C, deliverable format, checklist
  3dbore-content-writer-skill.md     Earlier, English-first writer skill (see "Known gaps")
  acturus/expansion-planning/        Lead the owner's expansion plan: options, gates, decision memos
  acturus/business-facts/            Keep the business facts register, answer factual questions
  acturus/ops-playbook/              Operating knowledge from the Drive documents (all PROPOSED)
  acturus/ops-weekly-review/         Weekly business review
  harvey/policy-drafting/            How to draft policies, terms and agreements
  harvey/legal-doc-library/          Documents needed, priority order, facts needed from the owner
  harvey/legal-risk-and-review/      Legal questions, red flags, lawyer review pack
  fore/content-planning/SKILL.md     Planning, handoffs, STATUS.md, review checklist, business claims check
  sudo/content-writer/SKILL.md       Plain casual Indonesian copy, carousels as one story, completion report
  jarvis/carousel-design/SKILL.md    Build carousels in Figma from the BSG
  jarvis/design-review/SKILL.md      Peer review checklist for Figma frames
  comet/carousel-design/SKILL.md     Same as the Jarvis copy
  comet/design-review/SKILL.md       Same as the Jarvis copy
```

## Content series

| Series | Prefix | Day | Brief section |
|---|---|---|---|
| WEEKLY TECH RECAP | WTR | Monday | Not written yet |
| MITOS ATAU FAKTA | MAF | Tuesday | 4 |
| NGOMONGIN OPEN-SAUCE | NOS | Wednesday | Not written yet |
| BENERIN YUK | BY | Thursday (alternating) | 6 |
| BEDAH PROYEK | BP | Thursday (alternating) | 5 |
| BUILDERNERRY | BN | Friday | Not written yet |

The Content Planning Google Sheet is the record of every episode. Its Series tab is the current source for concept, audience, hook pattern, CTA and lead times.

## How work flows

One episode moves through these hands:

```
FORE -> SUDO -> JARVIS or COMET -> the other designer (review) -> FORE -> owner approval -> publish
```

1. **Fore** plans the episode and opens a handoff to Sudo.
2. **Sudo** researches, verifies facts, then writes the script package (episode plan, script table, caption pack, production notes). Carousels start with a "Cerita singkat" paragraph.
3. **The series' primary designer** builds the visuals in Figma. The other designer reviews.
4. **Fore** checks the brief checklist and the business claims, gets owner approval, schedules, and logs the post link and numbers.

Two side lanes:
- **Business facts and expansion:** Acturus keeps the facts register (what 3D BORE offers, routes, prices; each line CONFIRMED, PROPOSED or OPEN) and leads the owner's expansion plan. Other agents ask him for facts and use a placeholder until a line is CONFIRMED.
- **Legal documents:** the owner asks Harvey for a policy, terms or agreement. He drafts it from the register's CONFIRMED facts. Everything stays DRAFT until the owner approves and a qualified lawyer reviews. Other agents never write legal wording themselves.

### Files the agents create

These are created at runtime in the Claude project (under its `claude/` folder). `STATUS.md` is copied into this repo as a snapshot. The `handoff/` and `work/` files are not.

| File | Purpose |
|---|---|
| `STATUS.md` | One overwritten file: this week's focus, each agent's next task, blockers, decisions |
| `handoff/<STATE>_<ID>_<FROM>-to-<TO>_<YYYYMMDD>.md` | Task passed between agents. States: `OPEN`, `WIP`, `BLOCKED`, `DONE`. FROM and TO: `FORE`, `SUDO`, `JARVIS`, `COMET`, `ACTURUS`, `HARVEY`, `OWNER` |
| `work/<ID>_<type>_v<N>.md` | Output files. Types: `research`, `script`, `caption`, `design-notes`, `report`, `ops-facts`, `ops-review`, `expansion-plan`, `legal-<slug>` |
| `work/GENERAL_ops-facts_v<N>.md` | The business facts register (Acturus) |
| `work/GENERAL_expansion-plan_v<N>.md` | The owner's expansion plan (Acturus) |
| `work/GENERAL_legal-<slug>_v<N>.md` | Legal drafts (Harvey) |

Project files cannot be renamed, so a state change means writing the file under the new name and deleting the old one. `agent-role.md` has the full templates.

## Rules every agent follows

1. Never invent facts, numbers, prices, lead times, test results or customer details. Use placeholders such as `[HARGA]` or `[LINK]`.
2. Credit every creator and state the license. Customer projects need written permission.
3. Content language is casual Indonesian. Notes, handoffs and file names are English. Customer legal documents are plain Indonesian.
4. Follow the brand. If sources disagree, the BSG in Figma wins for visuals and the brief wins for content.
5. Items marked `[ASSUMPTION]` or "draft" are unconfirmed. Flag them.
6. Stay in role. Hand other work off with a handoff file.
7. Ask before anything that publishes, sends, spends money or changes a customer-facing page.
8. Keep the sheet and the context files in agreement.
9. Read little, write little.
10. Business facts come from the register. Do not promise a material, price, discount, turnaround, link or quote route that is not CONFIRMED.
11. Legal wording comes from Harvey. Do not write terms, policies or disclaimers yourself, and do not say something is legal or illegal.

## Brand at a glance

Full detail is in `DESIGN.md`.

- **Vibe:** sharp, minimal, modern.
- **Colors:** Cobalt Surge `#3065EF`, Midnight Navy `#001848`, Electric Chartreuse `#DBEB42`, Blush Pop `#FB4988`. Blush is never a background. No white text on Chartreuse or Blush.
- **Type:** Geom only, nine text styles, sentence-case headlines.
- **Layout:** spacing and radius from tokens, one graphic device and one idea per layout, real photos only.
- **Voice:** direct, open, precise, friendly.

Source of truth for visuals is the Figma file **3DBORE**, page "Brand Guidelines".

## Known gaps

- `skills/3dbore-content-writer-skill.md` here is the earlier English-first version. The Claude project holds a newer plain-Indonesian version at `claude/3dbore-content-writer-skill.md` (same rules as `skills/sudo/content-writer/SKILL.md`). `agent-role.md` points Sudo at that filename. Replace this copy with the project's newer file, or retire it in favor of the `SKILL.md`.
- `skills/comet/` duplicates `skills/jarvis/` byte for byte. Update both together or collapse them into one shared skill.
- `STATUS.md` here is a snapshot from 20261106 and goes stale quickly. The live copy is in the Claude project.
- `handoff/`, `work/` (including the facts register, expansion plan and legal drafts) and `3DBORE-Brand_Style_Guides.pdf` are not in this repo.
- The brief covers only MAF, BP and BY. WTR, NOS and BN rely on the sheet's Series tab.
- Carousel size is unconfirmed: the template is 1080x1440, but MAF-01 used 1080x1350. Ask the owner.
