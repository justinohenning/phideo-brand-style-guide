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

A photo hero is **a layered stack, not segments**. The photograph runs full bleed under
everything; the other layers sit on top of it. The photo is never sliced into bands:

```
LAYER 4   lobe (logo tab)        floats top-left over the image
LAYER 3   type + CTA             the only fixed footprint (W1: bottom ~45%, centred)
LAYER 2   scrim                  gradient for legibility under layer 3
LAYER 1   the photograph         full bleed — shot wider than instinct
```

The wireframe fixes the **footprints of the overlay layers** (lobe top-left; type + CTA
per the layout — W1 puts it on the bottom ~45%, centre-aligned) plus the margins rule:
nothing critical within 8% of any edge (crop tolerance across placements).

Its real product is **composition knowledge for the photographer**. Knowing where the
copy layer will land, the photographer:

- places the **point of interest away from the copy footprint** — copy below → subject
  framed higher; copy left → subject framed right; and so on for any axis;
- **shoots a little wider** than instinct, so the layout has reframing room and the
  subject keeps its clearance across placements and crops;
- composes the copy footprint as **naturally quiet image** — floor, table, blanket, wall,
  a fall to shadow, out-of-focus foreground — in camera. No faces, hands, prints or
  screen there. The scrim is for legibility, never for burying detail;
- keeps the phone screen the single brightest point, whole, clear of the copy footprint.

Formats: email hero 600×420 (shoot 3:2, minimal crop) · web hero ~21:9 (shoot 21:9).

### 3 · Photographer — shoot to the wireframe

The shot brief = the photoshoot direction (message, composition, lighting, expression,
environment, in-scene brand accent — design-system §5) **plus the wireframe's layer
footprints as composition knowledge**. Frame the point of interest away from where the
copy layer will sit, shoot wider than the final crop needs, and compose the quiet space
in camera: a foreground surface, a fall to shadow, an empty wall. Do not plan to "fix it
with the scrim" — the scrim is for legibility, not for burying detail.

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
- **Wireframe:** W1 at 600×420. Copy footprint bottom 45% → point of interest
  (grandmother + granddaughter + glowing screen) framed in the upper half; the plum throw
  blanket and sofa sweep the bottom of frame, out of focus. Shot wider than the crop.
- **Shot brief:** golden-hour living room, camera at chest height so the sofa back and
  blanket fill the foreground; faces and phone in the upper half; 50mm f/2; plum blanket
  as the in-scene accent. 3:2.

### Plate S — story email hero ("Two Worlds II")
- **Goal:** editorial gravity — "there's more to this product than a gimmick" — that earns
  a *Read the Story* click. Campaign register.
- **Wireframe:** W1 at 600×420. Copy footprint bottom 40–45% → point of interest (the
  B&W print + phone with the living sunset) framed in the upper 55–60%; the charcoal
  studio wall falls to black beneath it. Shot wider than the crop.
- **Shot brief:** single spotlight from above so the light pools on the print and dies
  before the bottom of frame; phone screen upper-right; 3:2.

### Plate W — web photo hero ("The living side")
- **Goal:** instant comprehension of the product promise over a full-width hero, with a
  centred red CTA. Campaign register.
- **Wireframe:** W1 at ~21:9. Copy footprint bottom 45%, centred → point of interest
  (print + phone) framed in the upper half, right of centre to balance the lobe top-left;
  empty dark wall/table runs the full bottom width. Shot wider than the crop.
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
- **Take 3 (Seedance 2.5, same locked-camera brief):** shipped, then pulled after client
  review — painting pixel-stable, but the static hand read as "a guy watching a clip that
  looks like the painting", not AR. Lesson: freezing the world isn't enough; the phone
  must *prove* it's a live camera.
- **Take 4 (new start frame — camera mode):** start frame regenerated so the painting's
  gilded frame is visible *inside* the phone screen (live viewfinder, not full-bleed
  playback). Painting frozen, camera-mode read strong — but the prompted pan didn't
  happen; the hand barely moved. FIX.
- **Take 5 (explicit trajectory):** SHIP — pan brief rewritten as start position → end
  position ("hand starts in front of the LEFT side… glides to the RIGHT side, travelling
  the width of the painting"), 10s. The arm visibly travels and the on-screen view tracks
  it like a viewfinder — the ship slides into the screen as the phone reaches it — while
  the wall painting stays frozen. Lessons on file: (a) the mechanic's motion cues (frame
  inside the screen + a moving hand) are what sell "camera, not playback"; (b) video
  models ignore vague motion verbs — write trajectories as explicit start/end positions.
