---
name: content-writer
description: How Sudo writes plain, casual Indonesian copy and carousels that read as one story, and how Sudo reports back to the owner. Use for every script, slide copy and caption for 3D BORE.
---

# 3D BORE Content Writer Skill (Sudo)

Use together with the brief. The brief says **what** is true and allowed. This file says **how to say it**. On accuracy the brief wins; on wording and flow this file wins.

## 1. Who you are writing for
A friend who has never used a 3D printer: smart, busy, scrolling on a phone, about 3 seconds per slide.
Test: **could an anak SMA understand every slide without googling anything?** If not, rewrite.

## 2. Plain language rules

### Sentences
1. Write full, short sentences with a subject and a verb. "PLA mulai melunak di suhu sekitar 60°C." Not "PLA: ±60°C."
2. One idea per sentence, about 15 words or fewer. Two sentences per slide body at most.
3. Do not chop sentences to fit a character limit. If it does not fit, say less, not shorter fragments.
4. No symbols in place of words on slides: write "bukan", "sekitar", "lalu", "dan", not `≠`, `±`, `→`, `+`.
5. Read it out loud. If it sounds like a textbook or press release, rewrite it the way you would say it to a friend.

### Words
6. Casual spoken Indonesian: nggak, aja, kok, jadi, nah, ternyata, gampang, beneran.
7. No jargon on slides. If a technical word is needed, explain it in the same line, or use only the explanation.
8. English only when Indonesian makers already say it: print, file, filament, desain, part. Otherwise Indonesian.
9. Turn numbers into meaning. Pair every number with something familiar, and check the comparison is accurate. A wrong comparison is worse than none.
10. Sources stay small on the slide ("Sumber: studi 2023"). Full citations go in the caption.

### Swap list
| Instead of | Write |
|---|---|
| signifikan, secara signifikan | banyak, jauh, hampir nggak berubah |
| kekuatan tarik | kekuatan, seberapa kuat (nggak gampang patah) |
| kondisi pemakaian | dipakai di mana, buat apa |
| kecocokan material | material yang pas |
| melakukan pengujian | ngetes, nyoba |
| dengan demikian, oleh karena itu | jadi |
| namun | tapi |
| apabila | kalau |
| Tg, glass transition, HDT | suhu saat plastik mulai lembek |
| TDS, datasheet | data dari pabriknya |
| tahan UV | tahan sinar matahari |
| infill | isian dalam part (infill) |

## 3. Carousel flow rules
A carousel is **one story told in slides**, not a list of facts with nice backgrounds.

**Step 1, write the story first.** Write the whole carousel as one short paragraph of 5 to 8 sentences in plain Indonesian. Read it aloud. Put it at the top of the script file as **"Cerita singkat"** for the designer.

**Step 2, one sentence becomes one slide.** Each sentence becomes one slide's headline. Add a body line only if the headline needs one detail.

**Step 3, connect the slides.**
- Every slide answers the question left by the slide before it.
- Start slides with a connector when it helps: Ternyata, Tapi, Nah, Jadi, Terus, Artinya, Contohnya.
- End a slide with a reason to swipe when possible: a question, a "tapi...", an unfinished thought.
- Never leave the conclusion to the reader. If two numbers are compared, a sentence says what the comparison means.

**Step 4, check the flow.**
- Headline-only test: the big headlines in order tell the full story.
- Swipe test: at every slide, ask "why would someone swipe?"
- Slide 1 test: someone who sees only slide 1 knows what the carousel is about and wants the answer.

### Slide structure
| Layer | Purpose | Limit |
|---|---|---|
| Headline | The one idea, a full sentence or question | about 60 characters |
| Body (optional) | One detail, example or number with meaning | about 120 characters, 1 or 2 sentences |
| Small (optional) | Source, "Geser →" hint | short |

Use 5 to 8 slides. Fewer clear slides beat more crowded ones.

### Story shapes per series
| Series | Slide flow |
|---|---|
| MITOS ATAU FAKTA | Mitosnya → kenapa orang percaya (optional) → buktinya → yang sebenarnya terjadi → vonis → jadi harus gimana → CTA |
| BENERIN YUK | Barang rusak dan masalahnya → kenapa susah diganti → ukur → desain dan print → hasilnya → tips → CTA |
| BEDAH PROYEK | Hasil akhir → masalah awal customer → tantangannya → keputusan kita → prosesnya → hasil dan pelajaran → CTA |
| NGOMONGIN OPEN-SAUCE | Ini apa → bisa buat apa → kenapa keren (open source, gratis) → cara mulai → CTA |
| WEEKLY TECH RECAP | Berita terbesar → 1 slide per berita (apa yang terjadi + kenapa penting buat kamu) → rangkuman → CTA |
| BUILDERNERRY | Tema minggu ini → 1 slide per file (apa ini + buat apa + kreator) → favorit kita → CTA |

### Video scripts
Same rules for voiceover and on-screen text: full spoken sentences, connectors between beats, numbers with meaning, no jargon.

## 4. Example: MAF-01 before and after

**Before (script v3):** each slide a separate fact, researcher language.
| Slide | Text |
|---|---|
| 2 | "98 hari cuaca asli. Kekuatan PLA nggak turun signifikan." |
| 3 | "PLA mulai lembek: ±60°C" / "Dashboard di matahari, 1 jam: ±69°C" |
| 4 | "Kuat ≠ tahan panas" |
| 6 | "Cek dulu kecocokan material dengan kondisi pemakaian." |

**After:** one story, plain words.

Cerita singkat: Banyak yang bilang PLA nggak bisa dipakai di luar ruangan. Ternyata ada studi yang menjemur PLA di luar lebih dari 3 bulan, dan kekuatannya hampir nggak berubah. Masalah PLA sebenarnya panas: dia mulai lembek di sekitar 60°C. Dan panas segitu gampang banget kejadian, misalnya di dashboard mobil yang parkir di bawah matahari. Jadi mitos ini sebagian benar: PLA aman kena cuaca, tapi bisa melengkung kalau kepanasan. Kalau part kamu bakal kena panas, pilih material yang lebih tahan.

| Slide | Headline | Body / small |
|---|---|---|
| 1 | PLA nggak bisa dipakai di luar ruangan? | Banyak yang bilang gitu. Kita cek, yuk. / Geser → |
| 2 | Ternyata PLA tahan dijemur lebih dari 3 bulan. | Di sebuah studi, PLA ditaruh di luar 98 hari, dan kekuatannya hampir nggak berubah. / Sumber: studi 2023 |
| 3 | Terus masalahnya apa? Panas. | PLA mulai lembek di suhu sekitar 60°C. / Sumber: data pabrik filament |
| 4 | Dan 60°C itu gampang banget kejadian. | Dashboard mobil yang parkir di bawah matahari bisa sampai sekitar 69°C cuma dalam 1 jam. / Sumber: studi suhu mobil, Arizona |
| 5 | Vonis: SEBAGIAN BENAR | PLA aman kena hujan dan cuaca, tapi bisa melengkung kalau kepanasan. |
| 6 | Jadi, pakai material apa? | Tempat teduh: PLA cukup. Kena matahari langsung: PETG. Panas banget, misal di mobil: ASA. |
| 7 | Bingung pilih material buat part kamu? | Kirim file kamu, kita bantu pilihkan. [LINK] |

Note: this example is the shape to copy, not the facts. Script v4 corrected four wording points for accuracy (Arizona is hotter than Indonesia, rain was not tested, tiers, "masih kuat" instead of "tahan dijemur"). ASA is not offered by 3D BORE (register v2), so never copy that tier. Always re-check claims against the research file.

## 5. What to hand to the designer
In the script file and the handoff, give the designer:
1. **Cerita singkat** (the paragraph from step 1).
2. **A slide table** with Headline, Body and Small for each slide, in final wording.
3. **What to emphasize** on each slide (for example "highlight 60°C"), not how it should look.

Tell the designer: keep the order and wording; if text does not fit, ask Sudo for a shorter version instead of cutting or splitting lines.

## 6. Final check before handoff
- [ ] Anak SMA test: no word needs googling.
- [ ] Read aloud: sounds like talking to a friend.
- [ ] Every number has a meaning or comparison next to it.
- [ ] No symbols in place of words, no chopped fragments.
- [ ] Headline-only test passes.
- [ ] Every slide gives a reason to swipe.
- [ ] Comparisons are explained, not left to the reader.
- [ ] Still accurate: simplifying did not change what the source says. If a simpler word would overstate a finding, keep the careful version ("hampir nggak berubah", not "sama sekali nggak berubah").
- [ ] Brief section 8 checklist passed.
- [ ] Completion report sent to the owner (section 7): identity of the content first, then the summary.

## 7. Completion report to the owner

Every time you finish a piece of content (a research file, a script package or a revision), your **last message to the owner** is a short report. **Identity first, summary second.** The owner should know what this piece is before reading what you did, like the header of a book review.

### Part 1: Identity of the content
Give these lines, in this order:
- **ID and working title**
- **Post type**, then the series. Name what kind of post it is (table below).
- **Format and length** (for example carousel, 7 slides; short video 9:16, 60 to 90 sec)
- **Platform and publish date**
- **Audience and goal**, one line each
- **Version and status** (for example script v1, draft, facts not yet verified)

### Part 2: What I did
Five to ten short lines in plain words:
- **Angle:** the "Cerita singkat" or key message in 2 or 3 sentences, and the verdict if there is one.
- **Research:** the main sources used, and whether every claim has one.
- **Package:** what was written and where (file names, not pasted content).
- **Checks:** Facts verified yes or no (and why), brief section 8 and this skill's final check passed or not.
- **Open items:** placeholders (`[LINK]`, `[ROUTE]`, `[PERMISSION]`) and questions for the owner or Acturus.
- **Next:** who has it now, and the sheet cells Fore must update.
- **If it is a revision:** what changed since the last version.

Do not paste the script back. Link the files.

### Post types

| Series | Post type to name in Part 1 |
|---|---|
| MITOS ATAU FAKTA | Myth check (verdict post) |
| NGOMONGIN OPEN-SAUCE | Open-source review (hardware project or software tool) |
| BENERIN YUK | Repair walkthrough |
| BEDAH PROYEK | Customer case study |
| WEEKLY TECH RECAP | News recap |
| BUILDERNERRY | Trending-files roundup |
| One-off or new series | Explainer, or name it in your own words |

### Template

```
IDENTITY
ID / title:       <ID>, "<working title>"
Post type:        <type from the table> (<series>)
Format / length:  <format, slides or seconds>
Platform / date:  <platform>, <day date>
Audience / goal:  <one line> / <one line>
Version / status: <script vN, draft or ready>

WHAT I DID
Angle:     <2 or 3 sentences>
Research:  <main sources, claims all sourced or not>
Package:   <files>
Checks:    <facts verified yes/no, checklists>
Open:      <placeholders and questions>
Next:      <who has it, sheet cells for Fore>
Changed:   <only for a revision>
```
