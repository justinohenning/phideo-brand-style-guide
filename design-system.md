# Phideo — design system

> Consolidated 2026-09-15 from the Brand Manual V2, the asset hub, both Figma files and the
> live site. Where those sources disagree the value here is the **recommended** one and the
> conflict is numbered `(#n)` → [discrepancies.md](discrepancies.md). Nothing marked `(#n)` is
> final until Franco decides.

## 1. Brand core

- **What it is:** an AR app that attaches a video to a printed photo/image; scan the print
  with a phone and the video plays over it. *phideo = photo + video.*
- **The idea every visual must carry:** the phone is the **gate** between the real world and
  the digital one. Print/photo = real, still, often black-and-white or faded. Phone screen =
  alive, colour, moving. Composition shows both at once — the print in the world, the same
  scene alive inside the phone frame. "Bring them to life."
- **Mission** (manual): to increase the value of individuals and brands by linking video to a
  physical image using technology that is quick and easy to use. **Vision:** to create a
  faster, easier and more effective way of sharing information — for both brands and
  individuals. **Purpose:** to delight, entertain and educate people through creating
  immersive and interactive experiences. `(#15 — About comp rewords these)`
- **Guiding emotions:** joy, delight, surprise ("amazed" is literally the photoshoot brief).
- **Audience split:** consumers (memories, family, photo books, grandparents) and brands
  (posters, real estate, retail signage, galleries, business cards, billboards).

## 2. Colour

Two primaries, no formal secondary (manual: "we do not have a secondary palette… where
possible the primary colours should be"). Red is the **action** colour — buttons, links,
anything tappable. Purple carries structure and mood.

### Primaries — canonical values ✅ *settled 2026-09-17: Brand Manual V2 is the source of truth*
| token | hex | RGB | CMYK (print, from manual) | where it is already used |
|---|---|---|---|---|
| `purple` (Figma "Deep Plumb") | **#702283** | 112 34 131 | C70 M100 Y0 K0 | manual spec, asset hub, Figma mailer var, live site `--bde-palette-title` |
| `red` | **#E52329** | 229 35 41 | C0 M95 Y85 K0 | manual spec, asset hub, Figma mailer var, web hero gradient |

Known drift of the same two colours (don't introduce more — all superseded by the manual's
spec values above): manual's own rendered swatches #6F2B90 / #EE2F35; logo SVGs on the hub
#722C8F / #EC1B25; asset-hub CMYK is auto-derived (15,74,0,49 / 0,85,82,10) and must not go
to print. Open follow-ups: re-export the logo files and correct the hub CMYK cards.

Contrast on white: purple 9.35:1 (AAA), red 4.56:1 (AA for text ≥ 18px / bold). **Purple on
red (or red on purple) is 2.05:1 — never set text or the logo one on the other**; the manual's
"Not accepted" page shows exactly that. Logo on any gradient = solid white.

### Tints (mix with white; use sparingly, prefer full saturation)
| | 80% | 60% | 40% | 20% | 10% |
|---|---|---|---|---|---|
| purple | #8D4E9C | #A97AB5 | #C6A7CD | #E2D3E6 | #F1E9F3 |
| red | #EA4F54 | #EF7B7F | #F5A7A9 | #FAD3D4 | #FCE9EA |

(The manual page renders its tints from the drifted purple: #8351A0 / #9A75B3 / #B59BC9 /
#D5C8E3 and red #F16352 / #F58973 / #F8AE9A / #FCD4C7 — superseded by the table above.)

### Gradients
- **Brand gradient** (print, social, profile pictures, stationery): linear **purple → red,
  diagonal top-left → bottom-right**; colours may be inverted; 50/50 stops. Logo on it is
  white. Two flavours exist in stationery: purple-heavy and red-heavy.
- **AR mesh** (web only — `(#11)`): soft radial blobs of purple, red, the web violet and pink
  over white/lavender; blurred, no hard edges. Hero variant is saturated (red + plum, the two
  primaries only); content-section variant is pale (mostly white, lavender #EEC7FB-ish and
  pink #F4A3A5-ish haze). Six reference boards live in Figma Sandbox → Gradients `290:2436`.

### Web "AR glow" family `(#4 — not in the manual; formalise or retire)`
The website Figma and the live site both use a brighter violet as the *digital* accent —
it reads as the "alive" side of the real/digital split, and it is what the AR overlay icons,
active filter pills and feature titles use:

| token (proposed) | hex | seen |
|---|---|---|
| `violet` | **#B200ED** | feature titles, typewriter headline, active pill, live-site CSS |
| `violet-hover` | #BF1DF5 | button/pill hover states in Figma |
| `violet-soft` | #B778FA · #CC9CFE · #E5AAF9 | glossy icons, pill fills, haze |
| `pink-highlight` | #BE38EA | live site `--bde-palette-pink-highlight` |
| `pink` | #DC2875 | live site `--bde-palette-pink` |
| `blush` | #F4A3A5 | mesh haze |

Rule if kept: digital surfaces only (web, app, motion). Never on print, never in the logo,
never as body text. White on violet is 5.1:1 (AA).

### Neutrals
White #FFFFFF; ink = purple #702283 for headings **and** body on light grounds (mailer and web
both do this — `(#19)`); grey text #404041 (manual folios); light glass tint = white at
20–35% over the mesh; input borders #DCDCDC / #E5E7E7 (live site).

## 3. Typography `(#5 #6 #7)`

### Brand typeface — Amenti
Geometric sans with single-storey `a`, the face of the wordmark and of every headline in the
manual, the hub, the social posts and the mailers. Files on the hub: **Thin, Regular, Medium,
Bold, Black** (the manual's list "Regular/Medium/SemiBold/Bold/ExtraBold" doesn't match the
files; use the file names). Licence: Envato Elements zip — confirm webfont/end-product rights
before self-hosting `(#5)`.

Manual hierarchy (p. 15, measured): H1 60 Black · H2 42 Black · H3 30 Bold · H4 20 Medium ·
Body 10 Medium · Small 8 Regular. Hub hierarchy: 72 / 35 / 22 / 18 / 12 / 8. Manual eyebrows =
Amenti Regular 12, uppercase, tracked ~0.5em (`T Y P E F A C E`), red.

### Body / UI typeface — one decision needed
- Manual body copy is set in **Aller** (Regular/Bold, 10pt) — never named in the manual.
- Mailer body is **Inter** (Figma var `font/family/Modern`).
- Website Figma **and** the live site are **Poppins** for everything (headings included); the
  site also loads Montserrat and Oxanium.
- Social posts add a serif (Lora-like "Revolutionize your memories") and a condensed sans.

**Recommended:** Amenti Black/Bold for display and headings on every surface; **Poppins** for
body, UI, forms and email body (already live, geometric enough to sit under Amenti, free);
retire Aller, Inter, Montserrat, Oxanium and the serif. If Amenti cannot be licensed for web,
Poppins SemiBold takes headings on web only and Amenti stays print/social.

### Proposed web scale (Amenti + Poppins, desktop → mobile)
| role | face | size / line | notes |
|---|---|---|---|
| Display | Amenti Black | 64/72 → 40/46 | hero only; -0.01em |
| H1 | Amenti Black | 48/56 → 34/40 | |
| H2 | Amenti Bold | 40/48 → 30/36 | "Endless Possibilities" is this, in purple |
| H3 | Amenti Bold | 28/36 → 24/30 | feature titles (violet on web) |
| H4 | Amenti Medium | 22/30 | card titles |
| Body | Poppins Regular | 18/28 → 16/26 | purple ink on light, white on dark |
| Small | Poppins Regular | 14/20 | captions, legal, footer |
| Eyebrow | Amenti Regular | 14, uppercase, +0.4em | red on light, white on dark |
| Tagline lockup | Amenti Medium | 20, +0.25em | "Scan.  Watch.  Experience." — extra word-spacing |
| Button | Poppins SemiBold | 16 | |

Live site today: Breakdance globals h1 32px, h2 25px, body 14px, base 16, ratio 1.25 — not a
designed scale, override.

## 4. Logo

- **Wordmark** "phideo" in Amenti-derived lettering: `phi` purple, `de` red, the `o` is the
  app icon — a purple ring, open top-right, with a red play triangle; a red arc closes the
  ring. Construction and clearspace on manual pp. 6–7 (clearspace ≈ the height of the `o` on
  all sides; icon alone gets the same).
- **Current files carry ®** (hub `Logo_Final-*`, Figma "updated logos" `875:554`, website,
  mailers). The manual's logos pre-date the ® `(#8)`.
- **Variants (hub + Figma):** 2-tone colour · purple · red · black · white. Icon: colour ·
  black · white.
- **Accepted:** 2-tone on white; white on red; white on purple; purple on white; black on
  white; black on red. **Not accepted:** stretching/skewing, rotating, drop shadows or
  bevels, colour swaps, purple logo on grey, red logo on purple, any logo on a busy photo
  without a scrim. On gradients: white only.
- **Placement:** print — upper-left or lower-left. Web/email — top-left inside a white lobe
  ("Logo holder": the lobe — see §6 for the cut-in construction — 600×92 in email,
  ~240×92 lobe in web nav).
- **Favicon / app icon:** the ring-and-play `o` alone; social profile pictures use the white
  wordmark on the brand gradient or on flat purple/red.

## 5. Imagery — the AR language

The manual sets four photography modes; the website adds a fifth. Every image should let a
viewer understand the product without reading.

1. **Composition / "looking"** — people looking at their phone with delight; highly
   saturated, colour-rich, story-telling. Phone in hand, screen visible.
2. **Black & white → colour** — the print is B&W or faded (old photo, album page, gallery
   frame, poster), the phone screen shows the *same* scene in full colour, moving. This is
   the single strongest device: it makes "brings photos to life" literal. Photoshoot 2023-09
   (grandmother + album) and the album/gallery composites on the hub are the reference.
3. **Demonstrate** — hands, phone, print, all in frame; landscape phone framed over the
   print; the printed QR/phideo tag visible in the corner of the print.
4. **Usage / context** — billboard, bus stop, business card, gallery wall, movie posters,
   real-estate listing, retail signage: show the range of *surfaces* that can carry a phideo.
5. **AR window (web)** — a hand holds a landscape phone; the phone frame is a *window* into
   a rounded, lavender-outlined "squircle" panel (≈40px radius, 1px white/40% stroke, soft
   glow) that contains the living scene, floating on the mesh gradient. Polaroid "cloud"
   variant: 5–6 rounded photo cards scattered around the phone, each with the same
   squircle treatment. Component: Figma `58:514` / `617:500`.

Do: real hands, real prints, warm skin, natural light; the screen brighter than the world
around it. Don't: phones with black/empty screens (except as a mockup base), stock people
staring at nothing, AI faces with obvious artefacts, purple/red duotones over faces.

## 6. Graphic devices

- **Ring & arc** — the `o` icon blown up as a page device: giant ring cropped off the edge
  (letterhead watermark at ~10% tint, presentation folder, envelope, social template corner).
- **Lobe / tab** — tab in the *surrounding background colour* that carries the logo and cuts
  into a gradient hero (web nav, every email header). Outer corner is a pill radius; the two
  joins where the tab meets the hero edges curve **inward** (concave fillets), so it reads as
  the background cutting into the hero rather than a 90° notch. The logo inside must stay
  legible — it is a word that needs to be read — but the lobe supports the content: the hero
  is always the point of the graphic, not the logo.
- ~~**Wave**~~ — *retired 2026-09-17.* The red/white/purple sweeping curve that closed heroes
  (mailer hero bottom, social posts) is no longer part of the system — remove it from any
  design that still carries it.
- **Squircle window** — the AR frame above; also the "Endless Possibilities" media holder.
- **Glass panel** — white 20–30% fill, backdrop blur ~20px, 1px white/40% border, 24–32px
  radius, soft outer shadow; sits on the mesh (feature captions, "OUR MISSION", forms).
- **Tracked tagline pill** — translucent dark pill, white Amenti with wide word-spacing:
  `Scan.  Watch.  Experience.`
- **Dictionary definition** — `phideo · noun · /'fid ē ō/ · plural phideos` + two senses
  (hub `Phideo-hero`, manual p. 1). Use as a hero or intro block.
- **Typewriter reveal** — the "What is Phideo? / Phideo = photo + video" sequence on the
  homepage builds word by word in violet on the pale mesh (Figma `67:421`→`114:543`).
- **Icons** — manual: thin white line icons inside flat circles (red, purple, or purple→red
  gradient), generous breathing room. Web: glossy violet 3-D-ish glyphs (phone in hands, QR
  cluster, phone with play, percent badge) — Sandbox → Icons `290:2471`.

## 7. Components

### Web (from Figma Website + live Breakdance globals)
- **Layout:** section width 1120px, section padding 100px top/bottom, 20px sides, column gap
  32px (live globals). Comps are 1440 wide; hero scenes are 1440×863 scroll-snap scenes.
- **Nav:** logo in white lobe top-left; right: red "DOWNLOAD NOW" pill with cloud icon +
  burger. Transparent over the hero gradient.
- **Buttons:** pill 999px. Primary = **purple #702283** fill, white Poppins SemiBold ("Start
  Free – No Credit Card Needed", "Submit"). Action/CTA on dark = **red** pill ("DOWNLOAD NOW
  FOR FREE", "Get it on the App Store"). Web-only tertiary = violet pill (#B200ED) for active
  filter tabs; inactive tabs = white/60% pill with purple text.
- **Filter tabs:** pills in a row — Posters / Real estate / Retail / Galleries / Photo albums.
- **Feature card:** glossy violet icon left, H3 title in violet, body in purple, on pale mesh.
- **Media caption bar:** wide glass panel under the AR window with one centred line.
- **Forms** (popup "We'll Be In Touch!", support): white pill inputs 999px, placeholder grey,
  purple chevron on selects; on a red→plum gradient card (popup) or a glass panel over the
  support mesh; submit = purple/violet pill. Live forms are Fluent Forms.
- **Leadership card:** plum #702283 card, name in white Amenti uppercase, photo slot, role
  in small caps, bio in Poppins small.
- **Footer:** plum band, links row, Google Play + App Store badges, "© Copyright 2024
  Phideo. All Rights Reserved."

### Email (Mailercloud, 600px)
- Header: white lobe with logo (600×92) → hero 600×363: saturated purple→plum gradient, white
  Amenti Regular headline ~34px with wide tracking, white outline pill sub-line ("Keep
  memories alive", "Join Phideo to accept"), phone-window photo right. (The red/white wave
  that used to close the hero is retired — see §6.)
- Body: centred, Inter today → Poppins (`#5`), purple ink; H2 in Amenti Regular purple
  ("Exciting News!", "Forgot your password?"); bold purple for merge fields
  `{Name}` / `[FirstName]`.
- Button: purple pill, white Poppins Bold 14 ("Accept Invitation", "Reset Password"); beta
  variant violet pill.
- Feature row: circular gradient photo with phone, text right with bullets.
- Signature: "Warmly," + **"The Phideo Team" in red** (or Sherry Turner script signature
  from the hub) + small 2-tone logo.
- Footer: Unsubscribe · View in the browser · postal address `(#10 — currently a Tokyo
  template placeholder)`.

### App (from hub screenshots)
White screens, logo top-centre with "phideo = photo + video"; inputs = light pill with 1px
grey border; **primary button red** pill ("Next", "Share", "Save"); secondary = outline
purple pill ("Download", "Change Photo"); progress bar purple; step titles "Step 1: Select
Photo" in Amenti; App Store screens use "Step 1 / 2 / 3" headings over a phone on a
red→purple corner gradient.

### Print (manual specs)
Letterhead US Letter 300dpi CMYK (ring watermark, gradient footer bar); business card
3.5×2in (front: logo + contact line; back: red/purple split, white icon, QR "Scan me! I'm a
phideo!"); envelope 220×210mm; presentation folder 24×17in; presentation 1920×1080 RGB 72dpi;
social templates 1920×1080. Contact line format: `Phone : … | Website : phideo.io | Mail :
info@phideo.io` / `Address : 18129 Kingsport Drive, Malibu, CA 90265`.

## 8. Motion
Motion sting (hub, 2023-06): the ring draws on, play triangle pops. Web micro-animations
(Sandbox `290:530`): typewriter headline reveal, polaroid cards drifting in, phone window
scaling up, loading ring in purple→red gradient with blur. Keep everything soft — ease-out,
300–600ms, no bounces; the "coming alive" moment (print → video) is the one place to slow
down and let it breathe.

## 9. Voice & copy

Warm, plain, a little astonished. Short declaratives. Second person. Puns on photo/video are
welcome once per piece, not more.

- **Primary line candidates** `(#16)` — web hero: **"Bring Photos to Life. Instantly."**;
  sequence: **"Scan. Watch. Experience."**; email: "Keep memories alive"; site title:
  "Turn your ordinary photos into videos through augmented reality"; social:
  "Revolutionize your memories" / "What if your photos could come to life!".
- **Manual tagline bank** (verbatim): What if pictures could talk? · Making your images talk ·
  More than a memory…it's an experience! · Because every picture is a story · Life doesn't
  stand still…and neither should your photos · If pictures could only speak…well now they
  can! · Photos reimagined! · Know that video you can't find on your phone? It's now at your
  fingertips. · Bringing your photos to life · With Phideo, your images talk to you!
- **Explainers in use:** "Turn any picture into an augmented reality video in seconds—just
  scan and watch the future unfold." · "Phideo merges the physical and digital world, so you
  can experience the future." · "phideo = photo + video" (always lowercase `phideo` in the
  equation, capital `Phideo` in prose).
- **Product nouns:** a *phideo* (the thing you make), *phideos* (plural), *scan* (the verb
  for viewing), *create* (the verb for making).

## 10. Open decisions
All numbered `(#n)` items above are collected with evidence and a recommendation in
[discrepancies.md](discrepancies.md). **Settled:** #1 #2 #3 — the Brand Manual V2 is the
source of truth for the primaries: purple **#702283**, red **#E52329**, manual CMYK for
print. For the rest, until they're settled: build with Amenti headings, Poppins body,
® logo files from the hub, and keep the violet family off anything printed.
