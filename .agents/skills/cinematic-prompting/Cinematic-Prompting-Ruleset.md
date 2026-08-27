# Cinematic Prompting Ruleset

## Purpose of this file

This file contains the non-negotiable production and prompt-design rules. It does not define conversational style or repeat the chronological workflow.

## 1. Still-first video production

Every video shot must begin with a static version of that exact shot.

- Create and approve a start image before writing the final video prompt.
- Create a separate end image whenever the end composition, pose, product framing, transformation, reveal, focus destination, or transition must land precisely.
- When the end image will use the generated start image as a Magnific reference, approve the start image and obtain its exact Magnific node name before writing the copy-ready end-image prompt. Do not prewrite the end prompt with a guessed or placeholder node.
- Use the approved stills as visual truth for identity, composition, production design, lighting, palette, texture, and spatial relationships.
- Do not bypass this stage because a video model supports text-to-video.
- If the user explicitly changes this rule for a particular experiment, record the exception in that shot's notes.

## 2. One continuous camera shot per generated clip

- Each video prompt describes one uninterrupted camera take with no internal cut to another angle or setup.
- Do not use native multi-shot generation, automatic shot changes, or several camera setups inside one file unless the user explicitly requests it.
- Build coverage as separate clips and leave shot order, cutting, transitions, timing, and rhythm to post-production.
- A continuous camera move may change framing within a shot, but it must remain one physically coherent take.

## 3. Mood and style approval gate

- Do not build production prompts until the piece's mood, emotional promise, visual style, and anti-goals are explicit enough to direct the work.
- If those decisions are missing, propose creative lanes and obtain approval.
- Define style through visible choices: palette, lighting logic, contrast, production design, performance, composition, optics, texture, grade, movement, and pacing.
- Store the approved base direction in the production bible.
- Record scene-specific or sequence-specific departures as intentional overrides rather than weakening the base direction.

## 4. Brand-palette intake and controlled integration

- At the beginning of every new project, explicitly ask whether a particular brand hex code or defined palette should be incorporated in the imagery.
- Offer three clear paths: supply exact hex code(s) and priorities; derive a palette from supplied guidelines or references; or use no locked brand color.
- Record each approved code in the production bible with its intended role, priority, and exclusions. Suitable roles can include wardrobe accents, props, set dressing, signage, practical light, interface elements, product details, or selective grade relationships.
- Do not interpret a brand color as permission to apply a global wash, recolor every object, contaminate believable skin tones, or erase the natural color identity of a location.
- Use exact hex values as design targets, not a promise that a generative model will reproduce colorimetry perfectly. When exact compliance matters, recommend controlled grading, masks, compositing, or a measured finishing pass.
- Preserve color hierarchy. The brand color may be a hero accent, supporting rhythm, or environmental echo; it does not need to dominate every frame.

## 5. Research before inventing missing shots

- When the user lacks a usable shot list or requests visual discovery, research what is relevant to show before drafting shots or prompts.
- Define the research mandate from the communication objective, audience, approved direction, factual/cultural scope, required proof, and production constraints.
- Separate verified facts, source-backed observations, and creative hypotheses. Never turn an assumption into a campaign claim.
- Prefer authoritative and primary sources for route, product, geographic, historical, cultural, and current operational facts.
- Evaluate candidate motifs for strategic relevance, visual potential, narrative role, brand fit, feasibility, and stereotype or sensitivity risk.
- When useful, propose two or three distinct narrative routes and obtain approval before converting the selected route into a proposed shot list.
- Obtain approval of the proposed shot list before production prompts. Skip this stage when supplied visuals are already sufficient unless the user requests enrichment or verification.

## 6. Per-Shot Direction Check before drafting

- Do not write the first static prompt for a shot until its viewpoint and camera intention have been checked.
- For every still image, confirm or propose framing, camera height, angle, lens/perspective behavior, subject placement, depth, and focus plane.
- For every video shot, also confirm or propose camera support, movement path, orientation, lens operation, framing evolution, focus choreography, timing, and end state.
- Give the user three interaction paths: user-described direction, two or three agent-proposed options, or a hybrid of both.
- Agent-proposed options must differ in emotional and narrative effect, not merely in terminology.
- Recommend one option and explain its visible benefit and generation risk.
- Obtain approval before building start/end-frame prompts.

## 7. Mandatory Prompt Authorization Gate

- Copy-ready image and video prompt drafting is locked by default.
- Before the first static prompt for a shot, all material fields must be decided or surfaced as explicit defaults: purpose, subject/action, shot size, composition, camera position/height/angle, lens and perspective behavior, aspect ratio, production design, lighting, palette and assigned brand-color use, lived-in occupancy/background activity or an approved emptiness exception, depth of field, focus, start state, end state and end-image decision, continuity, reference-use decisions and bindings, target model/mode, and generation constraints.
- For video shots, also decide support/stability, three-dimensional path, orientation, lens operation, framing evolution, focus choreography, timing/easing, subject/environmental motion, landing frame, and continuity risks.
- Present these decisions as a concise Prompt Readiness Summary. Clearly label any remaining assumption, recommended default, unresolved conflict, or high-risk instruction.
- Ask the user to approve the specification and authorize prompt drafting. Do not infer authorization from earlier approval of mood, research, a narrative route, a shot list, or one camera option.
- An unambiguous affirmative response is sufficient; do not require a password-like phrase.
- Authorization may cover one shot, a named batch, all ready static prompts, or all ready video prompts. Do not extend it beyond the stated scope or across prompts whose selected reference bindings do not yet exist.
- Static-prompt authorization does not automatically authorize final video prompts. After the actual start/end images are approved, reconfirm affected motion decisions and obtain video-prompt authorization.
- A direct request to revise an existing prompt authorizes only that requested revision, provided it does not introduce unresolved conflicts with locked decisions.

## 8. Canonical intent before model syntax

- Maintain a model-neutral production bible and canonical specification for every shot.
- Treat model prompts as compiled outputs, not the source of creative truth.
- Never silently change an approved subject, product, wardrobe, location, mood, camera rule, or continuity state to accommodate a model.
- If a model cannot reliably execute the specification, recommend a different mode, reference strategy, shot design, model, or post-production solution.

## 9. Locked invariants and controlled variables

For campaigns and sequences, explicitly separate:

- **Locked invariants:** identity, product geometry, label or logo, wardrobe, hero props, location geography, time-of-day logic, base palette, brand rules, and approved optical language.
- **Controlled variables:** shot size, angle, focal-length tendency, performance beat, camera movement, focus behavior, weather, dirt, damage, intensity, and story-driven state changes.

Only accepted, intentional changes may update the continuity state. Never propagate accidental generation drift into later prompts.

## 10. Image prompts describe a state; video prompts describe change

Static prompts prioritize:

- subject and moment;
- composition and spatial relationships;
- pose and expression;
- camera position, framing, and lens behavior;
- lighting and production design;
- material, texture, palette, atmosphere, and visual hierarchy.

Video prompts prioritize:

- start state established by the approved image;
- one primary subject action;
- one physically coherent camera behavior;
- deliberate focus behavior when needed;
- environmental motion and secondary action;
- pacing and performance;
- end state, especially when an end image is supplied;
- audio behavior only when relevant and supported.

Do not unnecessarily redescribe or destabilize visual information already locked by the input images.

## 11. Camera language must have a visible purpose

- Camera and lens names are shorthand, not substitutes for direction.
- Translate references such as ARRI, RED, Fujifilm, anamorphic, spherical, vintage glass, or film stock into the characteristics that matter: format feel, perspective, focal length, distance, depth of field, focus falloff, flare, distortion, highlight behavior, color, contrast, grain, halation, frame rate, shutter, and motion blur.
- Include only parameters that create a visible or narrative consequence.
- Define one coherent camera choreography per clip. It may combine a spatial move, pan/tilt/orbit correction, optical zoom, and focus pull when those operations belong to the same continuous intention.
- Specify camera support, 3D path, orientation, framing evolution, lens operation, focus targets and timing, speed/easing, subject relationship, and landing state whenever they matter.
- Distinguish camera movement from optical zoom and focus movement. Never use "dolly zoom" as a generic synonym for pushing in.
- Use unambiguous spatial language such as `camera-right`, `subject-right`, or `toward the right side of frame`.
- Avoid stacks of unrelated moves that would require several camera setups or create contradictory motion.
- Preserve plausible screen direction, eyelines, geography, contact, shadow direction, reflections, and physical causality.

## 12. References must have assigned jobs

- Label what each reference controls: identity, wardrobe, product, location, composition, pose, lighting, palette, texture, camera movement, performance, or sound.
- Before prompt authorization, explicitly check whether a usable reference image is available for the shot or batch. Offer three paths: use it; leave it unused; or review it before deciding.
- If the user chooses to use an image through a Magnific prompt reference, obtain the exact node name shown in Magnific before writing the copy-ready prompt. Do not infer a node name from the filename, upload title, content, or earlier project label.
- Preserve the supplied node name exactly, including spelling, capitalization, spaces, punctuation, and numbering, and use that confirmed name in the corresponding `@` mention or interface-recognized node token.
- For multiple references, record one exact node name, assigned role, and priority per image. Resolve conflicting jobs before prompting.
- If an image has not yet been uploaded or its node has not been named, keep the binding unresolved and prompt drafting locked for that shot unless the user explicitly chooses to proceed without the reference.
- If Magnific binds a start image, end image, or other reference through a dedicated setting rather than an `@` prompt mention, record the exact node in the settings card and do not invent redundant prompt syntax.
- Do not attach a pile of references without explaining their relationships or priority.
- When references conflict, resolve the conflict before prompting.
- Use accepted start and end images ahead of verbal re-description whenever exact framing or continuity matters.

## 13. Lived-in world and plausible occupancy

- Unless the user explicitly directs otherwise, environments should feel inhabited, operational, and socially plausible rather than staged, abandoned, or reserved exclusively for the main character.
- Public, commercial, travel, hospitality, workplace, leisure, and social spaces normally include context-appropriate secondary people and activity. A Rio beachfront promenade should reflect believable pedestrian, beach, kiosk, traffic, and service life; a functioning restaurant should normally contain other patrons and staff.
- Match population density and behavior to the real place, time, weather, culture, and narrative. `Lived-in` does not mean maximum crowd density, uncontrolled clutter, or forcing visible faces into every frame.
- Build depth with varied background roles, actions, spacing, scale, occlusion, and focus. Keep the main subject and visual hierarchy clear while allowing the world to continue around them.
- Avoid duplicated extras, repeated faces or wardrobe, perfectly spaced groups, synchronized gestures, frozen crowds, generic stock poses, and background people who stare at the camera or steal the narrative beat.
- For video, give secondary people restrained, independent, physically plausible actions that support the scene without creating unnecessary temporal instability.
- Treat an empty, closed, private, evacuated, after-hours, surreal, or intentionally isolated environment as a deliberate exception. Record and approve the reason instead of allowing a model to empty the location by default.

## 14. Anti-AI-look standard

Reject or repair outputs with:

- waxy skin, glassy eyes, or over-retouched faces;
- uniform micro-detail, oversharpening, or edge halos;
- no focus, exposure, or visual hierarchy;
- gratuitous teal-orange grading, neon saturation, bokeh, fog, particles, flare, bloom, or chromatic aberration;
- impossible reflections, shadows, contact, scale, topology, or material response;
- mutated typography, logos, packaging, controls, seams, jewelry, hands, or product geometry;
- sterile symmetry or generic production design;
- implausibly empty public or social locations, background extras that look cloned or arranged, and spaces that feel closed solely because the model omitted normal human activity;
- temporal morphing, sliding contact points, liquid cloth, unstable hands, random focus hunting, or continuity drift.

Treat optical imperfection as a controlled system. Prefer a coherent clean master and add strong grain, halation, aberration, or distressed texture in finishing when practical.

## 15. Research and current capabilities

- Research only when it improves current model accuracy, technical accuracy, cultural or historical authenticity, location/product fidelity, or reference analysis.
- For research-to-shotlist work, preserve sources, uncertainty, cultural considerations, and the reason each finding matters to the piece.
- Keep sources and reasoning outside copy-ready prompts.
- Verify the current Magnific model, mode, aspect ratio, duration, reference, and control options before asserting that a setting is available.
- Do not blindly use automatic prompt enhancement if it might alter approved creative or continuity decisions.

## 16. Optional connected-history validation and credit safety

- Do not make Magnific MCP or any other connector a required part of the workflow. Detect only capabilities actually available in the current platform and preserve a manual upload/link path.
- When output review is due and read-only Magnific history access is available, offer it as an explicit user choice. Do not search account history automatically.
- History search, creation lookup, metadata reading, and preview/full-resolution retrieval must remain read-only. They may be used to validate a selected output against the approved shot specification and do not authorize any media mutation.
- Never generate, edit, transform, vary, upscale, relight, or create video as an implicit follow-up to validation. Explain the operation and its known credit consequence, then obtain separate explicit authorization for that exact action.
- Do not assume an account's unlimited plan applies through a connector. If a connector reports balance, cost, or unlimited-session limitations, disclose the relevant information before any paid action.
- Treat connector metadata as a retrieval aid, not creative truth. Only accepted intentional visual results may update continuity or become approved start/end frames.

## 17. Approval and version integrity

- For campaigns, sequences, and scripts, obtain approval of the creative treatment and production bible before shot prompting.
- When Shot Research is used, obtain approval of the narrative route and proposed shot list before production-bible and shot-prompt development.
- Obtain approval of the Per-Shot Direction Check before the first static prompt for that shot.
- Obtain explicit Prompt Authorization after presenting the completed shot specification; prior approvals do not substitute for it.
- Obtain approval of static start/end frames before final video prompting.
- Identify every shot and prompt version.
- Preserve previous approved versions when revising.
- Save prompts, settings, references, acceptance criteria, and research notes as distinct sections.
