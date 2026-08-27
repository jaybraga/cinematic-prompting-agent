# Worked Example — From Brief to Static-to-Video Prompt

This fictional example shows the workflow in simplified form. It is not a universal style preset.

The brief already defines the subject and basic shot idea, so Shot Research is not needed in this example. If the user had supplied only a broad travel-campaign guideline, the workflow would first use `templates/Shot-Research-Template.md` to develop and approve a proposed shot list.

## 1. Initial brief

> Create a five-second hero shot for a fictional premium travel campaign. A welcome drink sits on a dark stone side table beside a softly lit aircraft window. The feeling should be calm, tactile, and quietly luxurious—not flashy. Incorporate the fictional brand's rust-orange `#C86A3A` as a restrained accent rather than a global tint. The cabin should feel operational and inhabited, with other passengers present in the background without distracting from the drink. I also have a cabin-material reference image available. We will generate the static frames first and animate them later.

## 2. Direction Check

### Recommended direction — Quiet confidence

- **Emotional promise:** private calm and considered service.
- **Visual thesis:** small tactile details feel more valuable than spectacle.
- **Palette/light:** soft warm practical light balanced against cool twilight through the window; `#C86A3A` appears only as a controlled upholstery-piping and service-detail accent.
- **Production design:** dark stone, brushed metal, clear glass, restrained textile texture, and a believable softly occupied cabin rather than an empty showroom.
- **Composition/optics:** layered close observation, controlled negative space, natural perspective, selective focus.
- **Motion principle:** slow and deliberate; nothing calls attention to the camera mechanism.
- **Avoid:** gold-everywhere luxury clichés, excessive bloom, fake particles, aggressive flare, oversharpened materials, or nightclub saturation.

User approves this direction.

## 3. Per-Shot Direction Check

The user asks the agent to propose options.

### Option A — Controlled foreground reveal (recommended)

- **Audience effect:** discovers the service detail gently; premium and intentional.
- **Start:** medium-close composition with the window and seat texture readable; glass present but not dominant.
- **Movement:** stabilized diagonal dolly forward and camera-right, creating subtle foreground parallax.
- **Focus:** begins on the window-side environment, then racks once to the glass.
- **End:** tighter hero composition with the drink sharp on the right third and the cabin softly layered behind.
- **Risk:** moderate; requires compatible start/end geometry and a clean focus landing.

### Option B — Static observational frame

- **Audience effect:** composed, restrained, and quietly observational.
- **Start/end:** locked close composition; only condensation and distant cabin light move.
- **Focus:** fixed on the glass.
- **Risk:** low, but less sense of discovery.

### Option C — Gentle orbit around the glass

- **Audience effect:** more overt product heroism and dimensionality.
- **Movement:** short arc around the drink while holding its size.
- **Focus:** remains on the glass.
- **Risk:** higher; reflections and table/window geometry may drift.

User selects Option A.

## 4. Reference-image and Magnific node check

The agent offers to use the available image, leave it unused, or review it first. The user chooses to use it only for cabin materials, warm practical-light restraint, and overall production polish—not for composition, people, or exact cabin geometry.

The agent asks for the exact node name shown in Magnific. The user copies it as `CabinMood_01`. The binding is recorded as:

- **Reference:** cabin-material image
- **Exact Magnific node:** `CabinMood_01`
- **Prompt binding:** `@CabinMood_01`
- **Controls:** material restraint, practical-light character, production polish
- **Must not control:** composition, passenger identity, cabin geometry, or brand-color placement

Only after the exact node name is resolved does the workflow continue.

## 5. Static Prompt Readiness Summary

Before writing prompts, the agent consolidates the approved shot:

- **Purpose/beat:** reveal a refined service detail through quiet discovery.
- **Subject/action:** welcome drink remains physically stable beside the aircraft window.
- **Composition:** layered medium-close start resolving into a tighter right-third product hero.
- **Camera:** seated eye level, natural restrained perspective, diagonal forward and camera-right movement concept.
- **Lens/focus:** fixed focal-length behavior; shallow but controlled depth; environment-to-glass focus transition planned for video.
- **Lighting/design:** cool twilight outside, warm motivated cabin practical, dark stone, brushed metal, clear glass, restrained cabin textiles.
- **Brand color:** fictional `#C86A3A` used sparingly in upholstery piping and one service detail; no global orange wash and no contamination of skin or exterior twilight.
- **Occupancy:** other seated passengers and subtle service life remain visible in layered soft focus; the cabin is not empty, but the drink keeps clear visual priority.
- **Start/end:** separate end image required to control final product framing and focus destination; its copy-ready prompt is deferred until the approved start image has an exact Magnific node name.
- **Reference binding:** use `@CabinMood_01` for cabin materials and practical-light restraint only; do not inherit its composition, people, or geometry.
- **Continuity:** lock cabin geometry, window, table, glass, liquid level, materials, palette, and light direction.
- **Target/risk:** image generation first; reflections, glass geometry, condensation, and start/end spatial compatibility require attention.
- **Unresolved conflicts:** none.

The agent asks:

> Approve this specification and authorize the start-image prompt for this shot? The dependent end-image prompt will return for a compact binding check after the start image is approved and named in Magnific.

It clearly offers: approve and proceed, request changes to named fields, authorize only part of a batch, or hold and revisit an earlier decision.

The user approves. Only then does the agent provide the following prompt.

## 6. Start-image prompt

```text
Use @CabinMood_01 only as a reference for restrained cabin materials, warm practical-light character, and production polish; do not copy its composition, people, cabin geometry, or brand-color placement. Create a photorealistic premium-travel campaign still inside a refined modern aircraft cabin at twilight. A clear welcome drink rests on a dark honed-stone side table beside an aircraft window, visible but not yet the dominant subject. Compose a layered medium-close frame from seated eye level, with the window and softly illuminated cabin material in the midground and the glass positioned slightly right of center. The cabin is operational and plausibly inhabited: a few other seated passengers and a subtle service presence remain naturally layered in the deeper background, partially occluded and softly defocused, with varied posture and no one looking at camera. Use a natural restrained perspective with believable proportions, shallow but not extreme depth of field, initial focus held on the window-side environment, and the glass slightly softer. Balance cool twilight from outside with a warm, motivated cabin practical, producing gentle highlight roll-off, controlled reflections, tactile stone, brushed metal, clear glass, and realistic condensation. Integrate the fictional rust-orange brand color `#C86A3A` only as restrained upholstery piping and one small service-detail accent; preserve natural skin tones, glass, stone, metal, and exterior twilight without an orange wash. Quiet confidence, private calm, refined service, no empty-showroom cabin, no cloned or perfectly spaced passengers, no flashy luxury clichés, no excessive bloom, no particles, no aggressive flare, no oversharpening, no text, no watermark.
```

## 7. Start approval and end-image binding

The user generates and approves the start image. In Magnific, its exact node name is `SH01_Start_Approved`.

The agent records `@SH01_Start_Approved` as the geometry, identity, occupancy, material, palette, and lighting reference for the end image. It then presents a compact readiness update and asks the user to authorize the end-image prompt. The user approves.

## 8. End-image prompt

```text
Use @CabinMood_01 only to preserve the approved material and practical-light restraint. Use @SH01_Start_Approved as the exact reference for cabin design, table geometry, window position, glass design, materials, palette, background occupancy, and lighting direction. Create the final frame of the same continuous shot by moving the viewpoint physically closer and slightly camera-right, preserving believable parallax, all object geometry, and the softly layered presence of the same background passengers. End in a tighter layered hero composition with the welcome drink sharp on the right third, realistic condensation and reflections clearly resolved, while the aircraft window, cabin materials, and inhabited background remain softly defocused behind it. Preserve the quiet, tactile, restrained premium mood and the limited `#C86A3A` accent placement. Do not change the glass, liquid level, table, window, passenger identities, lighting direction, color palette, or cabin design. No added or removed people, cloned extras, text, logo, flare, particles, excessive bloom, or global orange wash.
```

## 9. Static approval

The user generates and approves the end image, whose exact Magnific node name is `SH01_End_Approved`. The agent verifies that the geometry, lighting, focus endpoints, and proposed movement remain compatible.

## 10. Video Prompt Readiness Summary

The agent presents the final movement plan before writing the video prompt:

```text
Reference bindings: dedicated start-frame node SH01_Start_Approved; dedicated end-frame node SH01_End_Approved; no guessed @ aliases
Support: stabilized wheeled dolly
Start: medium-close seated-eye-level composition; focus on the window-side environment
Path: tracks diagonally forward and camera-right
Orientation: slight counter-pan left to keep the glass moving toward the right-third hero position
Lens operation: fixed focal length; no optical zoom
Framing evolution: environment-led composition becomes a tighter product-led composition with increasing foreground parallax
Focus: one measured rack from the window-side environment to the welcome drink, triggered after the move begins and landing during the final second
Timing: five seconds; gentle acceleration, measured travel, soft deceleration, brief final hold
End: drink sharp on the right third; cabin and window softly layered behind; camera settled
```

The agent asks:

> Approve this motion specification and authorize the final video prompt for this shot?

It clearly offers: approve and proceed, modify the movement/focus/timing, simplify the move, or return to static-frame repair.

The user approves. Only then does the agent provide the video prompt.

## 11. Video prompt

```text
One continuous five-second photorealistic shot using the approved start image as the opening frame and the approved end image as the precise landing frame. The camera moves on a stabilized dolly, tracking diagonally forward and camera-right at a slow measured pace while counter-panning slightly left to preserve the glass's path toward the right-third hero position. Keep a fixed focal length with natural perspective and increasing foreground parallax; do not use an optical zoom. Begin with focus held on the window-side cabin environment. After the dolly move is established, perform one deliberate, smooth rack focus from the environment to the welcome drink, landing during the final second and holding. Background passengers remain consistent and make only restrained independent micro-movements appropriate to a calm flight; no one looks at camera, disappears, duplicates, or draws focus. Condensation remains physically stable, the liquid barely responds to the movement, the limited `#C86A3A` accents stay fixed, and cabin light stays consistent. Decelerate gently and settle into the approved end composition for a brief clean hold. No cuts, no angle change, no random reframing, no focus hunting, no object morphing, and no changes to glass, table, window, people, materials, palette, or lighting direction.
```

## 12. Acceptance criteria

- The clip remains one uninterrupted camera take.
- The path is diagonally forward and camera-right, not a digital zoom.
- The rack focus occurs once and lands cleanly on the glass.
- The final frame closely matches the approved end image.
- Glass, liquid, reflections, table, window, and lighting remain stable.
- The cabin remains plausibly inhabited without cloned, disappearing, frozen, or attention-stealing background people.
- The `#C86A3A` accent remains restrained and does not become a global color cast.
- `@CabinMood_01` affects only the assigned material and lighting qualities; its composition, people, and geometry do not leak into the shot.
- The camera settles long enough to create an editable endpoint.
