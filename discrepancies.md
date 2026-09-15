# Phideo — discrepancies between the sources

> Audited 2026-09-15 against the Brand Manual V2 (PDF), the asset hub, Figma "Phideo Website",
> Figma "Mailer Designs" and the live phideo.io. Each item: what disagrees, the evidence, and
> a recommendation. **Decision column is Franco's** — update it here when settled so the
> [design system](design-system.md) can drop the `(#n)` flags.

| # | topic | decision |
|---|---|---|
| 1 | purple hex | |
| 2 | red hex | |
| 3 | CMYK values for print | |
| 4 | web violet/pink family | |
| 5 | typefaces (Amenti + which body font; licence) | |
| 6 | type scale | |
| 7 | Amenti weight names | |
| 8 | ® on the logo | |
| 10 | contact details / mailer footer address | |
| 11 | gradient: linear brand vs web mesh | |
| 12 | live-site brand variables still defaults | |
| 15 | mission/vision wording | |
| 16 | primary tagline | |
| 19 | body-text colour | |

---

### 1 · Purple — four values for the same colour
- Manual spec (p. 10): **#702283** / R112 G34 B131.
- Manual's own rendered swatches, tints and headings: **#6F2B90** (CMYK→RGB conversion of C70 M100 Y0 K0; also #732B8F in the running text).
- Logo SVGs on the hub (`Logo_Final-color.svg`): **#722C8F**.
- Figma Mailer variable "Deep Plumb": #702283. Live site `--bde-palette-title`: #702283. Website Figma "Endless Possibilities" heading: #702283.
- **Recommend:** #702283 everywhere. Re-export the five logo SVG/PNGs with #702283 / #E52329 fills so the logo and the UI stop being ~1 step apart on the same page. Low risk — the drift is barely visible, but a design system with two purples is not a system.

### 2 · Red — same story
- Manual spec: **#E52329**. Manual render: **#EE2F35** (and #ED1C26 on the cover logo). Logo SVGs: **#EC1B25**. Figma var / live site: #E52329.
- **Recommend:** #E52329; fix the logo files together with #1.

### 3 · CMYK — manual vs asset hub
- Manual: purple **C70 M100 Y0 K0**, red **C0 M95 Y85 K0** (designed values, printed on the stationery).
- Asset hub "Colors" cards: purple **15,74,0,49**, red **0,85,82,10** — auto-derived from the hex by Brandbay; 49% black in the purple would print muddy.
- **Recommend:** the manual's CMYK for anything printed; correct the hub cards (or delete CMYK from them) so a printer never picks the wrong ones up.

### 4 · The web violet/pink family is not in the manual
- Manual: "we do not have a secondary palette"; tints "should be used sparingly"; primaries at full saturation.
- Website Figma + live site: **#B200ED** violet on feature titles, the typewriter headline, active tabs; #BF1DF5 hover; #B778FA / #CC9CFE / #E5AAF9 glossy icons and pills; **#BE38EA** and **#DC2875** as named live-site palette entries; #F4A3A5 blush and lavender haze across every content section.
- The mailers and social posts do **not** use it — they stay on #702283 / #E52329 and the linear gradient.
- **Recommend:** keep it, but formalise it as a *digital-only* "AR glow" set (web, app, motion) with the rule "never on print, never in the logo, never as body text". It does real work: it is the visual difference between the still print (brand purple) and the living overlay (violet). If you'd rather stay pure to the manual, the fallback is purple tints from the table — but the site would lose its glow and needs a recolour pass.

### 5 · Typefaces — five different answers
| source | headings | body |
|---|---|---|
| Manual | Amenti | **Aller** (Regular/Bold — embedded in the PDF, never named) |
| Asset hub → Fonts | Amenti | Amenti Regular |
| Figma Mailer | Amenti | **Inter** (var `font/family/Modern`) |
| Figma Website + live site | **Poppins** | Poppins (+ Montserrat and Oxanium loaded) |
| Social posts (hub) | Amenti | Amenti + a Lora-like serif + a condensed sans |

- Amenti files on the hub come from an Envato Elements zip (`amenti-clean-modern-sans-2023-03-18…`). Elements' licence covers a registered end product; webfont self-hosting is usually fine but needs the download registered against "phideo.io" — worth 5 minutes to confirm before it ships in CSS.
- **Recommend:** Amenti for display/headings on every surface (it *is* the wordmark), **Poppins** for body/UI/email (already live, free, geometric, pairs cleanly). Retire Aller, Inter, Montserrat, Oxanium, the serif and the condensed sans. Replace Poppins headings on the site with Amenti once licence is confirmed; if it can't be licensed for web, Poppins SemiBold headings on web only.

### 6 · Type scale — three of them, none for the web
- Manual p. 15 (measured): H1 60 Black · H2 42 Black · H3 30 Bold · H4 20 Medium · Body 10 Medium · Small 8 Regular.
- Hub: H1 72 Black · H2 35 Black · H3 22 Bold · H4 18 Medium · Body 12 Regular · Subtitle 8 Regular.
- Live site: Breakdance defaults — h1 32px, h2 25px, body 14px, ratio 1.25; components override ad hoc.
- **Recommend:** adopt the proposed web scale in the design system (§3) and mirror it to the hub cards so the three agree; keep the manual's as the print scale.

### 7 · Amenti weight names
- Manual lists Regular / Medium / SemiBold / Bold / ExtraBold. Fonts embedded in the same PDF and on the hub: Thin / Regular / Medium / Bold / **Black**. There is no SemiBold or ExtraBold file.
- **Recommend:** use the file names; "Black" wherever the manual says ExtraBold.

### 8 · ® on the logo
- Manual (2023): no ®. Hub `Logo_Final-*`, Figma "updated logos" `875:554`, website, mailers, social profile pictures: **®** top-right of the icon.
- **Recommend:** treat the ® files as current and the manual's logo page as outdated — but confirm the mark is actually registered (USPTO) before it goes on print runs; if it's only filed, that's ™.

### 10 · Contact details
- Stationery mockups: phone **+1 233 456 7890** (placeholder). Manual back cover: **+1 310 266 0412**. Address everywhere: 18129 Kingsport Drive, Malibu, CA 90265.
- Mailer footers (all three comps): "Tsukamoto Sogyo Building, Basement 1st Floor, 2-15, Ginza 4-chome, Chuo-ku, Tokyo, Japan" — Mailercloud template text.
- Manual footer © 2023 vs site footer © 2024.
- **Recommend:** confirm the real phone with the client; replace the mailer footer address before any send (CAN-SPAM needs a valid postal address); site footer year → current.

### 11 · Gradient — linear brand vs web mesh
- Manual: gradients are **linear, diagonal top-left → bottom-right**, purple↔red only, logo on top in white.
- Website: **mesh/blob** gradients with white, lavender, blush and violet; heroes red-plum, content sections mostly white. Not the manual's gradient at all.
- **Recommend:** two named gradients — *brand gradient* (linear, for print/social/avatars) and *AR mesh* (web/app backgrounds). Same primaries, different medium. Document both; don't let the mesh drift onto print.

### 12 · Live site globals never set
- `--bde-brand-primary-color` is still Breakdance's default **blue #3B82F6**; `--bde-body-text-color` is **#ccc**; headings colour is grey-900. Brand colours only exist as three ad-hoc palette entries (title #702283, pink #DC2875, pink-highlight #BE38EA) and inline #B200ED.
- **Recommend:** set the Breakdance globals (primary = #702283, hover = #8D4E9C or violet per #4, body text = #702283, fonts per #5) so new elements inherit the brand instead of blue.

### 15 · Mission / vision wording
- Manual: "To increase the value of individuals and brands by linking video to a physical image using technology that is quick and easy to use." / "To create a faster, easier and more effective way of sharing information…" / purpose "To delight, entertain and educate…".
- About-us comp: "Our mission is simple: to increase the value of photos and images by making them interactive through video. Our vision is to redefine how people share memories, information, and digital content by seamlessly merging physical images with digital content."
- **Recommend:** the client's call — the About comp reads better and drops "individuals and brands", which may or may not be intended. Use one text everywhere.

### 16 · Primary tagline
- In circulation: "Bring Photos to Life. Instantly." (web hero) · "Scan. Watch. Experience." (web + email) · "Keep memories alive" (welcome email) · "Turn your ordinary photos into videos through augmented reality" (site `<title>`) · "Revolutionize your memories" / "What if your photos could come to life!" (social) · plus the manual's ten-line tagline bank.
- **Recommend:** one primary ("Bring Photos to Life. Instantly." — it names the mechanism and matches your brief), one process line ("Scan. Watch. Experience."), and the bank stays as social/ad variants. Copy goes through review — this one is the client's to pick.

### 19 · Body-text colour
- Manual sets descriptive body copy in **red** Aller (hard to read at 10pt, and red is reserved for action). Mailers and the website set body in **purple** #702283. Live site global is #ccc.
- **Recommend:** body ink = #702283 on light grounds, white on dark; red only for CTAs and the "The Phideo Team" signature.

---

Minor, no decision needed: the hub's **Amenti Black** preview file (`Fonts/D4T9whAmenti Black.ttf`) returns 403, so the Heading 1/2 cards on the Fonts page render in a serif fallback — re-upload it (the Bold/Medium/Regular files are fine). the manual's "Not accepted" panel shows the logo in red-on-purple and purple-on-grey — both are contrast failures (2.05:1 red/purple), so the rule is already right. Social profile pictures put the white wordmark on the gradient, which follows the manual. The Website Figma's variables (Inter, blue #4094F7, greys) are a leftover UI kit — ignore them, don't build on them.
