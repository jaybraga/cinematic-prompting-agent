# Camera Movement Language

## Purpose

Use this reference for every video prompt. Its job is to translate what the user can visualize or physically perform into precise camera and focus instructions that a video model can follow.

Do not invent decorative movement. Clarify or infer the movement that best expresses the approved shot function and mood, present the interpretation clearly, and let the user redirect it.

## Pre-draft Per-Shot Direction Check

Run this before creating the first static prompt because camera intent determines the start frame, end frame, lens perspective, spatial layering, blocking, and focus plan.

Ask:

```text
How would you like to direct this shot?

1. Describe the camera/viewpoint idea in your own words, and I will develop and translate it.
2. Show me two or three options based on the approved mood and shot purpose.
3. Hybrid: I will provide part of the idea, and you will complete or refine it.
```

For a still-only shot, translate `camera direction` into viewpoint and composition choices without inventing motion.

For a video shot, provide the complete movement and focus choreography. When proposing options, vary the directorial effect—for example restrained observation, immersive discovery, controlled reveal, subjective tension, or energetic participation—not merely the movement label.

Each option should include start frame, path or viewpoint, framing evolution, focus, end frame, emotional effect, generation risk, and a recommendation. Do not draft start/end prompts until one direction is approved.

## First establish the shot's endpoints

Before naming a move, identify:

- start framing, camera height, angle, and subject position;
- end framing, camera height, angle, and subject position;
- primary subject action during the move;
- foreground, midground, and background relationships;
- initial and final focus targets;
- duration and emotional purpose of the movement.

The approved start and end images define composition endpoints. The movement description defines how the camera travels between them.

## Build the camera choreography from components

### 1. Support or platform

State the physical behavior when it affects the result:

- locked tripod or static head;
- slider or short linear move;
- wheeled dolly or track;
- stabilized gimbal or Steadicam-like follow;
- handheld with restrained or energetic operator movement;
- jib, crane, pedestal, or boom;
- drone, vehicle mount, cable, robotic arm, or virtual camera.

Avoid naming a support only for prestige. Describe the stability, inertia, and operator character it should create.

### 2. Translation through 3D space

- **Dolly/push in:** camera physically moves closer.
- **Dolly/pull back:** camera physically moves farther away.
- **Truck/track left or right:** camera moves laterally.
- **Pedestal/boom up or down:** camera rises or falls without tilting by definition.
- **Arc/orbit:** camera travels around the subject.
- **Crane/jib move:** camera combines vertical and horizontal travel along an arc.
- **Follow/lead:** camera maintains a relationship behind, beside, or ahead of a moving subject.

For diagonal movement, state both axes: `tracks forward and camera-right` or `pulls back while rising`.

### 3. Camera orientation

- **Pan:** rotates left or right from the camera's position.
- **Tilt:** rotates up or down.
- **Roll:** rotates around the lens axis.
- **Counter-pan/counter-tilt:** rotates while translating to hold or deliberately release composition.

State whether the camera keeps the subject framed, lets the subject drift, reveals another element, or changes the horizon.

### 4. Optical change

- **Zoom in/out:** changes focal length without moving the camera.
- **Dolly zoom:** physically dollies while zooming in the opposite direction, usually keeping the principal subject approximately the same size while perspective changes around it.
- **Lens breathing:** an optical side effect, not a substitute for a designed zoom.

If the user says `zoom` but describes physical travel, verify whether they mean a zoom, a dolly, or both. Never silently convert one into another when the difference changes perspective.

### 5. Framing evolution

Describe what the audience sees, not only the mechanism:

- wide to medium close-up;
- centered subject drifting to the right third;
- foreground object entering and becoming dominant;
- shoulder-level profile resolving into an over-the-shoulder frame;
- background reveal created by parallax;
- camera clears an occlusion and lands on the hero composition.

### 6. Focus choreography

Specify:

- initial focus target;
- destination focus target;
- cue that starts the pull;
- direction: foreground to background or background to foreground;
- speed and character: snap, quick, measured, slow, nearly imperceptible;
- when focus should land and whether it should hold;
- depth-of-field behavior and whether breathing should be minimized.

Use `rack focus` or `pull focus` only with named targets. Prevent random hunting by stating a single deliberate transition and final hold.

### 7. Timing, speed, and easing

Define:

- total clip duration;
- when the move begins;
- acceleration and deceleration;
- constant, accelerating, or decelerating travel;
- pauses, holds, or settles;
- synchronization with subject action, sound, reveal, or focus cue.

Use time ranges when they clarify a continuous shot. Do not over-segment a simple move.

### 8. Subject relationship and parallax

State whether the camera:

- maintains distance from a moving subject;
- overtakes or falls behind the subject;
- keeps subject size constant;
- crosses foreground elements for depth and parallax;
- reveals background geometry;
- preserves or intentionally changes screen direction.

### 9. Landing state

End with an exact visual instruction:

- final shot size and camera angle;
- subject position in frame;
- final focus target;
- whether the camera settles, stops cleanly, or continues drifting;
- any required hold for use in the final edit.

## Clarify ambiguous terminology

Ask a concise question when different interpretations would create materially different shots. Common ambiguities include:

- `zoom in` versus physical push-in;
- `move right` meaning camera-right, subject-right, or composition drifting right;
- `orbit` versus lateral tracking with a pan;
- `dolly zoom` versus dolly plus ordinary zoom in the same direction;
- `focus on the foreground` meaning start there, rack there, or merely use shallow depth.

If the likely interpretation is clear and low risk, state it as an assumption and proceed.

## Camera Movement Breakdown format

Before the copy-ready prompt, use this compact verification block when movement is more than a static frame:

```text
CAMERA MOVEMENT BREAKDOWN
Support: [platform and stability]
Start: [framing, height, angle, subject position, focus]
Path: [translation through space]
Orientation: [pan, tilt, roll, subject hold/release]
Lens operation: [fixed focal length or zoom behavior]
Framing evolution: [visible compositional change]
Focus: [target A -> target B, cue, speed, landing]
Timing: [duration, acceleration/easing, holds]
End: [final framing, subject position, focus, settle/hold]
```

Omit fields that are genuinely irrelevant, but do not omit a field merely because it is difficult to describe.

## Copy-ready prompt sentence pattern

```text
One continuous [duration]-second shot on [support]. Start [start composition and focus]. The camera [3D path] [speed/easing] while [orientation behavior] to [framing purpose]. [Lens operation, if any]. As [action/cue], perform one [focus-pull character] rack focus from [target A] to [target B], landing by [time or visual beat] and holding. End [final composition, focus, and settle]. No cuts, no reframing jumps, no random focus hunting.
```

Adapt the prose naturally to the shot and target model; do not leave bracketed template language in a final prompt.

## Example: diagonal push with foreground focus pull

If the intended move is a physical push rather than a true dolly zoom:

```text
One continuous six-second shot on a stabilized dolly. Start in a medium-wide frame with the principal subject on the left third and focus held on the subject. The camera tracks diagonally forward and camera-right at a measured pace, counter-panning slightly left to keep the subject framed while foreground geometry creates increasing parallax. As the foreground object clears into the right side of frame, perform one deliberate rack focus from the principal subject to that foreground object, landing during the final second and holding. End in a tighter layered composition with the foreground object sharp, the principal subject softly defocused behind it, and the camera settling cleanly. No cuts and no focus hunting.
```

If the user intends a true dolly-zoom effect, state the opposing optical operation:

```text
One continuous six-second stabilized dolly-zoom. The camera tracks diagonally forward and camera-right while the lens zooms out at a matched rate, keeping the principal subject approximately the same size as the background perspective expands. Counter-pan gently to preserve the subject on the left third. On the foreground object's entrance, execute one measured rack focus from the principal subject to the foreground object, land during the final second, and hold. End with the foreground element sharp, the subject softly defocused, and the camera settled. No cuts, no framing jumps, and no random focus hunting.
```

These are different effects. Confirm which one the user intends before finalizing the prompt when the wording is ambiguous.
