# OJW Carousels — Project Instructions

This project produces LinkedIn + Instagram carousels for **One Just World** (OJW), an Indian NGO advocating plant-based futures, animal welfare, and food-system change.

> **Always start by re-reading this file and `brand/foundations.html`** before producing visuals. They are the source of truth.

---

## The brand in one paragraph

OJW speaks **truth, not alarm bells**. Confident, compassionate, Gen Z-energy, Indian in context. *Reconstruction* is the main identity (joyful future-facing); *deconstruction* (hard truths about dairy industry contradictions) is occasional and audience-appropriate. Reframes Darwinism: **Survival of the Kindest. Conscious Selection. Evolution by Compassion. Struggle for Dignity of Life.**

Tagline: **"One just world. Because change is coming for all of us."**

---

## Brand assets (saved in this project)

- `brand/logo-black-wordmark.png` / `logo-white-wordmark.png` — full lockup, black/white
- `brand/logo-light-wordmark.png` / `logo-deepgreen-wordmark.png` — green-on-green hero treatments (light green logo for deep green bg; deep green logo for light green bg)
- `brand/logo-mark-black.png` / `logo-mark-white.png` / `logo-mark-light.png` / `logo-mark-deepgreen.png` — monogram only
- `brand/fonts/` — Cooper BT family (Light, Medium, Bold, Black + italics)
- `brand/references/` — existing campaign visuals (Dairytale cow, Change Is Coming catfish/ants, manifesto spread, herd landscape, logo green combos)
- `brand/tokens.css` — colors, type scale, @font-face for Cooper BT — **import in every carousel**
- `brand/foundations.html` — visual reference for the entire system

## Source PDFs (in `uploads/`)
- `Brand Voice.pdf` — buckets, frames, voice/tone, CTAs
- `OJW - Typography .pdf` — Inter type scale
- `OJW Style Sheet (ongoing).pdf` — colors, fonts
- `OJW 2026.pdf` — strategy, manifesto, "Origin of Change"

---

## Color palette

| Token | Hex | Use |
|---|---|---|
| `--ojw-green-deep` | `#012c12` | Dominant. Backgrounds. |
| `--ojw-green-mid` | `#659d67` | Secondary surfaces. |
| `--ojw-green-light` | `#97cc98` | Soft fills, tints. |
| `--ojw-cream` | `#d2dfd7` | Paper, calm bg. |
| `--ojw-mist` | `#bfc9c2` | Borders, dividers. |
| `--ojw-black` / `--ojw-white` / `--ojw-ink` `#1a1a1a` | — | Type, surfaces. |
| `--ojw-signal` | `#e62154` | **Sparingly.** Alerts, CTAs. |
| `--ojw-highlight` | `#fff500` | **Sparingly.** Underlines, marker emphasis. |

> **Greens dominate. Signal/highlight are accents, never foundations.**

## Type
- **Inter** (primary) — full weight range. Use for everything.
- **Cooper BT** — licensed, loaded from `brand/fonts/`. Weights: Light (300), Medium (500), Bold (700), Black (900) + italics. Display only, never long copy. Use Black for hero claims, Light for editorial.

## Recurring motifs
- **Wave divider** — echoes the curved baseline of the OJW mark. Available as `.ojw-wave` in `tokens.css`.
- **Yellow marker highlight** on key words — `.ojw-mark` class.
- **Signal pill** for CTAs — `.ojw-pill`.

---

## Voice & tone

- Clear, not academic
- Confident, not defensive
- Impact-oriented, not emotional overload
- Indian in context (cultural cues, ahimsa, modern India)
- Avoids shaming individual farmers — names the *system*
- Joyful, future-facing — even when calling out hard truths

## Visual checklist
- Human faces > graphics
- Warm earthy palette (greens + cream)
- Indian cues (texture, type, culture)
- Clean layout, no clutter

---

## Six content buckets — every carousel declares its bucket

1. **Changemaker Stories** — peer credibility, distributed leadership
2. **Proof of Impact** — what worked, why, what changed
3. **Knowledge Tools** — equip changemakers (FAQs, stats, research)
4. **Culture & Aspiration** — normalize plant-based future, joyful
5. **Institutional Shift** — cafeterias, HR, college clubs, default-to-plant
6. **Seasonal Myth Busting** — festivals, news, viral myths corrected with warmth

## Six frames — every post must hit at least one

Wellness · Sustainability · Economically Smart · Compassion · Youth Leadership · Future-Focused India

> If none apply → rethink the post.

---

## CTA tiers

- **Soft** (most posts): "Share with your group." "Save for your next meeting." "Tag someone."
- **Hard** (max 1×/week, Sunday): Sign up · Join · Attend action · Download
- **Institutional** (2×/month): "If you work in HR/campus admin, DM us."

---

## Carousel canvas sizes (use one per export)

- **LinkedIn portrait / Instagram portrait** — `1080 × 1350`
- **LinkedIn square** — `1200 × 1200`
- **Story / Reel cover** — `1080 × 1920`

## Output workflow

User exports as **PNG per slide** to upload directly to Canva (where photos may be added on top by the team). So:
- Build each slide as a self-contained `<section class="ojw-slide ig-portrait">` etc., a direct child of a `<deck-stage>` (or in a design canvas)
- For posts that need photos, leave a clearly labeled photo placeholder zone (the team adds the photo in Canva)
- For text-only / illustrative posts, ship as final PNGs

To export PNG per slide: open the carousel HTML, capture each slide, save as PNG. Use the Save-as-PDF or screenshot path; PPTX export is the fallback.

---

## How to brief a new carousel (template the user fills)

1. **Topic / hook** —
2. **Bucket** (1–6) —
3. **Frame(s)** (≥1) —
4. **Audience** — Gen Z changemakers / Institutional / Mix
5. **Slide count** — typically 5–8
6. **CTA tier** — soft / hard / institutional / none
7. **Photos** — supplied? or text-only? or leave placeholders for Canva
8. **Canvas** — IG/LI portrait 1080×1350 (default), LI square 1200×1200, or story 1080×1920

---

## Working approach

1. Re-read this file + `brand/foundations.html`.
2. If the user hasn't briefed using the template above, ask 1–2 quick questions (bucket, frame, audience, photos).
3. Build the carousel as a `deck-stage` HTML file in a folder named after the topic (e.g. `carousels/calcium-myth/`).
4. Each slide is `<section class="ojw-slide ig-portrait">` (or appropriate size class).
5. Vary slide layouts — type-led, quote, stat, photo placeholder, CTA — never all five in the same composition.
6. End the deck with the OJW logo + handle slide.
7. Show the file via `done`.
8. Export to PNGs when the user approves.

## What to ask the user for, going forward

- **Photos** for each carousel (the user supplies; team gives them)
- **Cooper BT font file** (when licensed) — replace Lilita One in `tokens.css`
- **Examples of OJW carousels they like** — keep references in `references/` to refine the system
- Any **campaign-specific assets** (e.g. "Milk is Not Vegetarian" campaign visuals)
