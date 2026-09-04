# Workflow Guidelines

## Purpose of this file

This file defines the chronological execution process and deliverable structure. It relies on `Agent-Guidelines.md` for collaboration behavior and `Cinematic-Prompting-Ruleset.md` for production invariants.

At the entry and exit of every material phase, apply the Guided Choice Protocol from `Agent-Guidelines.md`. Proactively state what decision is needed, recommend a path, show relevant options and consequences, and wait at required approval gates. The user should never need to ask what their options are or request clarification questions.

## Phase 0 — Classify the assignment

Identify:

- operating mode: static shot, static-to-video shot, campaign/sequence, research-to-shotlist, script breakdown, or output repair;
- source material: topic, brief, script, shot list, existing images/video, or references;
- deliverables and platform;
- intended target models and Magnific modes, if known;
- whether current factual or model-capability research is needed;
- for an output-review request, whether the current platform exposes read-only Magnific history/search/retrieval capabilities.

Keep the process proportional, but retain the creative-direction gate and still-first video sequence.

Tell the user which operating mode you recommend and let them preserve existing shots, enrich partial material, begin research-to-shotlist work, start from one shot, or switch to output validation/repair. Capability detection does not authorize searching a connected account.

## Phase 1 — Parse the brief and ask only material questions

Extract what is already known, then ask one compact batch covering only missing decisions that could change the work:

Always include this new-project check, even if the rest of the brief is complete: `Is there a particular brand hex code or defined palette we should deliberately incorporate in the images?` Offer three answer paths: exact hex code(s) with priority; derive the palette from supplied brand guidelines or references; or no locked brand color. If a code is supplied, ask only the necessary follow-up about intended use or exclusions and recommend plausible integration surfaces rather than assuming a global color cast.

1. **Purpose and audience:** desired response, message, action, placement, and viewing context.
2. **Deliverables:** still/video, shot count, duration, aspect ratio, resolution, frame rate, audio, copy, logo, and platform requirements.
3. **Mood and style:** emotional promise, realism versus stylization, references, anti-references, brand character, and intended production value.
4. **Brand color:** exact hex codes or defined palette, priority, intended integration surfaces, exclusions, and whether exact compliance needs finishing or compositing.
5. **Continuity:** recurring talent, characters, products, wardrobe, props, locations, time progression, and deliberate changes.
6. **Cinematography:** shot language, format feel, lens behavior, depth of field, movement, focus, lighting, grade, and texture.
7. **World occupancy:** expected background population and secondary activity; identify any shot or sequence that intentionally requires isolation, exclusivity, closure, or an empty environment.
8. **Constraints:** exact brand/product details, usage rights, cultural accuracy, safety, deadline, budget, and iteration limits.
9. **Visual-development status:** complete shot list, partial ideas, locked script moments, or research-to-shotlist need; define what may be invented, enriched, verified, or must remain unchanged.

Ask what each supplied reference should control, but do not assume every available image should be used. Record which references are merely available and which are selected candidates for specific shots.

Present the missing decisions as one compact guided batch with examples or options. Do not ask the user to generate the questionnaire or supply technical terminology they may not know.

## Phase 2 — Direction Check

Before prompt production, present a short creative treatment for approval.

If direction is clear, return one treatment that translates the user's language into concrete visual decisions.

If direction is incomplete or contradictory, use `references/Mood-and-Style-Framework.md` to propose two or three distinct creative lanes. Put the recommended lane first. Do not continue until the user selects, combines, or redirects them.

The Direction Check must include:

- interpretation of the objective and audience;
- emotional promise and visual thesis;
- realism/stylization level;
- palette and lighting logic;
- approved brand hex codes, their intended visual roles, and surfaces that should remain naturally colored;
- production design and material language;
- performance, human energy, occupancy, and secondary life in the environment;
- composition, optics, texture, and grade;
- motion and pacing principles for video;
- anti-goals and recognizable AI failure risks;
- assumptions and unresolved choices.

## Phase 3 — Shot Research and visual discovery when needed

Run this phase when the user asks for help deciding what to show, has no usable shot list, supplies only a broad guideline or partial script, or wants factual/cultural enrichment. Skip it when the supplied visuals are already sufficiently defined unless the user requests verification or alternatives.

Read `references/Shot-Research-and-Shotlist-Design.md` and:

1. define the research mandate from the objective, audience, approved direction, scope, claims, required proof, sensitivities, duration, and constraints;
2. research only the facts, human behaviors, places, cultural context, brand truths, and visual opportunities that can improve the piece;
3. separate verified findings from creative hypotheses and record sources beside factual claims;
4. build a Visual Research Board of candidate motifs, evaluating relevance, narrative role, visual potential, brand fit, feasibility, and cliché/sensitivity risk;
5. when different organizing ideas are viable, propose two or three narrative routes with a recommendation;
6. obtain approval of one route, a combination, or a redirect;
7. turn the approved route into a proposed shot list with provisional IDs, visual ideas, narrative functions, research basis, duration/priority, likely treatment, feasibility notes, and fallbacks;
8. obtain shot-list approval before continuing.

For current, cultural, historical, geographic, route, product, or brand claims, use live research and prefer authoritative primary sources. If source access is unavailable, state the limitation and label unverified ideas as hypotheses.

Do not force one research fact into one shot. Sequence only the strongest motifs into a coherent emotional and narrative progression. Leave exact composition and movement choices for the Per-Shot Direction Check unless they are inseparable from the concept.

## Phase 4 — Build the production bible

After the Direction Check is approved, define:

- approved base look and mood;
- locked continuity invariants;
- controlled variables;
- character, product, wardrobe, location, and prop descriptions;
- reference manifest and role assignments;
- camera, lens, focus, lighting, color, texture, and movement grammar;
- brand-color integration map and tolerance for exact versus perceptual matching;
- lived-in occupancy grammar: expected density, background roles, secondary actions, and approved empty-space exceptions;
- scene or sequence overrides;
- target-model and generation-mode strategy;
- acceptance criteria.

For a single simple shot, this may be a compact block. For a campaign or script, make it a reusable project section.

## Phase 5 — Design the shot architecture

For every shot, define its purpose in the final edit and its narrative purpose before decorative detail.

Assign:

- scene ID and shot ID;
- narrative function and emotional beat;
- intended duration and relationship to adjacent shots;
- subject blocking, screen direction, and geography;
- composition, shot size, camera height/angle, and lens behavior;
- start state, action, and end state;
- lighting and environmental behavior;
- context-appropriate background people, staff, passersby, patrons, or other secondary life, with an explicit reason for any empty-space exception;
- references and continuity carried in/out;
- whether an end frame is required.

Do not combine several continuous camera shots into one generation. Coverage is represented as separate shot IDs.

## Phase 5A — Per-Shot Direction Check

Run this gate before writing the first static prompt for each shot.

First ask the user to choose how they want to direct it:

1. **User-described:** the user explains the camera/viewpoint idea informally or technically; the agent develops and translates it.
2. **Agent-proposed:** the agent offers two or three meaningfully different options.
3. **Hybrid:** the user supplies part of the intention and the agent completes it or offers refinements.

For every still image, confirm or propose:

- shot size and composition;
- camera height and angle;
- lens/perspective behavior;
- subject placement and visual hierarchy;
- foreground, midground, and background design;
- occupancy, background human activity, and secondary environmental action;
- depth of field and focus plane;
- how the viewpoint expresses the approved mood and shot function.

For every video shot, also confirm or propose:

- camera support and stability character;
- three-dimensional movement path;
- pan, tilt, roll, orbit, or subject-tracking behavior;
- optical zoom, if any;
- framing evolution and parallax;
- initial and final focus targets, cue, speed, and landing;
- timing, acceleration, deceleration, settle, and hold;
- end-frame composition and whether a separate end image is required.

When the agent proposes options, each option must state:

- a short descriptive name;
- what the audience feels or notices;
- start composition;
- camera/viewpoint behavior;
- focus behavior;
- end composition;
- generation complexity or risk;
- why it fits the shot.

Put the recommended option first. Wait for approval before Phase 6.

For a long shot list, present the checks in a compact table for batch approval. Handle hero shots, ambiguous shots, and technically complex movements individually.

## Phase 5B — Reference-image and Magnific node-binding check

Run this check for every shot or approved batch before the Prompt Readiness Summary. Read `references/Magnific-Reference-Node-Bindings.md` when any image is available or may be used.

First ask whether a usable reference image exists, then offer:

1. use the image as a reference;
2. leave it unused;
3. review it before deciding;
4. continue without a reference because none is available.

For each image selected for use:

- assign the exact visual job and priority;
- identify unwanted traits that must not transfer;
- confirm whether it is already available in the relevant Magnific canvas or node graph;
- obtain the exact Magnific node name as displayed in the interface before copy-ready prompt drafting;
- record whether the image will be addressed through an `@` mention or a dedicated reference/start/end setting in the selected mode.

Do not infer the node name from the filename or invent a placeholder. If the name is unavailable, the user may supply it after uploading, choose not to use the image, or hold the dependent prompt. Keep drafting locked only for prompts that require the unresolved binding; ready prompts may proceed as an explicitly named subset.

## Phase 5C — Static Prompt Authorization

Prompt drafting remains locked after the Per-Shot Direction Check. Compile the approved decisions into a concise Prompt Readiness Summary before writing any copy-ready static prompt.

For each shot or approved batch, confirm:

- purpose, emotional beat, subject, action, and continuity state;
- shot size, composition, camera position, height, angle, lens/perspective behavior, and aspect ratio;
- foreground/midground/background design and visual hierarchy;
- production design, wardrobe/props, lighting, palette, texture, grade, depth of field, and focus;
- assigned use of any locked brand hex codes and the lived-in occupancy plan or approved empty-space exception;
- start state, end state, and whether a separate end image is required;
- reference-image availability and use decisions;
- references selected for use, the job assigned to each, and every exact Magnific node name/binding method required by the chosen mode;
- target image model/mode, output requirements, and material generation risks;
- for video-bound shots, the approved movement/focus/landing concept that the static endpoints must support;
- assumptions, recommended defaults, unresolved conflicts, and intentionally deferred items.

Ask: `Approve this specification and authorize static prompt drafting for [shot IDs or batch]?`

Offer these actions:

- approve and authorize the named scope;
- request changes to specific fields;
- authorize only a ready subset;
- hold and revisit research, direction, shot architecture, or continuity.

Do not include the copy-ready prompts in the same response as the authorization request. Continue to Phase 6 only after an unambiguous affirmative response covering the named scope. If some shots are incomplete or have unresolved selected reference bindings, authorize and draft only the ready subset.

## Phase 6 — Build the static shot package

Create the static prompt package before any final video prompt.

Build it incrementally when a later static prompt depends on an image that has not yet been generated. For example, if the end image should use the approved start image as a reference, deliver and generate the authorized start prompt first. After the start image is selected, run the reference-image check again, obtain its exact Magnific node name, present a compact readiness update for the end image, and obtain authorization before writing the copy-ready end prompt. Never fill the dependency with a guessed node or production placeholder.

For each shot provide:

1. **Canonical static specification:** model-neutral creative intent.
2. **Start-image prompt:** copy-ready prompt adapted to the chosen image model.
3. **End-image decision:** required or not required, with a one-line reason and whether its prompt must wait for an approved start-image node.
4. **End-image prompt:** when required and all selected bindings are resolved, describe the final state while preserving locked continuity; otherwise mark it as deliberately deferred until the named dependency exists.
5. **Reference bindings:** image order, what each reference controls, exact confirmed Magnific node names, and whether each is used through an `@` mention or dedicated control.
6. **Magnific settings card:** model, mode, aspect ratio, resolution, exact node/reference assignments, and other relevant live settings.
7. **Static acceptance criteria:** the visible conditions that make the frame usable for video.

Separate prompts from explanatory notes so they can be copied without cleanup.

For a multi-shot project, the agent may deliver all static shot prompts in one organized report, but each shot remains independent.

## Phase 7 — Static review and approval

When static results are ready for review, determine how the user wants to provide them. If the current platform has read-only Magnific history/search/retrieval capabilities, read `references/Magnific-MCP-Validation.md` and offer:

1. search recent Magnific history read-only, then show likely matches for the user to select;
2. retrieve a creation from a link or selection supplied by the user;
3. use manually uploaded start/end images;
4. skip or defer review when the next step does not depend on approval.

If no Magnific connection is available, offer the manual and direct-link/file paths without treating the missing connector as a blocker. Explain that read-only retrieval does not generate or transform media, and that any paid or credit-consuming action would require a separate explicit approval. Wait for the user's choice before searching history.

After the exact images are selected, review them against:

- approved mood and visual thesis;
- identity and product fidelity;
- composition and shot function;
- location geography and continuity;
- light direction, palette, material response, and texture;
- brand-color integration, plausible occupancy, background human behavior, and whether the environment feels operational rather than staged or abandoned;
- hands, typography, logos, packaging, reflections, shadows, and topology;
- start/end compatibility and plausible motion path.

For failures, recommend the smallest repair: prompt revision, reference change, localized edit, image composite, different image model, or shot redesign.

Do not write the final video prompt until the relevant static frame or frame pair is approved.

## Phase 7A — Video Prompt Authorization

After static approval, compare the actual start/end images with the approved shot specification. If their geometry, blocking, focus, or endpoints require a movement change, revise and approve that change first.

Re-run the reference binding check for every approved start image, end image, or additional image that will be used by the video mode. Obtain each exact Magnific node name before the video authorization request when the selected mode requires node-based assignment or an `@` mention. If the mode uses dedicated start/end slots, record those exact assignments rather than adding redundant prompt mentions.

Present a concise final motion readiness summary containing:

- approved start/end image IDs;
- exact Magnific node names and binding methods for selected start/end/additional references;
- support and camera path;
- orientation and framing evolution;
- lens operation;
- focus choreography;
- subject and environmental motion;
- duration, timing, easing, settle, and landing state;
- target video model/mode and material risks;
- any change from the earlier Per-Shot Direction Check.

Ask: `Approve this motion specification and authorize the final video prompt for [shot IDs or batch]?`

Offer approval, specific changes, subset authorization, movement simplification, or a return to static-frame repair when the endpoints do not support the move.

Do not include the copy-ready video prompt in that authorization request. Continue to Phase 8 only after explicit approval.

## Phase 8 — Build the single-shot video package

Read `references/Camera-Movement-Language.md`, then read the relevant model guidance in `references/Model-Adapters.md` and verify live Magnific options.

For each approved shot provide:

1. **Approved start image:** reference ID or filename.
2. **Approved end image:** reference ID or filename when used.
3. **Camera Movement Breakdown:** support, path, orientation, lens operation, framing evolution, focus choreography, timing/easing, parallax, and landing frame.
4. **Canonical motion specification:** one continuous shot, independent of model syntax.
5. **Copy-ready video prompt:** adapted to the selected model and mode, with camera and focus instructions clearly stated.
6. **Reference bindings:** what the start frame, end frame, or other references control, with each exact confirmed Magnific node name and binding method.
7. **Magnific settings card:** model, image-to-video/start-end mode, exact node assignments, duration, aspect ratio, resolution, audio controls, and relevant settings.
8. **Motion acceptance criteria:** performance, camera path, focus, physical behavior, and final landing state.
9. **Fallback:** the smallest alternate prompt, reference strategy, model, or post-production solution if the first approach fails.

The video prompt should describe one primary action and one coherent camera choreography. It may combine spatial movement, orientation, lens operation, and focus movement when their timing and relationship are clear. It must not request cuts, coverage changes, or a montage.

## Phase 9 — Generation QC and continuity update

When a generated video or revised visual output becomes part of the workflow, use the same optional input-acquisition choice from Phase 7. If read-only Magnific history is available, offer it; otherwise accept a direct link, current selection, or manual upload. Do not retrieve account history without the user's choice and do not call a modifying tool as part of QC.

After the exact result is selected:

- compare the actual output with the canonical specification;
- classify it as accepted, repairable, or rejected;
- use targeted intra-shot repair for local failures;
- update future shots only with accepted intentional state changes;
- do not propagate accidental drift;
- log model, mode, prompt version, settings, references, generation ID, and decision.

End the review with visible options: accept, inspect another result, retrieve another history candidate, request prompt-only repair instructions, revise references or model strategy, use post-production, redesign, or stop. If generation or transformation is proposed, identify it as a separate action, disclose the known credit consequence or uncertainty, and obtain explicit authorization before calling it.

Keep temporal repair separate from final upscaling and finishing.

## Phase 10 — Deliver and save the report

Use this report order:

1. Project metadata and version.
2. Approved Direction Check.
3. Shot Research mandate, findings, Visual Research Board, narrative route, and sources when used.
4. Approved proposed shot list when developed by the agent.
5. Production bible.
6. Reference manifest.
7. Shot index.
8. Approved Per-Shot Direction Checks.
9. Static Prompt Authorization record and approved scope.
10. Static shot packages.
11. Static approval/QC notes, including optional retrieval source and selected creation metadata.
12. Video Prompt Authorization record and approved scope.
13. Single-shot video packages, added only after static approval and authorization.
14. Global and shot-specific avoidance rules.
15. Revision/generation log, including read-only retrievals and any separately authorized paid actions.
16. Other research sources and notes, separate from prompts.

Save project reports in the user-specified project folder. Do not mix temporary drafts with final deliverables.

## File naming

Use this grammar unless the user specifies another convention:

`YYYY_Client-or-Project_Project-Name_Deliverable_Version.ext`

Examples:

- `2026_Airline_Insignia-Launch_Shot-Prompts_V01.md`
- `2026_Client_Project-Name_SC03-SH02_Start-Frame_A.png`
- `2026_Client_Project-Name_SC03-SH02_End-Frame_A.png`
- `2026_PersonalProject_Project-Name_SC03-SH02_Video_V02.mp4`

Use underscores to separate naming sections and hyphens within a section. Use stable scene/shot IDs and alphabetic suffixes for creative variants.
