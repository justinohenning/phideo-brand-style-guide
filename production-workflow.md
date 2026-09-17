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
tighter crop is allowed (the phone is a zoomed-in window), and the print's frame visible
*inside* the screen is the strongest live-camera read — visibly alive and brighter
than the frozen print beside it. The life stays inside the print's frame. Never unrelated
footage, never app chrome, never a screen that contradicts the print it faces.

**The crew (every shot brief is written by five roles, in this order):**

- **Creative director** — the one-sentence message the frame must say, and the register.
- **Photographer** — POV, lens, camera height, composition; point of interest placed per
  the wireframe; always framed a little wider than instinct.
- **Set dresser** — environment and props; the brand accents planted *in scene* (plum
  ribbon/mug/throw, red pencil/raincoat/thread) — never colour in post.
- **Lighting specialist** — the light plan: source, temperature, falloff; the phone screen
  is always the single brightest, most saturated point; quiet zones fall away in *light*
  (shadow, out-of-focus foreground), not in retouching.
- **Graphic designer** — what the screen shows (the same image as the print, alive, per
  the mechanic) and, on layout plates, the copy footprints the composition must keep quiet.

One prompt/brief carries all five voices; a brief missing a role's answer isn't ready to shoot.

### 4 · Creative Director — QA gates

Review the **final composite** (photo + scrim + type + lobe + CTA), never the photo alone:

1. **Goal** — does the piece deliver the producer's paragraph at a glance?
2. **Impact** — is the subject unobstructed? **Nothing overlaps the point of interest** —
   the lobe, logo, type and badges never sit on the subject, above all on faces (an
   overlapped focal point is the fastest "an AI made this" tell). Type entirely on
   negative space? Screen the brightest point? Would you stop scrolling?
3. **Brand** — scrim per photography rule 1, screen sacred per rule 2, accents in-scene
   per rule 3, containers per rule 4, focal point uncovered per rule 5, orientation lock
   per rule 6; **brightness floor** — fun, bright brand: drama comes from light and
   colour, never a dark room; type scale, tracking and red-usage per the system; the
   send's CTA is a real brand button (red pill on dark, purple on light — never glass).
4. **Mechanic** — if a print and a screen share the frame: same image on both, screen a
   slightly tighter living crop, print frozen, life inside the print's frame
   (design-system §5, "The mechanic"). **Orientation lock:** the screen shows what a real
   camera would see — matching orientation, or the print's edges inside the screen, or an
   unmistakable zoomed detail; a portrait screen full-bleeding an entire landscape print
   is an automatic FIX. A screen showing unrelated footage is an automatic reshoot.

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
- **Shot brief:** bright airy daylight studio (brightness floor applies — no dark rooms);
  landscape print pinned to a warm sunlit wall, **landscape** phone in camera mode over it
  (orientation lock); cluster upper half right of centre; the lower frame quiet lit wall
  easing to gentle shadow. The plum scrim supplies the type contrast, not the scene. 3:2.

### Plate W — web photo hero ("The living side")
- **Goal:** instant comprehension of the product promise over a full-width hero, with a
  centred red CTA. Campaign register.
- **Wireframe:** W1 at ~21:9. Copy footprint bottom 45%, centred → point of interest
  (print + phone) framed in the upper half, right of centre to balance the lobe top-left;
  empty dark wall/table runs the full bottom width. Shot wider than the crop.
- **Shot brief:** the Two Worlds studio concept recomposed for 21:9: sunlit wall, landscape
  print with a **landscape** phone in camera mode raised into the upper half right of
  centre; upper left quiet lit wall; the full-width bottom band quiet wall easing to soft
  shadow — lit, never black (brightness floor). The plum scrim carries the type. 21:9.

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

## QA log — full library reshoot (2026-09-17, all nine shipped)

Once the mechanic became canon (see the demo-film log below), the entire photography
library — six reference shots + three layout plates — was reshot on GPT-Image 2.5 (2K),
every brief written by the five-role crew, every image gated on the mechanic.

- **Batch 1 (9/9 generated):** photographer's cull passed all nine — no text artifacts
  (the light-and-space prompt language from the earlier lesson held), mechanic read strong
  across the set, and the camera-mode read (print's frame visible inside the screen)
  landed on The Wall, Two Worlds and both studio plates.
- **CD round 1:** six of nine SHIP. Three FIX — The Wall: phone floated beside the frame
  it was "viewing" instead of overlapping it (camera-geometry break); The Gift: the screen
  showed a *different* wedding moment than the print (mechanic violation, automatic fix);
  Plate M: heads inside the 8% top-edge clearance.
- **Fix pass:** all three repaired as targeted image-to-image edits on the approved takes
  (reposition the phone over its frame; replace the screen with a tighter living crop of
  the print's own scene; reframe wider for headroom) — cheaper and more consistent than
  reshooting, since the rest of each frame was already approved.
- **CD round 2:** nine of nine SHIP — occlusion geometry, screen-to-print match and
  measured 8.2%/9.4% crown clearance all verified. Lesson: the mechanic gate catches
  subtle breaks (a matching-but-different moment on the screen) that a general "on brand"
  review sails past; keep it as its own gate.
- **Composite round (the workflow's real gate — never the photo alone):** web hero SHIP;
  marketing FIX — the 600×420 crop pushed the headline off the scrim onto the cardigan →
  type block lowered (padding 6→2.5cqw) and the scrim start raised (36→32%); story FIX —
  the lobe covered the print's top-left corner and the crop had no slack (phone already on
  the right edge) → the *plate* was reframed wider via a targeted edit (cluster smaller,
  right of centre, 12% margins) rather than fighting the crop. Bonus: the reframe put the
  phone overlapping its print — a stronger live-camera read. Final: all three composites
  SHIP. Lesson: when a crop has no slack, fix the plate, not the layout.

## QA log — client design review, story email (2026-09-17)

The client reviewed the shipped story email and failed it on four counts. All four are now
codified (photography rules 5–6, the brightness floor, the CTA rule) so no future pass
repeats them:

- **Too dark.** "This brand is fun and bright; the image doesn't reflect that." The
  campaign register had drifted from *dramatic* to *murky*. → Brightness floor added:
  drama comes from directional light and rich colour, never a dark room.
- **The lobe overlapped the print** — the focal point. "I now know that an AI designed
  this and I immediately don't like the design." → Rule 5: no overlay ever sits on the
  subject, above all faces; if the lobe would touch the subject, the plate is wrong, not
  the layout.
- **The CTA read as off-brand.** The glass-white pill didn't feel like a primary button —
  because it wasn't one. → The glass pill is retired as a CTA; every send's action is a
  real brand button (red pill on dark grounds, purple on light).
- **Orientation break.** Landscape print on the wall, portrait full-bleed image inside
  the phone — "that destroys the illusion that it's the same thing and his phone is in
  camera mode." Audit found the same break on the web plate. → Rule 6 (orientation lock)
  added to the photography rules and the CD mechanic gate.

Fix: both studio plates (S and W) reshot from the approved Two Worlds frame — bright airy
studio, landscape print with a **landscape** phone in camera mode — solving brightness and
orientation in one move; story CTA switched to the red pill; story scrim moved to plum.

**Fix-round CD QA:** web hero SHIP first pass (after the type block was tightened to clear
the print's bottom edge — the taller hero flips the cover-crop to the horizontal axis and
reveals the plate's full quiet band). The CD then flagged the marketing send: the new
rule-5 gate caught the lobe grazing the grandmother's hair — a break the earlier "on
brand" reviews had sailed past. Crop slack was exhausted, so per doctrine the *plate* was
reframed (pair right of centre, upper-left quarter quiet sofa/bokeh, full headroom), not
the layout. Final round: all three composites SHIP. Watch item: ~10px headline-to-hand
clearance on marketing — no room for further upward cropping.

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
- **Take 5 (explicit trajectory):** shipped, then pulled after client review — pan brief
  rewritten as start position → end position ("hand starts in front of the LEFT side…
  glides to the RIGHT side"), 10s. The arm travels and the viewfinder tracks — but the
  pan read as mechanical (constant robotic speed) and the footage inside the screen
  played in heavy slow motion, which hides the very thing being sold: that the photo is
  now a *video*. Lessons: (a) video models ignore vague motion verbs — write trajectories
  as explicit start/end positions; (b) motion cues (frame inside the screen + a moving
  hand) are what sell "camera, not playback".
- **Take 6 (natural motion + real-time speed):** shipped, then pulled after client
  review — hand movement natural (kept), but two notes: the locked-down camera should be
  a first-person POV from the person holding the phone, and the screen *still* read as
  slow motion ("I was expecting waves crashing and the ship riding them through the
  roughness; instead a slow clip of sea slowly moving"). Naming the speed ("real-time,
  no slow motion") wasn't enough — the model nodded and drifted anyway.
- **Take 7 (POV + events, not speeds):** SHIP — two changes. (a) Camera rebriefed as
  first-person POV: "the camera IS the eyes of the person holding the phone — it
  breathes, sways, drifts with a human rhythm, never a locked tripod", with the painting
  pinned as "a physical printed object; the only apparent change is parallax from the
  swaying viewpoint". (b) The screen footage briefed as **scheduled events instead of
  speed adjectives**: "in the very first second a wave breaks against the hull and throws
  spray; the ship pitches and rolls, bow plunging; at least three distinct wave crashes
  in the clip". Verified in QA: crashes land at ~0.5–1.0s and ~6.0–6.5s with whitecaps
  fully reorganising between frames 0.5s apart; the wall painting stays pixel-identical
  under a continuously drifting viewpoint; the gilded frame stays visible inside the
  screen throughout. Lesson: models ignore speed adjectives but obey *scheduled events* —
  brief motion as things that happen at moments, not as a tempo. And POV sway is free
  realism: the world moving while the print stays frozen is itself proof the print is an
  object, not a screen.
