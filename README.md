# Phideo — brand style guide

Consolidated brand system for **Phideo** (phideo.io) — the AR app that attaches a video to a
printed photo. Point a phone at the print and the video plays over it. *phideo = photo + video.*

Developed by **Lunchbox Agency**, 15 September 2026, from every brand source in circulation:

- **Brand Manual V2** (2023)
- the **asset hub** (assets.lunchbox.agency/brand/phideo — logos, fonts, social, photography, app, video)
- Figma **"Phideo Website"** and **"Phideo | Mailer Designs"**
- the **live site** (phideo.io — WordPress + Oxygen 6)

## Files

| file | what it is |
|---|---|
| [`index.html`](index.html) | The visual style guide — open it in a browser. Self-contained (Amenti embedded, Poppins from Google Fonts). Same content as the hosted version. |
| [`design-system.md`](design-system.md) | The system in text: brand core, colour, typography, logo, imagery language, graphic devices, components (web / email / app / print), motion, voice. |
| [`discrepancies.md`](discrepancies.md) | **Read first if you're deciding anything.** Every place the sources disagree — colour values, CMYK, typefaces, type scale, the ®, contact details, gradients — with evidence and a recommendation. Settled so far: #1–3 (Brand Manual V2 is the source of truth for the primaries). |
| [`logo/phideo-logo-color-spec.svg`](logo/phideo-logo-color-spec.svg) | The 2-tone logo re-coloured to the spec values `#702283` / `#E52329`. |
| `logo/phideo-logo-{purple,red,black,white}-spec.svg` | The four single-colour variants, generated from the spec file — ready to replace the hub set. |
| `logo/phideo-logo-*-spec.png` | 1024×1024 transparent PNG exports of all five variants (rendered with Chrome, so the ® mask is correct). |
| [`logo/phideo-logo-color-hub-original.svg`](logo/phideo-logo-color-hub-original.svg) | The same file as it sits on the asset hub today (`#722C8F` / `#EC1B25`) — kept for comparison, see discrepancy #1. |
| `photography/phideo-photo-0{1..6}-*.png` | The reference photoshoot (Higgsfield Soul 2.0 / Soul Cinema, 2K): six directed shots covering the everyday and campaign registers — see the Photography section of the guide for the shot notes and the photo-treatment rules. |
| `photography/plate-{m,s,w}.png` | Layout plates shot **to the wireframe** (subject top ~55%, type-safe negative space bottom ~45%) and passed through CD QA — used by the photo-hero demo and the two photo-hero email templates. |
| [`production-workflow.md`](production-workflow.md) | The photo-led production pipeline: goal → wireframe → shoot → CD QA, with role briefs, the W1 wireframe, the worked plate briefs and the QA log. Nothing photo-led ships without it. |

## The short version

- **Colour:** purple `#702283` for structure and ink, red `#E52329` for anything you tap. No
  secondary palette in print; a digital-only violet family (`#B200ED` …) for web and app if
  adopted (discrepancy #4).
- **Type:** Amenti (Black / Bold / Medium / Regular) for display and headings; Poppins for body
  and UI (recommendation — discrepancy #5).
- **Logo:** the `o` is the app icon. Clearspace = the height of the `o`. White on gradients.
  Never red-on-purple or purple-on-red.
- **Imagery:** the print is still (often black-and-white); the same scene is alive in colour
  inside the phone. Both visible at once. Hands, real prints, delight.
- **Voice:** warm, plain, a little astonished. "Bring Photos to Life. Instantly." ·
  "Scan. Watch. Experience."

Items marked `(#n)` in the design system are open decisions; the numbers point into
`discrepancies.md`.
