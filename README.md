# Olympics Unleashed — Daisy Thomas

A 9-slide schools presentation ("Unleash Your Potential") built as a self-contained
HTML deck. No build step, no internet connection, no dependencies — it runs by
opening one file.

## Run / present it

Double-click **`Daisy Thomas - Olympics Unleashed.html`** to open it in any modern
browser (Chrome, Edge, Safari).

**Controls**
- `←` / `→`, `PgUp` / `PgDn`, `Space` — previous / next slide
- `Home` / `End` — first / last slide
- number keys — jump to a slide
- `R` — reset to slide 1
- On a touch screen, tap the left/right half of the slide to go back/forward
- A thumbnail rail appears on the left (click to jump; drag the edge to resize).
  It is hidden automatically when presenting full-screen.

## The slides

1. **Cover** — "Unleash Your Potential" over a full-bleed halfpipe shot
2. **Meet Daisy (video)** — full-bleed 1920×1080 video (`assets/daisy-video-1.mp4`)
3. **Who Am I?** — Daisy's profile (Gangwon 2024, Milano Cortina 2026)
4. **Daisy in Action (video)** — full-bleed 1920×1080 ski clip (`assets/daisy-video-2.mp4`)
5. **The Early Years** — childhood photos
6. **Overcoming Challenges** — resilience
7. **The Olympic Dream…** — full-bleed section divider
8. **Taking Opportunities**
9. **Goal Setting** — Greg Reid quote + animated goal card (see below)
10. **Brisbane 2032** — with the two olympics.com.au link cards
11. **Closing** — "Wherever You Land, Unleash Your Potential!"

## The video slides (2 and 4)

Both videos fill their slide (each is exactly 1920×1080) and have standard playback
controls. A video **starts playing automatically** when you navigate to its slide, and
**pauses and rewinds** when you move away. If a browser blocks autostart (some block
audio until you've clicked once), just tap the play button — it works normally once
you've started navigating. Sources: `assets/daisy-video-1.mp4` and
`assets/daisy-video-2.mp4`. Both are H.264/AAC `.mp4` (universal browser support); the
cover video is web-compressed to ~86 MB so the whole deck stays under hosting limits.

## Slide 9 — the animated goal card

When slide 9 opens it auto-plays: a gold highlight steps through each field and the
answers type themselves in (Goal → the three "how" steps → support team).
**Click the card to replay it** during the talk.

## Print to PDF

Use the browser's **Print → Save as PDF**. The deck lays out one slide per page at
full 1920×1080, with no extra margins or browser chrome.

## Export to editable PowerPoint

The motion (Fade & Rise entrance, slide-9 typing) and the **videos** (slides 2 and 4)
play only in the HTML version —
it can't be baked into a `.pptx`. The deck already uses Office-safe fonts
(Franklin Gothic Heavy headings / Calibri body), so a PowerPoint export resolves
fonts natively on Windows and Mac. To reproduce the entrance in PowerPoint, select
the elements on each slide and apply **Animations ▸ Float In + Fade** (set bullets
to "By Paragraph" so they cascade).

## Files

- `Daisy Thomas - Olympics Unleashed.html` — the slides (static markup) + the video and goal-card scripts
- `deck.css` — the design system (palette, fonts, layouts, goal-card animation)
- `deck-stage.js` — the reusable deck runtime (nav, scaling, thumbnail rail, print)
- `serve.cjs` — a tiny local static server (Node) with video range-request support, for previewing
- `assets/` — the 16 images plus `daisy-video-1.mp4` and `daisy-video-2.mp4` the deck uses

### Palette
Sky blue `#3EA0D9` · deep blue `#15486B` · ink blue `#0E3148` · gold `#F5B301` ·
text ink `#1C2B36`
