# Start Here — Cinematic Prompting Workflow

You do not need to know how to code or how AI systems are built to use this package.

This workflow helps you work with an AI assistant to plan and write high-quality prompts for cinematic images and single-shot video clips, especially when using Magnific with models such as Seedream, Nano Banana, Seedance, and Kling.

## What this package does

It helps you:

- turn a rough topic, creative brief, script, or shot list into a clear visual direction;
- research relevant facts, culture, places, behaviors, and visual motifs when you do not yet know what to show;
- turn that research into narrative-route options and a proposed shot list;
- decide the mood and style before prompt writing;
- ask whether exact brand hex colors or a supplied palette should be integrated, and define where they belong;
- plan each shot's viewpoint, composition, camera movement, and focus;
- recommend a primary model, fallback, prompt form, reference plan, and iteration/cost strategy for each shot;
- decide whether available reference images should be used, ignored, or reviewed first, and bind selected Magnific references to their exact node names;
- keep public, commercial, travel, hospitality, workplace, and social environments plausibly lived-in unless you intentionally approve an empty or private scenario;
- create and approve static start images before generating video;
- create end images when the final framing or action needs control;
- write one continuous camera shot per generated video file;
- maintain character, product, wardrobe, location, lighting, and style continuity;
- optionally retrieve selected Magnific history results for validation when the current AI platform has an active read-only connection;
- reduce generic AI-looking results and identify likely failures.

It does not automatically generate images or videos unless the AI platform is connected to generation tools. In the normal workflow, the assistant writes the prompts and you use them in Magnific.

## Before you begin

You need:

- access to an AI assistant that can read Markdown files, such as Codex, Claude Code, Claude Projects, or another file-aware chat assistant;
- web access or research tools when the project requires current or source-backed Shot Research;
- access to Magnific or another image/video generation platform;
- a topic, brief, script, shot list, or even just a rough idea;
- any useful brand guidelines, references, product images, character images, or existing campaign materials.

Do not upload confidential or restricted material to an AI service unless the applicable owner, collaborator, employer, or client policies allow it. Confirm account privacy, data retention, and usage-right requirements first.

## The easiest way to start

### 1. Unzip the package

Double-click the ZIP on macOS or Windows. Keep the folder structure intact. Do not move individual reference files out of their folders.

### 2. Choose your AI platform

- **Codex:** follow the Codex section in `Cross-Platform-Setup.md`.
- **Claude Code:** follow the Claude Code section in `Cross-Platform-Setup.md`.
- **Claude Projects:** upload the listed files and paste the supplied project instructions.
- **Another AI chat:** attach the core files and use `platforms/Generic-Chat-Starter.md`.

### 3. Prepare your first brief

Open `templates/Project-Brief-Template.md`, make a copy, and fill in whatever you know. It is fine to leave fields blank—the assistant should ask only the questions that matter.

At the beginning of each new project, the assistant should always ask whether there is a particular brand hex code or defined palette to incorporate. You can provide exact code(s), ask it to derive a palette from supplied brand guidelines, or say that no color is locked.

### 4. Start the conversation

Give the assistant your brief, topic, script, or shot list. Add reference images when useful and explain what each reference should control.

You do not need to know which questions to ask. At every important stage, the assistant should state the current decision, recommend a path, and show the relevant options with their consequences. You can choose an option, combine options, describe your own direction, ask it to use its recommendation, defer, or revisit an earlier decision when appropriate.

### 5. Approve the Direction Check

Before prompts, the assistant will translate your goals into a proposed mood and visual treatment.

The Direction Check should also explain how approved brand colors will appear and how populated or active the world should feel. Unless you intentionally request isolation, closure, exclusivity, or emptiness, locations should include believable background people and activity appropriate to the place and time.

If your direction is vague, it should offer two or three options. You can:

- choose one;
- combine parts of different options;
- reject them and redirect the assistant;
- specify a different mood for an individual scene.

Do not approve vague language such as `make it cinematic` or `make it premium` without concrete visual consequences.

### 6. Use Shot Research when you do not yet have the visuals

If your script or shot list already explains what should appear, continue to the next step.

If you only have a guideline, message, destination, product story, partial script, or theme, tell the assistant you need **Shot Research**. It should:

1. confirm what the research needs to achieve;
2. find and source relevant facts, human behaviors, places, cultural details, brand truths, and visual motifs;
3. distinguish verified facts from creative interpretations;
4. avoid stereotypes, postcard checklists, and pretty-but-irrelevant trivia;
5. propose two or three narrative routes when useful;
6. turn the approved route into a proposed shot list for your approval.

For example:

> I have a manifesto for a new direct route between Rio de Janeiro and Lisbon, but no visuals yet. Research relevant cultural, human, geographic, culinary, and travel connections, then propose narrative routes and a shot list. Verify current route and campaign facts before using them.

Use `templates/Shot-Research-Template.md` when you want a structured research report. The assistant should place sources beside factual claims and keep them out of copy-ready generation prompts.

### 7. Approve each Per-Shot Direction Check

Before the first prompt for each shot, choose one of these paths:

1. Describe your camera or composition idea in your own words.
2. Ask the assistant to propose two or three options.
3. Give part of the idea and ask the assistant to complete it.

For static images, this check covers framing, camera height, angle, perspective, subject placement, depth, and focus.

For video shots, it also covers camera support, physical path, pan/tilt/orbit, zoom, framing evolution, focus pull, timing, and end composition.

You do not need to know the technical names. For example, you can say:

> I want to get closer while moving toward the right. Something in the foreground should gradually become the focus.

The assistant should determine whether you mean a physical push-in, optical zoom, true dolly zoom, lateral move, or a combination—and explain the result before prompting.

### 8. Choose reference images and confirm Magnific node names

Before the assistant prepares the Prompt Readiness Summary, it should ask whether a useful reference image is available for the shot. You can choose to:

1. use it as a reference;
2. leave it unused;
3. ask the assistant to review it before deciding;
4. continue without a reference if none is available.

If you choose to use an image in Magnific, tell the assistant the exact name of that image's node as displayed in Magnific. Copy the name rather than paraphrasing it. The assistant must preserve that spelling, capitalization, spacing, punctuation, and numbering in any `@` mention or dedicated reference assignment.

If the image is not in Magnific yet, upload it and obtain the node name before prompt drafting—or choose to continue without it. The assistant should never guess from the filename or put `@image1`, `@reference`, or another placeholder into a production prompt.

### 9. Authorize the static prompts

After all relevant shot decisions are complete, the assistant must show you a **Prompt Readiness Summary**. This should consolidate the shot purpose, subject/action, composition, camera position and angle, lens behavior, production design, lighting, palette and approved brand-color use, plausible occupancy and secondary background activity, depth of field, focus, start/end state, reference-use decisions, exact Magnific node bindings for selected images, model strategy, and important risks.

It will then ask whether you approve that specification and authorize static prompt drafting. The prompts must not appear in the same message as the authorization request.

You can reply naturally: `Approved`, `Looks good, proceed`, or `Write the static prompts for SH01–SH04`. You do not need to use an exact phrase.

If you are not ready, the assistant should clearly offer alternatives such as changing a field, authorizing only selected shots, holding the prompts, or returning to an earlier decision.

### 10. Create the static prompts

The assistant writes a start-image prompt for each shot. It will also recommend an end image when the final composition, pose, reveal, transformation, or focus destination needs to be controlled.

When an end image should reference the generated start image, this happens in two passes: generate and approve the start image, give the assistant its exact Magnific node name, then authorize the end-image prompt. This prevents the assistant from guessing a node that does not exist yet.

Copy the prompt and settings into Magnific. Generate variations, then select or repair the strongest frame.

### 11. Return the approved images

Show the approved start image—and end image when used—to the assistant. It should check composition, continuity, brand/product fidelity, lighting, materials, hands, typography, reflections, and other common problems.

If the current AI platform has an active Magnific connection with read-only history access, the assistant should detect it and offer these choices before review:

1. search recent Magnific history read-only and let you select the matching result;
2. use a Magnific creation link or current selection you provide;
3. use images you upload manually;
4. skip or defer validation when appropriate.

It should not search your history until you choose that option. Read-only retrieval and critique do not generate or transform media and do not normally consume Magnific generation credits. Any generation, edit, variation, upscale, or video operation is a separate action: the assistant must explain the known credit consequence and obtain your explicit approval first. If no connection is available, upload the files manually; the rest of the workflow still works.

### 12. Authorize the video prompt

After approving the actual start/end images, review the final motion readiness summary. If those images changed the geometry, focus, or movement endpoints, resolve that first. Authorize the final video prompt only when the camera choreography still works.

### 13. Create the video prompt

Only after the static images are approved should the assistant write the final video prompt. Each generated file should contain one continuous camera shot without baked-in cuts to other setups.

The prompt should clearly describe what the camera, subject, environment, and focus are doing over time.

### 14. Edit in post-production

Generate separate clips for each shot. Assemble, trim, cut, transition, grade, and mix them in your editing software.

## The approval gates

The workflow intentionally pauses at six points when Shot Research is needed:

1. **Direction Check:** Does the mood/style fit the project?
2. **Research/shot-list approval:** Are these relevant things to show, organized into the right story?
3. **Shot specification and Static Prompt Authorization:** Are all material shot decisions complete, and may the agent now draft image prompts?
4. **Static approval:** Are the generated start/end images strong and consistent?
5. **Video Prompt Authorization:** Does the final motion plan fit the approved images, and may the agent now draft the video prompt?
6. **Video QC:** Did the generated motion follow the approved shot?

When a complete script or shot list is already supplied, the second gate can be skipped.

These pauses reduce wasted generations and prevent the AI from making important directing choices by accident.

## Folder map

```text
cinematic-prompting/
├── README.md                         Package doorway
├── START-HERE.md                     Read this first
├── SKILL.md                          Entry point used by AI assistants
├── Cross-Platform-Setup.md           Installation and platform setup
├── Agent-Guidelines.md               How the assistant should collaborate
├── Cinematic-Prompting-Ruleset.md    Non-negotiable production rules
├── Workflow-Guidelines.md            Step-by-step working process
├── references/
│   ├── Mood-and-Style-Framework.md
│   ├── Shot-Research-and-Shotlist-Design.md
│   ├── Camera-Movement-Language.md
│   ├── Model-and-Prompt-Strategy.md
│   ├── Model-Adapters.md
│   ├── Magnific-Reference-Node-Bindings.md
│   └── Magnific-MCP-Validation.md
├── templates/
│   ├── Project-Brief-Template.md
│   ├── Shot-Research-Template.md
│   ├── Shot-Direction-Check-Template.md
│   ├── Prompt-Readiness-and-Authorization-Template.md
│   └── Shot-Prompt-Package-Template.md
├── examples/
│   └── Worked-Example_Static-to-Video.md
├── platforms/
│   ├── Claude-Project-Instructions.md
│   └── Generic-Chat-Starter.md
└── agents/
    └── openai.yaml                   Optional Codex/OpenAI interface metadata
```

## Short glossary

- **AI assistant:** The conversational AI that helps plan and write prompts.
- **Prompt:** Instructions given to an image or video generation model.
- **Model:** The specific image/video system selected inside Magnific.
- **Reference image:** An uploaded image used to control identity, product, style, lighting, composition, or another visual property.
- **Magnific node name:** The exact name shown for an image node in Magnific. The assistant uses this name when compiling an `@` mention or recording a dedicated reference assignment.
- **Shot:** One uninterrupted camera take between edits.
- **Clip:** One generated video file. In this workflow, one clip normally contains one continuous shot.
- **Start image/frame:** The approved static image used as the beginning of a video generation.
- **End image/frame:** An approved static image defining where the generated motion should finish.
- **Shot size:** How much of the subject is visible, such as wide, medium, close-up, or detail.
- **Camera path:** How the camera physically moves through three-dimensional space.
- **Pan/tilt:** Rotating the camera left/right or up/down without necessarily moving its position.
- **Zoom:** Changing focal length without physically moving the camera.
- **Focus pull/rack focus:** Deliberately changing sharp focus from one subject or depth plane to another.
- **Depth of field:** The range of distances that appear acceptably sharp.
- **Aspect ratio:** The shape of the image, such as 16:9, 9:16, or 1:1.
- **Continuity:** Keeping people, products, wardrobe, locations, lighting, and story state consistent across shots.
- **Research mandate:** The question, scope, factual requirements, and creative purpose guiding Shot Research.
- **Visual Research Board:** A shortlist of source-backed or clearly labeled speculative ideas that might become shots, evaluated for relevance and feasibility.
- **Narrative route:** The organizing story logic that determines which visual ideas appear and in what progression.
- **Post-production:** Editing, compositing, color grading, sound, and finishing after generation.
- **MCP/connector:** An optional connection that lets an AI assistant use specific Magnific capabilities. In this workflow, history retrieval is read-only unless you separately authorize a modifying operation.

## Common beginner problems

### The assistant starts writing prompts immediately

That means the workflow was not loaded or the Prompt Authorization Gate was not followed. Say:

> Stop. The Prompt Authorization Gate has not been completed. Present the Prompt Readiness Summary and wait for my explicit authorization without drafting prompts in the same response.

Confirm that `SKILL.md` and the referenced files were installed or uploaded correctly.

### The assistant asks vague questions or does not explain your options

Say:

> Apply the Guided Choice Protocol. State the current decision, recommend a path, and show me the relevant options and consequences. Let me choose, combine, describe my own direction, defer, or revisit when valid.

If this keeps happening, confirm that the current `Agent-Guidelines.md` is available to the assistant.

### The assistant invents a generic shot list without research

Say:

> Stop. Run the Shot Research stage first. Show me the research mandate, verified findings versus creative hypotheses, Visual Research Board, and narrative-route options before proposing the shot list.

Confirm that `references/Shot-Research-and-Shotlist-Design.md` is available to the assistant.

### The style options all feel the same

Ask for alternatives with different emotional and production logic, not just different colors or lenses.

### The camera instructions are vague

Ask for the `Camera Movement Breakdown` from `references/Camera-Movement-Language.md` before accepting the video prompt.

### The video contains cuts or changes angle by itself

Confirm that the prompt says `one continuous camera shot`, `no cuts`, and defines one coherent start-to-end movement. Generate separate coverage as separate clips.

### Character or product details change

Use stronger reference images, assign each reference a specific job, simplify conflicting instructions, and repair the static frame before video generation.

### The prompt points to the wrong Magnific image

Check the exact node name in Magnific and copy it to the assistant. Do not provide only the upload filename. Ask the assistant to update every affected `@` mention and settings-card assignment using the confirmed node name from `references/Magnific-Reference-Node-Bindings.md`.

### The assistant cannot see my Magnific history

The connection may not be installed, authenticated, or available on that AI platform. Upload the selected result manually or provide a usable creation link. Magnific history access is optional and should never block the workflow.

### The result looks generically AI-generated

Return to the approved mood/style treatment and check lighting motivation, production design, material behavior, focus hierarchy, texture, saturation, reflections, hands, typography, and continuity. Avoid adding random grain, flare, fog, or chromatic aberration as a substitute for direction.

## Where to go next

- Read `examples/Worked-Example_Static-to-Video.md` for a complete simplified example.
- Fill in `templates/Project-Brief-Template.md` for your first project.
- Use `templates/Shot-Research-Template.md` when you need help discovering and organizing what the piece should show.
- Use `templates/Shot-Direction-Check-Template.md` to review each shot.
- Use `templates/Prompt-Readiness-and-Authorization-Template.md` to record exactly what was approved before prompt drafting.
- Use `templates/Shot-Prompt-Package-Template.md` to organize final deliverables.
