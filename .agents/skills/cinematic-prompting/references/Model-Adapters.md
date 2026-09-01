# Model Adapters

## Purpose

Use this file only after the canonical static or motion specification is approved. It compiles approved intent into target-model language without changing locked decisions.

Read `Model-and-Prompt-Strategy.md` first to select the model, prompt form, reference plan, and escalation path. Model and Magnific capabilities change; verify the live model name, mode, reference limits, duration, aspect ratio, resolution, audio, start/end-frame support, and credit consequence before final delivery.

## Shared compiler rules

- Preserve the canonical subject, mood, composition, continuity, and camera logic.
- Use the prompt form approved in the Model & Prompt Strategy Card.
- Prefer natural, concrete language over tag piles.
- Assign each reference one job and priority; state unwanted traits that must not transfer.
- Put actual settings in the Magnific settings card, not in JSON-shaped prompt text.
- Use avoidance instructions only when they improve control.
- Keep explanatory notes and citations outside copy-ready prompts.
- Default Magnific prompt enhancement to off for approved production prompts. If testing it, compare against the canonical specification and reject drift.

## Magnific orchestration

For every package specify the selected model and exact mode, start/end assignments, additional references and roles, aspect ratio, resolution, duration and audio controls, relevant live options, known credit consequence, and whether prompt enhancement is off.

Follow `Magnific-Reference-Node-Bindings.md`. Preserve exact confirmed node names in `@` references. If the mode uses a dedicated slot, list the assignment in the settings card without redundant prompt syntax.

## Seedream 5 Pro — static generation and editing

Use for new cinematic keyframes, environments, lifestyle imagery, controlled spatial composition, lighting/material exploration, and brand-aware art direction.

Default prompt order:

1. intended image and moment;
2. identities and spatial relationships;
3. composition and camera position;
4. lighting, palette, materials, and production design;
5. performance and small physical details;
6. reference assignments and exclusions;
7. preservation requirements for edits.

Use labeled natural prose by default. Use object-by-object structure only when a dense layout benefits from it. For revisions, make the smallest requested change and state what must remain unchanged.

## Nano Banana Pro — static generation and editing

Use for professional precision edits, reference fusion, branded compositions, product/character continuity, typography, localization, aircraft/uniform fidelity, and controlled placement.

- Prefer `CHANGE`, `PRESERVE EXACTLY`, and `REFERENCE JOBS` blocks for edits.
- Use positive, direct instructions and explicit spatial relationships.
- Quote required on-image copy and specify placement and hierarchy.
- Validate text, logos, product geometry, hands, and fine brand details visually.
- Move compliance-critical marks to post when generation cannot reproduce them reliably.

## Nano Banana 2 — static exploration and economical edits

Use for rapid ideation, variants, simpler edits, background extensions, and exploratory start/end frames.

- Keep prompts concise.
- Use it to answer composition or concept questions before spending on a precision pass.
- Escalate to Nano Banana Pro for fine identity, typography, product geometry, or complex multi-reference control.
- Consider Seedream 5 Pro when environmental rendering and cinematic interpretation matter more than edit precision.

## Kling 3.0 / 3.0 Omni — single-shot video

Prefer image-to-video or compatible start/end frames from approved stills.

- Use concise motion prose: one primary action, one camera intention, focus behavior, secondary environmental motion, and landing.
- Keep native multi-shot/custom storyboard mode off unless explicitly requested.
- Do not repeat static appearance already controlled by the frame.
- Do not use prompt text to overcome geometrically incompatible endpoints.
- If motion feels robotic or patterns drift, simplify tracking, reduce simultaneous motion, repair an endpoint, or split coverage.

## Seedance 2.5 — complex single-shot video

Reserve for continuity-heavy movement, difficult physical interactions, sequential beats, or premium attempts justified by approved stills and a clear risk hypothesis.

Build around one continuous shot, the start state, primary performance, coherent camera choreography, focus behavior, physical/environmental response, and landing. Use time ranges only for genuine sequential beats that remain one take.

Before generation, recheck endpoint compatibility and disclose the known credit consequence or uncertainty. Do not use Seedance to solve a static-design or reference problem.

## Fallback order

Preserve creative intent and try the smallest intervention first:

1. remove contradiction or simplify the prompt;
2. repair, replace, or re-role a reference;
3. reduce simultaneous action or camera complexity;
4. create a stronger compatible endpoint;
5. split coverage into additional single-shot clips;
6. switch prompt form, mode, or model;
7. use a localized edit or post-production composite.

After two materially similar failures, stop appending constraints and return to `Model-and-Prompt-Strategy.md`.
