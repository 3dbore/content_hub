# 3D BORE Content Making

Knowledge base for the AI agents that run the social media division of **3D BORE**, an online manufacturing brand (3D printing and CNC). It holds no application code. It holds the roles, brand rules and skills that tell each agent what to do and how to hand work to the next one.

Mission: *making manufacturing more open to anyone.* Content educates and builds trust first. Every piece ends with one soft pointer to 3D BORE's services, never a hard sell.

## The team

| Codename | Role | Model | Owns |
|---|---|---|---|
| **Fore** | Content Manager | Gemini | Plan, schedule, `STATUS.md`, final review |
| **Sudo** | Content Writer | Claude | Research, hooks, scripts, captions |
| **Jarvis** | Graphic Designer (Figma) | Claude | Visuals for Jarvis's series, reviews Comet |
| **Comet** | Graphic Designer (Figma) | Gemini | Visuals for Comet's series, reviews Jarvis |

The human owner (Reza, 3D BORE) approves anything published, any customer project, any promo or price, and any new logo use. Shooting and editing video are done by the human team.

To start a session, tell the agent **"You are `<codename>`"** (for example "You are Sudo"). It reads its own section of `agent-role.md`, then `STATUS.md` and its open handoffs.

## Repository layout

```
agent-role.md                        Agent roles, workflow, shared rules, handoff and status formats
DESIGN.md                            3D BORE design system (colors, type, spacing, components, agent rules)
skills/
  3dbore-content-series-brief.md     Brief: brand, voice, shared rules, series A/B/C, deliverable format, checklist
  3dbore-content-writer-skill.md     Earlier, English-first writer skill (see "Known gaps")
  fore/content-planning/SKILL.md     Planning, handoffs, STATUS.md, review checklist
  sudo/content-writer/SKILL.md       Plain casual Indonesian copy, carousels as one story
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
4. **Fore** checks the brief checklist, gets owner approval, schedules, and logs the post link and numbers.

### Files the agents create

These are created at runtime and are not in this repo yet.

| File | Purpose |
|---|---|
| `STATUS.md` | One overwritten file: this week's focus, each agent's next task, blockers, decisions |
| `handoff/<STATE>_<ID>_<FROM>-to-<TO>_<YYYYMMDD>.md` | Task passed between agents. States: `OPEN`, `WIP`, `BLOCKED`, `DONE` |
| `work/<ID>_<type>_v<N>.md` | Output files. Types: `research`, `script`, `caption`, `design-notes`, `report` |

Project files cannot be renamed, so a state change means writing the file under the new name and deleting the old one. `agent-role.md` has the full templates.

## Rules every agent follows

1. Never invent facts, numbers, prices, lead times, test results or customer details. Use placeholders such as `[HARGA]` or `[LINK]`.
2. Credit every creator and state the license. Customer projects need written permission.
3. Content language is casual Indonesian. Notes, handoffs and file names are English.
4. Follow the brand. If sources disagree, the BSG in Figma wins for visuals and the brief wins for content.
5. Items marked `[ASSUMPTION]` or "draft" are unconfirmed. Flag them.
6. Stay in role. Hand other work off with a handoff file.
7. Ask before anything that publishes, sends, spends money or changes a customer-facing page.
8. Keep the sheet and the context files in agreement.

## Brand at a glance

Full detail is in `DESIGN.md`.

- **Vibe:** sharp, minimal, modern.
- **Colors:** Cobalt Surge `#3065EF`, Midnight Navy `#001848`, Electric Chartreuse `#DBEB42`, Blush Pop `#FB4988`. Blush is never a background. No white text on Chartreuse or Blush.
- **Type:** Geom only, nine text styles, sentence-case headlines.
- **Layout:** spacing and radius from tokens, one graphic device and one idea per layout, real photos only.
- **Voice:** direct, open, precise, friendly.

Source of truth for visuals is the Figma file **3DBORE**, page "Brand Guidelines".

## Known gaps

- `skills/3dbore-content-writer-skill.md` conflicts with `skills/sudo/content-writer/SKILL.md`. It is English-first, aims at home builders and advanced prototypers, uses a Mon/Wed/Fri rhythm and a spec line plus disclaimer on every post. `agent-role.md` points Sudo at this filename, but the newer `SKILL.md` has the plain-Indonesian and carousel rules. Decide which one is current and retire or merge the other.
- `skills/comet/` duplicates `skills/jarvis/` byte for byte. Update both together or collapse them into one shared skill.
- `agent-role.md` names `STATUS.md`, `handoff/`, `work/` and `3DBORE-Brand_Style_Guides.pdf`. None of them are in this repo.
- The brief covers only MAF, BP and BY. WTR, NOS and BN rely on the sheet's Series tab.
- Carousel size is unconfirmed: the template is 1080x1440, but MAF-01 used 1080x1350. Ask the owner.
