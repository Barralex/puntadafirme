# Puntada Firme

One-page landing for **Puntada Firme**, a Venezuelan-rooted sewing business in Solymar, Ciudad de la Costa. The page has a single job: get the visitor to tap the WhatsApp button.

Published at `https://puntadafirme.com/` through GitHub Pages.

## Stack

One static page. No build step, no dependencies, nothing to install: `index.html` carries the HTML, the CSS and the JS. Leaflet 1.9.4 from a CDN for the coverage map.

## Before pushing

```bash
python .github/scripts/check.py
```

It also runs on every push to `main` and stops the deploy on failure. It checks the 60 KB budget for `index.html`, balanced markup, that every referenced file exists, that no image was pasted in as base64, and that the social tags are absolute and on the right domain. **The budget is nearly spent** (~59 KB): delete dead CSS before adding anything.

## Page rules

- **Copy is Spanish, written in tuteo** ("me escribes", "consúltame", "cerca de ti"), because the business is Venezuelan-rooted. No Rioplatense voseo; if that ever changes, the whole page changes at once.
- **Avoid "doblada"** when describing a garment — the word carries an unintended reading in Uruguayan Spanish. Use "ruedo", "dobladillo" or "prenda plegada".
- **File names are English, kebab-case**, even though the content is Spanish.
- **No code comments.** Not in CSS, not in HTML, not in JS. Anything that needs explaining goes in chat or in this file.
- **No emojis in the UI.** Icons are inline SVG `<symbol>`s in the sprite at the top of `<body>`, used via `<use href="#id">`. The Venezuelan and Uruguayan flags are the only exception — they are identity.
- Uruguayan vocabulary carries the local SEO: *ruedo*, *túnica*, *modista*, *costurera*, *arreglos de ropa*.

## Palette

Tokens in `:root`, sampled from the logo. Ratios are measured against cream, the surface each one actually sits on.

| Token | Value | Role | On cream |
|---|---|---|---|
| `--green` | `#123A2B` | Brand, header, buttons | 11.2:1 |
| `--cream` / `--linen` | `#F7F1E6` / `#F2ECDD` | Section surfaces | — |
| `--leather` | `#AC733F` | Accents, display type | 3.4:1 — large only |
| `--leather-deep` | `#8A5A2B` | Small type, labels | 5.2:1 |
| `--gold` | `#D4A95C` | Accent on dark surfaces | 1.9:1 — never here |

Type: Cormorant Garamond sets the headings, EB Garamond the gallery and steps, Inter the body copy, Source Serif 4 Bold only the wordmark.

A new color becomes a token or it doesn't ship. No mints, no cold greens.

## Brand

The seal in `assets/brand/` is original vector work: a leather rope, a laurel wreath top and bottom, and the **PF centered in the circle — centered by its ink, not by the text baseline**. If the PF's size or tracking changes, measure the ink bounds again and re-center. The pieces are `seal-cream.png` (header and footer, on green), `stamp-seal.png` (the inked stamp on the delivery card), `seal-badge.png` (link preview), the favicons and `apple-touch-icon.png` — those last ones use a simplified mark with no wreath, because at 16px the wreath turns to mush.

## Data kept in more than one place

The opening hours (Mon–Fri 15–19, Sat 9–15) sit in two spots that must always agree: the footer and `openingHoursSpecification` in the JSON-LD. The phone number sits in five: the four WhatsApp buttons, `telephone` in the schema, and the footer text. Change one, change them all — a mismatch between the page and the Google Business Profile cancels out the local SEO signal it was meant to send.

## Legal

`machine-heavy-duty.jpg` is CC BY by storebukkebruse. **The footer credit stays** — `alt` text does not count as attribution.

## Commits

`type(scope): short message`, in English, no signatures or trailers. For example `feat(landing): add rate card`, `fix(deploy): ...`, `docs(readme): ...`.
