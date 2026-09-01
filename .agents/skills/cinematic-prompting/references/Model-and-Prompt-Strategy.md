# Model and Prompt Strategy

## Purpose

Use this guide during every Per-Shot Direction Check, again before prompt authorization, and whenever a shot pivots, fails, or expands into alternatives. It selects the model, prompt form, and reference strategy before prose accumulates.

Model behavior, Magnific availability, modes, reference limits, and credit prices change. Treat the tendencies below as routing guidance, verify consequential live settings, and distinguish verified platform facts from observed workflow tendencies.

## Recommend before asking

Do not ask only `Which model do you want?` or `Natural prompt or JSON?`

For every shot, first recommend a primary model and prompt form, explain the visible benefit and principal risk, name a practical fallback, then ask the user to approve or override. If the user already chose a model, respect it while flagging material limitations and a fallback.

Use this compact card:

```text
MODEL & PROMPT STRATEGY — [shot ID]
Primary: [model + mode] — [why it fits this shot]
Fallback: [model + mode] — [when to pivot]
Prompt form: [form] — [why]
Reference plan: [node/slot -> one assigned job each]
Iteration plan: [cheap exploration, precision pass, or direct production]
Main risks: [top two or three]
Stop status: clear / blocked by [check]
Decision: approve, choose fallback, or redirect.
```

For batch planning, use a compact table, but call out hero shots, branded assets, geographic fidelity, and difficult motion individually.

## Prompt forms

### 1. Labeled natural prose — default

Use short paragraphs with explicit labels or a clear order: moment, subjects and spatial relationships, composition/camera, light and design, reference jobs, and preservation rules. This is the default for cinematic lifestyle, portrait, architecture, travel, hospitality, and most image-to-video work.

This is not vague prose. Use concrete spatial and physical language, and keep explanation outside the copy-ready prompt.

### 2. Change / Preserve / Reference — precision edits

Use for revisions to an approved image:

```text
CHANGE
[small requested change]

PRESERVE EXACTLY
[composition, identity, geometry, light, wardrobe, background, crop]

REFERENCE JOBS
@[node] controls only [role]
```

Prefer this over rewriting the entire shot. If the edit changes composition, camera side, or scene logic, treat it as a new shot or controlled variant rather than pretending it is local.

### 3. Object-by-object structured prompt — complex layouts

Use labeled blocks or JSON-like structure for flat lays, menus, product grids, several precisely placed props, or commercial layouts where each object needs its own position, material, and color. JSON-shaped text is an organization aid, not a different generation API.

Do not use JSON merely because it looks technical. Natural prose is usually better for atmosphere, candid human behavior, and cinematography. Never confuse JSON text pasted into a prompt node with actual structured API fields such as start image, end image, duration, resolution, seed, or reference slots.

### 4. Shared master plus shot delta — match-cut families

Use for paired locations, campaign variants, or several shots that must share composition. Keep one approved master specification, then list only the controlled differences for each shot. Do not duplicate and independently mutate long prompts.

### 5. Concise motion prompt — image-to-video

Let approved frames carry appearance. Prompt the change: primary action, camera behavior, focus, environmental response, pace, and landing. Use timed beats only when a continuous shot truly contains sequential actions. Do not redescribe every static detail or ask prose to repair incompatible endpoints.

## Current model routing

### Seedream 5 Pro

Best first choice for creating new cinematic stills, environments, travel/lifestyle imagery, lighting/material exploration, and composed keyframes where the image needs room to interpret art direction.

- Preferred prompt form: labeled natural prose.
- Use object-by-object structure for dense tabletop or multi-object layouts.
- For edits, isolate the change and preservation requirements.
- Watch for: over-instruction, geographic invention, exact typography/logo distortion, and reference-role blending.
- Typical pivot: Nano Banana Pro when reference fusion, brand/product precision, or a localized edit matters more than generative interpretation.

### Nano Banana Pro

Best for high-control still editing, reference fusion, branded products, uniforms, aircraft, character continuity, typography, localization, and precise placement or preservation.

- Preferred prompt form: direct natural language with `CHANGE`, `PRESERVE EXACTLY`, and explicit reference roles.
- Use for a precision pass after composition is approved elsewhere.
- Watch for: unnecessary rebuilding when a local edit would do, overloaded reference stacks, and assuming an AI-rendered logo is compliance-ready.
- Typical pivot: compositing/post for exact logos, legal marks, liveries, or colorimetry that must survive close inspection.

### Nano Banana 2

Best as a fast, economical generalist for ideation, variants, simpler edits, background extensions, start/end-frame exploration, and tests where the risk of a failed pass is low.

- Preferred prompt form: concise natural prose or a short change/preserve block.
- Use before Pro when the task is exploratory rather than compliance-critical.
- Watch for: fine identity, typography, product geometry, or multi-reference precision limits.
- Typical pivot: Nano Banana Pro for the approved precision pass; Seedream 5 Pro when cinematic rendering and environmental invention are the priority.

### Kling 3.0 / 3.0 Omni

Best for short image-to-video shots with approved frames, one readable subject action, and one coherent camera move. It often benefits from giving the model a clear physical intention without micromanaging every instant.

- Preferred prompt form: concise motion prose: subject action, camera behavior, focus, environmental motion, and landing.
- Use start/end frames only when their geometry can connect naturally.
- Watch for: temporal texture noise, pattern drift, robotic tracking, conflicting screen direction, and prompts that repeat static appearance.
- Typical pivot: simplify the move, strengthen one endpoint, split the coverage, or use Seedance 2.5 for unusually demanding continuity.

### Seedance 2.5

Best reserved for difficult continuous motion, complex physical continuity, sequential beats, or shots where reference adherence and temporal reasoning justify the higher credit cost.

- Preferred prompt form: production-note prose; use restrained time ranges only for genuine sequential beats inside one uninterrupted shot.
- Confirm compatible start/end frames before spending credits.
- Watch for: expensive experimentation, excess instructions, and using a premium video model to solve a static-design problem.
- Typical pivot: return to static repair, simplify coverage, or test the motion in Kling before another premium pass.

## Reference strategy

Give each reference one explicit job and priority:

- identity, product, uniform, logo, or livery;
- composition, crop, pose, or camera angle;
- location, geography, or architecture;
- lighting, palette, texture, or color grade;
- movement, timing, or performance.

Use the fewest references needed. State traits that must not transfer. A composition reference must not silently become a lighting reference; a low-quality geography reference must not become a texture source.

For branded color, combine the hex code with a color name, intended material/surface, approximate frame coverage, and lighting behavior. Treat the hex as a design target rather than guaranteed rendered colorimetry. Recommend grading, masks, or compositing when exact compliance matters.

## Mandatory stop checks

Stop prompt drafting or generation and surface the blocker when any condition applies:

1. **No strategy decision:** the model, mode, and prompt form have not been recommended and accepted, or consequential live availability/cost is unverified.
2. **Format without purpose:** JSON-shaped text is being used without a layout/control benefit, or actual settings are being buried inside pseudo-JSON instead of the proper interface fields.
3. **Reference conflict:** two references compete for composition, identity, geography, lighting, or motion; a reference lacks an assigned job; or the stack is larger than necessary.
4. **Brand asset risk:** a compliance-critical logo, livery, uniform, product, menu, or typography lacks an authoritative reference, fidelity tolerance, or post-production plan.
5. **Brand color ambiguity:** an exact hex is requested without an intended surface, prominence, material response, or lighting behavior.
6. **Geographic fidelity risk:** the shot implies accurate geography or architecture without an authoritative reference or an explicitly approved tolerance for approximation.
7. **Incompatible video endpoints:** start and end frames disagree on camera side, horizon, scale, lens perspective, geometry, light direction, identity, pose path, or screen direction. Do not try to prompt through the mismatch.
8. **Premature expensive generation:** a premium model is about to be used before cheaper concept tests, static approvals, or endpoint checks have answered the uncertain questions.
9. **Unapproved pivot:** a new idea changes a locked field, shot function, model strategy, or reference role without refreshing the strategy card and readiness summary.
10. **Prompt bloat or contradiction:** accumulated revisions contain redundant, opposing, or over-specific instructions. Reset from the last approved canonical specification.

The stop is diagnostic, not bureaucratic. State the exact conflict, recommend the smallest resolution, and offer the user a clear choice.

## Iteration and pivot protocol

Before revising, classify the failure:

- concept or shot function;
- composition/camera;
- identity, product, or brand fidelity;
- geography/architecture;
- lighting, grade, or optical character;
- anatomy, pose, or human behavior;
- motion, physics, or temporal consistency;
- model or mode limitation.

Then:

1. Preserve every approved dimension that is already working.
2. Change the smallest failing dimension.
3. Explain whether the same model/prompt form remains best or whether the failure justifies a pivot.
4. Refresh the Model & Prompt Strategy Card whenever the concept, model, prompt form, reference plan, endpoints, or cost tier changes.
5. After two materially similar failures, or as soon as the prompt becomes contradictory, stop stacking instructions. Rebuild concisely from the canonical specification, repair/create a better reference, change the model, split the shot, or move an exact element to post.

When exploring alternatives, distinguish a controlled variant from a repair. A variant may change approved creative variables; a repair should not.
