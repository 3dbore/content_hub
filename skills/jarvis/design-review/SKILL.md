---
name: design-review
description: Checklist for Jarvis and Comet reviewing each other's Figma frames against the BSG and DESIGN.md. Use when a design handoff arrives for review.
---

# Design review (Jarvis and Comet)

The other designer reviews. If one designer is unavailable, the other covers both and Fore reviews against the BSG. Comments must be **specific and fixable**: name the frame, the layer and the change.

Good: "Slide 3, layer 'Body': white text on Chartreuse. Switch to `text/primary`."
Not useful: "Contrast feels off."

## 1. What to open
- Design handoff and the notes file (`work/<ID>_design-notes_v<N>.md`).
- The script (`work/<ID>_script_v<N>.md`), for wording, order and Cerita singkat.
- `DESIGN.md` section 12, plus BSG in Figma if anything disagrees.

## 2. Check, frame by frame
1. **Tokens:** semantic color variables only, no raw hex. Text styles from the nine BSG styles. Radius and spacing tokens only.
2. **Components:** BSG components used and not detached.
3. **Contrast:** every pair at least AA. Look for the banned pairs (white on Chartreuse or Blush, Chartreuse on white, Blush background).
4. **Logo:** colorway matches the field, not below 120 px, clearspace kept, no effects.
5. **One device, one idea** per slide. Remove anything that does not serve precision, speed or openness.
6. **Type:** Geom only, sentence-case headlines, body left-aligned, no centered long paragraphs. Caps only in Label, and flag stamps for owner decision.
7. **Copy fidelity:** wording and order match Sudo's script. No fragments, no dropped connectors, no symbols replacing words.
8. **Hierarchy:** headline is the most prominent text. Run the headline-only read.
9. **Flow:** does each slide earn the swipe? Does slide 1 stand on its own?
10. **Phone size:** readable at actual phone size. Charts and small text checked.
11. **Honesty:** charts start at 0, labels are not new claims, placeholders still visible, no third-party images without credit.
12. **Safe areas and size:** correct frame size for the format.

## 3. Outcome
- All pass: set the handoff to `DONE`, open `OPEN_<ID>_<FROM>-to-FORE_<date>.md`.
- Fixes needed: leave comments in Figma, list them in the handoff, send it back to the designer as `OPEN`, and note whether a second review is needed.
- A rule is unclear or disagrees with Figma: flag to the owner via FORE, do not decide alone.

## 4. Also
- Propose new components or tokens only when a need repeats. The owner approves design system changes.
- Update your STATUS.md line and add one log line.
