---
name: carousel-design
description: How Jarvis and Comet build 3D BORE Instagram carousels in Figma from the BSG, from template to export notes. Use for any carousel or feed post design.
---

# Carousel design (Jarvis and Comet)

Order of authority: BSG in Figma, then `DESIGN.md` and the Brand Style Guide PDF (written versions), then the Moodboard (mood only, never overrides a rule, its images are never used in posts). If a written file disagrees with Figma, follow Figma and flag it to the owner.

## 1. Before you start
1. Read the handoff and the script file. Read **"Cerita singkat"** first so the slides keep one flow.
2. Check the BSG (Brand Guidelines page), then the Moodboard for direction.
3. Duplicate the closest template from the Social Media Team page. Never edit the original.
   - Carousel: 1080x1440. Feed post: 1080x1350. Story and reels: 1080x1920.
   - MAF-01 used 4:5 (1080x1350) while the carousel template is 1080x1440. **Confirm the size with the owner** before building more (open item).
4. If any text is missing or marked `[...]`, keep the placeholder visible and flag it. Never fill it in.

## 2. Build rules
- Build only from BSG components (`BSG/Logo`, `Card`, `Tag`, `Button`, `Callout`, `Spec Row`), BSG text styles and semantic variables. No raw hex, no custom text style, no detached component when a BSG one exists.
- Geom only, the nine text styles, sentence-case headlines (caps only for Label, plus verdict stamps if Comet and Fore confirm).
- Corners from radius tokens (`md` cards, `sm` chips, `full` pills, `lg` large containers). Spacing from the scale (4, 8, 12, 16, 24, 32, 48, 64, 96, 128).
- Every text and background pair at least AA (4.5:1 body, 3:1 large). Allowed pairs: white on Cobalt or Navy, Navy on Chartreuse or Blush, Chartreuse on Navy, Cobalt on white.
- Never: white on Chartreuse or Blush, Chartreuse text on white, Blush as a background.
- One graphic device and one idea per slide. If in doubt, remove it.
- Logo: never recolor, stretch, rotate, outline or add effects. Minimum 120 px wide on screen (240 px preferred). Clearspace is the height of the "o" in BORE. White or Electric on dark and Cobalt, Navy on light.
- Real photos of parts, machines and hands only. No generic stock. Do not use Moodboard images.
- Keep the creator and IP disclaimer from the templates on any slide that shows a customer's or third-party design.

## 3. Copy rules
- Keep Sudo's slide order and wording. Make the headline the most prominent text on every slide.
- Do not split sentences into fragments or reorder lines for layout. Keep connector words (Ternyata, Tapi, Nah, Jadi) visible.
- If text does not fit, ask Sudo for a shorter version. Never cut it yourself.
- Density: owner prefers dense layouts over spacious ones (decision 5 Nov, MAF-01). A phone-size check is part of the work.

## 4. Naming and structure
- Frames: `<ID> / Slide <N> <name>` (for example `MAF-01 / Slide 4 Dashboard`). Delete superseded frames when the new version is built.
- Each slide: top bar (logo plus series label), content, bottom bar (small line plus counter "0X/0N").
- Work lives in the Social Media Team page, section "Post To Go" [ASSUMPTION: confirm with the owner].

## 5. Hand-off
1. Save links, field and mode per slide, deviations from the script and open items in `work/<ID>_design-notes_v<N>.md`. Designs live in Figma, the notes file holds links, sizes and export notes only.
2. Open a handoff to the other designer for review (`OPEN_<ID>_<FROM>-to-<TO>_<date>.md`), then after review to FORE.
3. Update your STATUS.md line and add one log line.
4. Export (PNG 1x) only after the reviewer and Fore approve.

## 6. Self-check before review
- [ ] Headline is the biggest text on every slide, and the headline-only read still tells the story.
- [ ] Each slide gives a reason to swipe.
- [ ] Contrast pairs pass. No raw hex. Radius and spacing tokens only.
- [ ] No placeholders hidden or filled in.
- [ ] Logo untouched, one device per slide.
- [ ] Chart axes start at 0 and labels are not new claims (confirm label wording with Sudo).
