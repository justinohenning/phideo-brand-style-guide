# Phideo — photo-led production workflow

*Added 2026-09-17 after the first photo-hero pass failed QA: the photography was strong and
the layout was strong, but they were made independently — so the type landed on the most
important part of the image and both lost their impact. The fix is sequence, not talent.
Nothing photo-led ships without passing through all four roles, in order.*

## The pipeline

Every photo-led deliverable (web hero, email hero, social, OOH) runs:

```
1. GOAL        what the piece must make the audience feel/do (producer + client)
2. WIREFRAME   the layout decides placement first: type, CTA, logo, safe zones
3. SHOOT       the photographer shoots TO the wireframe — negative space is
               composed in-camera where the type will live
4. CD QA       the Creative Director signs off against four gates:
               meets the goal · aesthetically strong · on brand · mechanically true
```

A deliverable that skips a step goes back. A photo that wasn't shot to the wireframe is a
gallery/reference asset, not a layout plate.

## Role briefs (use these as agent prompts)

### 1 · Producer — the goal

One paragraph, written before anything visual: audience, the single feeling, the single
action, the register (everyday warm / campaign dark — see design-system §5). No layout, no
art direction. Every later role is measured against this paragraph.

### 2 · Designer — the wireframe

The wireframe fixes **where things live** before the photo exists:

- **Zone A — lobe** (logo tab): top-left. The image will be covered there; nothing
  important may live under it.
- **Zone B — subject**: where the story happens (faces, the phone screen, the print).
  The screen is the single brightest point and must sit whole inside Zone B.
- **Zone C — type + CTA**: where the copy and button sit, on the plum scrim. The photo
  must offer **low-detail, low-contrast negative space** here — floor, table, blanket,
  wall, shadow, out-of-focus foreground. No faces, no hands, no prints, no screen.
- Margins: nothing critical within 8% of any edge (crop tolerance across placements).

#### W1 — photo hero (web + email), the standard wireframe

```
+—————————————————————————————————————+
| [A lobe]                            |
|                                     |
|            ZONE B  (top ~55%)       |
|      subject · faces · screen       |
|                                     |
|-------------------------------------|
|            ZONE C  (bottom ~45%)    |
|     quiet negative space + scrim    |
|       eyebrow / headline / CTA      |
|          (centre-aligned)           |
+—————————————————————————————————————+
```

Formats: email hero 600×420 (shoot 3:2, minimal crop) · web hero ~21:9 (shoot 21:9).

### 3 · Photographer — shoot to the wireframe

The shot brief = the photoshoot direction (message, composition, lighting, expression,
environment, in-scene brand accent — design-system §5) **plus the wireframe zones as
hard constraints**. Compose the negative space in camera: a foreground surface, a fall
to shadow, an empty wall. Do not plan to "fix it with the scrim" — the scrim is for
legibility, not for burying detail.

**The mechanic is canon** (design-system §5, "The mechanic"): whenever a print and a
screen share the frame, the screen shows the *same* image as the print — a slightly
tighter crop is allowed (the phone is a zoomed-in window) — visibly alive and brighter
than the frozen print beside it. The life stays inside the print's frame. Never unrelated
footage, never app chrome, never a screen that contradicts the print it faces.

### 4 · Creative Director — QA gates

Review the **final composite** (photo + scrim + type + lobe + CTA), never the photo alone:

1. **Goal** — does the piece deliver the producer's paragraph at a glance?
2. **Impact** — is the subject unobstructed? Type entirely on negative space? Screen
   the brightest point? Would you stop scrolling?
3. **Brand** — scrim per photography rule 1, screen sacred per rule 2, accents in-scene
   per rule 3, containers per rule 4; type scale, tracking and red-usage per the system.
4. **Mechanic** — if a print and a screen share the frame: same image on both, screen a
   slightly tighter living crop, print frozen, life inside the print's frame
   (design-system §5, "The mechanic"). A screen showing unrelated footage is an automatic
   reshoot, not a fix.

Verdict: **ship / fix (specific notes) / reshoot**. Two failed fixes = reshoot.

## Worked briefs — 2026-09-17 reshoot

### Plate M — marketing email hero ("The Moment II")
- **Goal:** a warm jolt of recognition — "my family's photos could do this" — that earns
  one tap on *Bring One to Life*. Everyday register.
- **Wireframe:** W1 at 600×420. Zone B: grandmother + granddaughter + glowing screen,
  upper 55%. Zone C: the plum throw blanket and sofa sweeping the bottom 45%,
  out of focus.
- **Shot brief:** golden-hour living room, camera at chest height so the sofa back and
  blanket fill the foreground; faces and phone in the upper half; 50mm f/2; plum blanket
  as the in-scene accent. 3:2.

### Plate S — story email hero ("Two Worlds II")
- **Goal:** editorial gravity — "there's more to this product than a gimmick" — that earns
  a *Read the Story* click. Campaign register.
- **Wireframe:** W1 at 600×420. Zone B: the B&W print + phone with the living sunset,
  upper 55–60%. Zone C: the charcoal studio wall falling to black, bottom 40–45%.
- **Shot brief:** single spotlight from above so the light pools on the print and dies
  before the bottom of frame; phone screen upper-right; 3:2.

### Plate W — web photo hero ("The living side")
- **Goal:** instant comprehension of the product promise over a full-width hero, with a
  centred red CTA. Campaign register.
- **Wireframe:** W1 at ~21:9. Zone B: print + phone upper 55%, right of centre balanced
  by the lobe top-left. Zone C: empty dark wall/table across the full bottom width.
- **Shot brief:** the Two Worlds studio concept recomposed for 21:9: print and hand-held
  phone raised into the upper half, spotlight tight, bottom half of frame near-black
  empty space. 21:9.

## QA log — 2026-09-17 (all three shipped)

Final plates live in `photography/plate-{m,s,w}.png`; composites in the style guide
(photo-hero demo + the two photo-hero email templates).

- **Photographer's cull:** first 21:9 web plates rejected — layout language in the shot
  brief ("built to carry type") got rendered as literal baked-in text. Lesson: shot briefs
  describe *light and space*, never layout or typography. Reshot clean.
- **CD round 1:** web — eyebrow touched the print's bottom edge → hero made taller, type
  block moved down. Marketing — screen read as a photo grid / camera viewfinder, dimmer
  than the faces → plate reshot, then the screen replaced via a targeted image edit (one
  full-bleed living video, no UI chrome, graded brighter than the faces). Also a
  producer-side lesson: give the CD full-frame exports — two round-1 flags were artifacts
  of cropped review exports.
- **CD round 2:** web SHIP · story SHIP · marketing FIX (screen content).
- **CD round 3:** marketing SHIP — saturation measured: screen 0.55 vs faces 0.45. One
  non-blocking note on file: +⅓ stop on the screen if the plate is ever touched again.

## QA log — mechanic demo film (2026-09-17)

`photography/phideo-mechanic-demo.mp4` — first-person museum demo of the mechanic
(directed GPT-Image start frame → image-to-video, 8s, 1080p).

- **Take 1 (Kling 3.0, slow push-in):** FAIL on the mechanic — the wall painting's sea
  visibly animated. Lesson: camera movement forces the model to re-render the whole scene;
  a "frozen background" brief needs a locked camera.
- **Take 2 (Kling 3.0, locked camera, hard freeze language):** better — gallery rock
  solid — but the painting's waves still drifted subtly. FAIL.
- **Take 3 (Seedance 2.5, same locked-camera brief):** SHIP — painting pixel-stable
  across the full 8s, all motion inside the phone screen. Lesson on file: for
  selective-motion shots ("only X moves"), Seedance holds the frozen regions; Kling
  wants to animate everything it sees.
