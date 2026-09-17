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

Two primaries plus a **digital-only secondary palette** (settled 2026-09-17, #4/#5 — the
manual's "no secondary palette" now applies to print and social, which stay on the
primaries). Red is the **action** colour — buttons, links, anything tappable. Purple
carries structure and mood.

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
- **Gradient choice (settled 2026-09-17, #11):** both gradients are in the system, chosen by
  **tone, not medium** — cleaner, lighter compositions take the AR mesh; more striking,
  saturated pieces take the linear brand gradient. On print/social, where the secondary
  palette isn't available, build the mesh from primary tints.
- **AR mesh**: soft radial blobs of purple, red, the web violet and pink
  over white/lavender; blurred, no hard edges. Hero variant is saturated (red + plum, the two
  primaries only); content-section variant is pale (mostly white, lavender #EEC7FB-ish and
  pink #F4A3A5-ish haze). Six reference boards live in Figma Sandbox → Gradients `290:2436`.

### Secondary palette — digital only ✅ *settled 2026-09-17*
The "AR glow" family is the official secondary palette, anchored on the violet. It reads as
the "alive" side of the real/digital split — the AR overlay icons, active filter pills and
feature titles — while brand purple stays with the still print:

| token (proposed) | hex | seen |
|---|---|---|
| `violet` | **#B200ED** | feature titles, typewriter headline, active pill, live-site CSS |
| `violet-hover` | #BF1DF5 | button/pill hover states in Figma |
| `violet-soft` | #B778FA · #CC9CFE · #E5AAF9 | glossy icons, pill fills, haze |
| `pink-highlight` | #BE38EA | live site `--bde-palette-pink-highlight` |
| `pink` | #DC2875 | live site `--bde-palette-pink` |
| `blush` | #F4A3A5 | mesh haze |

Rule: **digital surfaces only** (web, app, email accents, motion). Print and social stay on
the primaries. Never in the logo, never as body text. White on violet is 5.1:1 (AA).

### Neutrals
White #FFFFFF; ink = purple #702283 for headings **and** body on light grounds (mailer and web
both do this — `(#19)`); grey text #404041 (manual folios); light glass tint = white at
20–35% over the mesh; input borders #DCDCDC / #E5E7E7 (live site).

## 3. Typography ✅ *#5 #6 #7 settled 2026-09-17*

**The rule set:** two media, one voice. **Digital** (website, app, email) = Amenti for
display and headings, **Poppins** for body and UI. **Print & social stay on brand** =
Amenti throughout, per the manual. Aller, Inter, Montserrat, Oxanium, the serif and the
condensed sans are retired.

### Brand typeface — Amenti
Geometric sans with single-storey `a`, the face of the wordmark and of every headline in the
manual, the hub, the social posts and the mailers. Weight names are normalized to the files
(#7): **Thin, Regular, Medium, Bold, Black** — "Black" wherever the manual says ExtraBold,
"Bold" for SemiBold. Licence: Envato Elements zip — confirm webfont/end-product rights
before self-hosting.

Manual hierarchy (p. 15, measured): H1 60 Black · H2 42 Black · H3 30 Bold · H4 20 Medium ·
Body 10 Medium · Small 8 Regular. Hub hierarchy: 72 / 35 / 22 / 18 / 12 / 8. Manual eyebrows =
Amenti Regular 12, uppercase, tracked ~0.5em (`T Y P E F A C E`), red.

### Body / UI typeface — settled
**Poppins** for body, UI, forms and email body on all digital surfaces (already live,
geometric enough to sit under Amenti, free). Print and social body copy stays in Amenti.
Historic drift, now retired: Aller (manual body), Inter (mailers), Montserrat + Oxanium
(live site), the Lora-like serif and condensed sans (social). If Amenti cannot be licensed
for web, Poppins SemiBold takes headings on web only and Amenti stays print/social.

### Digital type scale — normalized (Amenti + Poppins, desktop → mobile)
**Normalized 2026-09-17 (#6):** modular scale, major third (**×1.25**) from the 18px body,
rounded to even px: **14 · 18 · 22 · 28 · 36 · 44 · 56**. Mirror these to the hub cards;
print keeps the manual's pt hierarchy.
| role | face | size / line | notes |
|---|---|---|---|
| Display | Amenti Black | 56/64 → 40/46 | hero only; +0.02em |
| H1 | Amenti Black | 44/52 → 34/40 | +0.02em |
| H2 | Amenti Bold | 36/44 → 30/36 | +0.03em; "Endless Possibilities" is this, in purple |
| H3 | Amenti Bold | 28/36 → 24/30 | +0.03em; feature titles (violet on web) |
| H4 | Amenti Medium | 22/30 | +0.03em; card titles |
| Body | Poppins Regular | 18/28 → 16/26 | purple ink on light, white on dark |
| Small | Poppins Regular | 14/20 | captions, legal, footer |
| Eyebrow | Amenti Regular | 14, uppercase, +0.4em | red on light, white on dark |
| Tagline lockup | Amenti Medium | 20, +0.25em | "Scan.  Watch.  Experience." — extra word-spacing |
| Button | Poppins SemiBold | 16 | |

**Tracking rule (set 2026-09-17):** Amenti never runs tight or default — it always gets
positive letter-spacing, graded by size: **+0.02em** at Display/H1, **+0.03em** at H2–H4,
**+0.04em** on small Amenti labels (weight names, swatch labels, card names). The alphabet
specimen runs at +0.08em with 0.6em word gaps as the reference for the open feel. Eyebrows
(+0.42em) and the tagline lockup (+0.25em) keep their existing wide tracking. Poppins body
runs at its default spacing.

Live site today: Breakdance globals h1 32px, h2 25px, body 14px, base 16, ratio 1.25 — not a
designed scale, override.

## 4. Logo

- **Wordmark** "phideo" in Amenti-derived lettering: `phi` purple, `de` red, the `o` is the
  app icon — a purple ring, open top-right, with a red play triangle; a red arc closes the
  ring. Construction and clearspace on manual pp. 6–7 (clearspace ≈ the height of the `o` on
  all sides; icon alone gets the same).
- **The mark is registered (settled 2026-09-17, #8): the logo carries ® across the board** —
  hub `Logo_Final-*`, Figma "updated logos" `875:554`, website, mailers, print. The manual's
  logo page pre-dates the registration and is outdated.
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

### The o as the mark (added 2026-09-17)

The `o` stands alone as the brand mark: it is the **play affordance on every video surface**
and the "this is a phideo" badge on prints, posters and tags. **No generic ▶ triangle appears
anywhere** in the product, site or communications — if it plays, it's the o.

Colour is decided by the ground (contrast first, per overlay-control best practice):

1. **Full colour** (purple ring + red arc + red triangle) — white and light neutral grounds
   only, where both colours hold contrast: marketing pages, packaging, the printed tag.
2. **Monotone white** — on brand gradients, brand colours, dark UI, and **always over
   photography/video** (overlay play controls are monochrome white, industry standard).
   A soft drop shadow is allowed for separation; no containing circle or pill.
3. **Monotone purple (or black)** — one-colour print, engraving, embossing; also the
   fallback at small sizes.

Construction never changes: ring open top-right, arc closing it, triangle pointing right;
all three pieces recolour together, never independently — and never violet. Minimum size
16px; from 16–24px use monotone (the two-colour split stops reading). The o alone doesn't
carry the ®; that belongs to the full logo.

### Icon usage (added 2026-09-17)

**The o's own ring is the button.** The play mark is never wrapped in a disc, circle,
pill, badge or second ring — double-ringing muddies the mark and makes it read as a
generic player control. Wherever something plays, the bare o sits directly on the media
or gradient, monotone white, nothing drawn around it.

- **Do:** bare o, monotone white, straight on the media/gradient; a soft drop shadow
  (~20–40% opacity) is the only separation allowed.
- **Don't:** no containing disc, no outer ring, no glass badge, no tinted or greyed o.
- **Hit area ≠ glyph:** grow the touch target invisibly (≥44px); the drawn icon stays bare.
- **Colour:** white over media, gradients and dark UI; full colour only on white/light
  neutrals; single-colour purple/black for one-colour print (see "The o as the mark").
- **Everything else:** icons that aren't play affordances follow the icon families —
  print: thin white line icons in flat red/purple/gradient circles; web: glossy violet
  glyphs. The circle treatment belongs to *those* icons, never to the o.

## 5. Imagery — the AR language

### The mechanic (canon, 2026-09-17)

What actually happens when a phideo plays — every photograph, video and marketing composite
must depict this correctly:

- **The photo itself comes to life.** With the naked eye you see a still print. Through the
  phone, the *same* photograph is moving footage. The phone is a **window into the digital
  world**, not a player for separate content.
- **The life stays inside the photograph's own frame.** The motion never spills past the
  print's edges, never cuts away, never becomes a different scene. Frame on the wall =
  frame of the video.
- **The two eyes don't match exactly.** The phone's view may be modestly **zoomed in**
  relative to the naked eye — a tighter crop of the same image — so the motion reads
  clearly on the small screen. Framing, subject and palette are always the print's own.
- **In any shot where print and screen share the frame:** the screen shows the same image
  as the visible print (slightly tighter crop allowed), unmistakably alive — spray, drift,
  motion light — and brighter/more saturated than the still print beside it. The print
  itself must read as frozen. Full-bleed footage, no app chrome. Never unrelated footage
  on the screen.

Reference film: `photography/phideo-mechanic-demo.mp4` — first-person museum demo, the
painting still on the wall, alive inside the phone.

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

### Photography direction (added 2026-09-17)

Reference shoot in `photography/` (six shots, Higgsfield Soul 2.0 / Soul Cinema, 2K).
Every shot is directed like a sentence — one message, one composition, one light, one honest
expression — and brand colour enters as **objects and light inside the scene** (plum ribbon,
red pencil, plum mug, red raincoat, violet screen glow), never as a filter in post.

Two registers: **everyday** (warm, window-lit: The Moment, Demonstrate, The Gift) and
**campaign** (low-light, the screen carries the colour: Looking, The Wall, Two Worlds).
The darker the scene, the more the screen becomes the light source.

Rules for photos in layouts:

1. **The plum scrim** — type never sits raw on a photograph. Gradient from transparent to
   `rgba(43,10,52,.84)` (near-black plum, not grey) rising from the edge that carries the
   type, covering the bottom ~55–65%. Type on it is always white. On very dark photos a
   neutral near-black scrim at lower opacity is enough.
2. **The screen is sacred** — scrims, washes and logos never dim the phone screen; it stays
   the brightest, most saturated element. Anchor the scrim away from the screen.
3. **Accents in-scene, not in post** — no duotones, no colour overlays on faces, no
   recolouring. Plant the brand colour at the shoot.
4. **Containers do the branding** — photos live inside brand geometry: 18–28px radii or the
   squircle window, the lobe carrying the logo top-left, the scrim carrying the type.

**Photo as the hero:** same anatomy as the gradient hero — lobe top-left, content centred
horizontally — but the content drops to the bottom edge onto the scrim (the photo is the
content; don't float type mid-image). Eyebrow goes lavender `#E9D5F5`, headline white,
red keeps its one job (the primary action). In email, the photo-hero marketing template and
the dark story/editorial template in the style guide are the references; soft sends use a
glass-white pill instead of red.

**Production rule (2026-09-17):** photo-led layouts are never assembled from photos that
already exist. The pipeline is **goal → wireframe → shoot-to-wireframe → CD QA** — the
wireframe fixes where type, CTA and lobe live before the shoot, and the photographer
composes the negative space in camera. Full role briefs, the W1 wireframe and the QA log:
`production-workflow.md`.

## 6. Graphic devices

- **Ring & arc** — the `o` icon blown up as a page device: giant ring cropped off the edge
  (letterhead watermark at ~10% tint, presentation folder, envelope, social template corner).
- **Lobe / tab** — tab in the *surrounding background colour* that carries the logo and cuts
  into a gradient hero (web nav, every email header). The two joins where the tab meets the
  hero edges curve **inward** (concave fillets, radius *r*); the outer corner curves outward
  at up to **lobe height − r**. At that maximum the concave and convex arcs meet tangent —
  one continuous S-curve with no straight segment (the current build: 84px lobe, 32px
  fillets, 52px outer). Exceed it and the arcs no longer meet — the edge breaks. It reads as
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
- **Footer:** plum band, links row, Google Play + App Store badges, "© Copyright {current
  year} Phideo. All Rights Reserved." — keep the year current (#10).

### Email (Mailercloud, 600px)
- **Hero alignment (2026-09-17):** the gradient hero is "blank" — there is no grid to align
  to — so hero content is always **centred**: headline, sub-lines and buttons on one axis.
- **Template family (2026-09-17):** one skeleton (lobe header → hero → body → footer), four
  volumes by intent. Hierarchy comes from the scale of the hero + headline; contrast comes
  from where red is allowed — **red only on the send's primary action**, one CTA per send.
  - *General communication* — the baseline: hero 600×363, Amenti Regular 34px headline,
    tagline pill, purple button, red reserved for the signature.
  - *Marketing* — loudest: hero 600×420, Display-scale Amenti **Bold** headline, tracked
    eyebrow for the campaign name, the send's only **red** CTA inside the hero.
  - *Education / informational* — hero recedes to 600×260 (headline only); the body leads
    with numbered steps (purple circles, bold purple titles, grey detail); purple button —
    learning, not selling.
  - *Automated / transactional* — quietest: no hero; small centred 2-tone logo, a thin
    purple→red gradient rule, utility type, muted reassurance line, purple button.
- **Photo heroes (2026-09-17):** either the marketing or story volume can swap the gradient
  for a photograph (hero 600×420). Content stays centred horizontally but drops to the
  bottom edge onto the plum scrim (§5 photography rules 1–2: type on the scrim, the phone
  screen never dimmed). Warm everyday photo → marketing send with the red CTA on the darkest
  plum; dark campaign photo → story/editorial send with a lavender eyebrow and a glass-white
  pill (no red — red would promote it to marketing).
- Header: white lobe with logo (600×92) → hero: saturated purple→plum gradient, white
  Amenti Regular headline with wide tracking, white outline pill sub-line ("Keep
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
social templates 1920×1080. Contact line format (#10 — **no phone number on public
materials**, no placeholders anywhere): `Website : phideo.io | Mail : info@phideo.io` /
`Address : 18129 Kingsport Drive, Malibu, CA 90265`.

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
All numbered `(#n)` items above are collected with evidence and the decision in
[discrepancies.md](discrepancies.md). **Settled:** #1–#3 (Brand Manual V2 = source of truth
for the primaries: #702283 / #E52329, manual CMYK for print) · #4 (violet family = secondary
palette, digital only) · #5 (digital = Amenti + Poppins; print & social = Amenti, on brand) ·
#6 (modular ×1.25 type scale) · #7 (weight file names) · #8 (mark is registered, ® across
the board) · #10 (no placeholders, no public phone, © current) · #11 (both gradients, chosen
by tone) · #12 (set the live-site globals). **Still open:** #15 mission wording, #16 primary
tagline, #19 body-text colour — the copy calls are the client's.
