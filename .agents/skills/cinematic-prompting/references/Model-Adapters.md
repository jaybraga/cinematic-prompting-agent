# Model Adapters

## Purpose

Use this file only after the canonical static or motion specification is approved. It translates creative intent into target-model language without changing locked decisions.

Model and Magnific capabilities change. Verify the live model name, mode, reference limits, duration, aspect ratio, resolution, audio, start/end-frame, and other controls before final delivery.

## Shared compiler rules

- Preserve the canonical shot's subject, mood, composition, continuity, and camera logic.
- Use natural, concrete language instead of tag piles.
- Preserve the full approved camera choreography; simplify wording for the model without deleting path, framing, focus, timing, or landing requirements.
- Assign each reference a role and priority.
- Put settings in a separate Magnific settings card rather than burying them in prose.
- Use avoidance or negative instructions only when the selected model supports them and they improve control.
- Keep explanatory notes and citations outside copy-ready prompts.

## Magnific orchestration

For every prompt package specify:

- selected model and exact mode;
- start image and end image assignments;
- additional references and their roles;
- aspect ratio, resolution, duration, and audio controls;
- any relevant model-specific sliders or options visible in the current interface;
- whether Magnific prompt enhancement should remain off.

Before compiling a selected image reference into a Magnific prompt, follow `Magnific-Reference-Node-Bindings.md`. Use the exact confirmed node name in each `@` reference. If the active Magnific mode uses a dedicated reference slot instead, list the exact node assignment in the settings card without adding unsupported or redundant prompt syntax.

Default prompt enhancement to off for approved production prompts. If testing it, compare the enhanced version against the canonical specification and reject changes to locked fields.

## Seedream 5.0 Pro — static generation and editing

Use for complex keyframes, spatial composition, reference-driven design, product/brand work, and controlled edits.

Prompt order:

1. intended image and moment;
2. subject identities and spatial relationships;
3. composition and camera position;
4. lighting, palette, materials, and production design;
5. performance and small physical details;
6. reference assignments;
7. exact preservation requirements for edits.

For revisions, describe the smallest requested change and explicitly state what must remain unchanged. Prefer iterative edits over rebuilding an approved frame.

## Nano Banana Pro — static generation and editing

Use for complex professional stills, branded compositions, product integration, typography, localization, and conversational refinement.

- Use positive, direct instructions and explicit spatial relationships.
- For edits, distinguish `change` from `preserve exactly`.
- Quote required on-image copy and specify placement, hierarchy, and typographic character.
- Validate text, logos, product geometry, hands, and fine brand details visually.
- When multiple references are used, state the relationship between them rather than listing them.

## Seedance 2.5 — single-shot video

Use after the start image, and preferably the end image when the landing state matters, have been approved.

Build the prompt around:

1. one continuous shot and intended duration;
2. starting state already established by the start image;
3. one primary performance/action beat;
4. one coherent camera choreography, including support, spatial path, orientation, lens operation, and framing evolution as applicable;
5. focus targets, direction, cue, duration, and landing point when a focus pull is required;
6. secondary environmental motion and physical response;
7. ending state or end-image landing;
8. audio behavior when relevant and supported.

Use time ranges only when a single shot contains sequential action beats that remain physically continuous. Do not ask Seedance to cut to another setup.

## Kling 3.0 / 3.0 Omni — single-shot video

Prefer image-to-video or start/end-frame generation from approved stills.

- Keep native multi-shot/custom storyboard mode off by default.
- Use one continuous setup, one primary action, and one coherent camera choreography.
- Bind character, product, location, motion, or voice references by purpose.
- Use a start/end pair when the final pose, framing, reveal, transformation, or transition must be controlled.
- If the desired move cannot plausibly connect the two frames, redesign the frames or split the coverage into separate shot IDs.

Only use Kling multi-shot when the user explicitly requests baked-in cuts for a particular experiment.

## Fallback order

When a model fails, preserve approved creative intent and try the smallest intervention first:

1. simplify or clarify the prompt;
2. repair or replace a reference image;
3. reduce simultaneous action or camera complexity;
4. create a stronger end frame;
5. split coverage into additional single-shot clips;
6. switch generation mode or model;
7. solve the remaining issue with a localized edit or post-production composite.
