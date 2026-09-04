# Cinematic Prompting Workflow

This is a guided creative-direction and prompt-writing system for cinematic images and single-shot video clips.

It is designed for people who care about visual quality but do not want to memorize prompt formulas, filmmaking terminology, AI settings, or agent technology. You can arrive with a complete script—or with nothing more than “I need an image that feels joyful and real.” The assistant helps you work out the missing decisions before it writes anything for generation.

No coding experience is required.

The workflow is designed around Magnific and models such as Seedream, Nano Banana, Seedance, and Kling, but its creative-direction system remains useful with other image and video tools.

## In one sentence

You bring the creative problem; the assistant helps research, direct, organize, and translate it into approved, copy-ready image and video prompts.

## Why use a workflow instead of asking for a prompt immediately?

A model can fill missing information quickly, but its defaults are often the source of the “AI look.” It may choose generic lighting, exaggerated depth of field, empty public spaces, random camera movement, inconsistent characters, or reference-image traits you never intended to copy.

This workflow makes those choices visible. It asks what matters, explains practical options, recommends a direction, and pauses for approval before spending time or generation credits on the wrong idea.

## What it can help you do

### Find the visual idea

If you know the message but not what to show, the assistant can research relevant places, behaviors, culture, product truths, and visual motifs. It separates verified findings from creative ideas, proposes narrative approaches, and turns the selected approach into a shot list.

Example:

> I have a manifesto about a new direct flight between Rio and Lisbon, but no visual ideas. Research meaningful connections between the cities and propose two or three narrative routes before creating a shot list.

### Direct mood and style

The assistant helps define what words like “premium,” “playful,” “intimate,” or “energetic” actually mean on screen: palette, lighting, contrast, materials, human performance, composition, lens behavior, texture, grade, movement, and pacing.

Example:

> It should feel premium without looking like a generic luxury ad. Give me distinct visual directions and explain the difference.

### Design individual shots

For each image or clip, you can describe the camera idea yourself, ask for two or three options, or combine both approaches. The assistant helps decide shot size, camera height, angle, lens behavior, foreground and background, focus, lighting, and the purpose of the shot in the final edit.

Example:

> I picture the camera getting closer and moving right while focus changes to something in the foreground, but I do not know the correct terminology. Develop that movement for me.

### Choose the model and prompt approach

The assistant recommends a primary model and mode for each shot, explains why it fits, names a practical fallback, and chooses a prompt form based on the control problem. A cinematic lifestyle frame may use labeled natural prose; a precision edit may use `CHANGE`, `PRESERVE EXACTLY`, and `REFERENCE JOBS`; a dense product layout may benefit from object-by-object structure.

It also identifies the main risks and proposes whether to explore cheaply first, move directly to a precision pass, or stop before an expensive generation. If two materially similar attempts fail, it should diagnose the real problem instead of endlessly adding instructions to the prompt.

Example:

> Recommend the best image model and prompt structure for this shot, explain the fallback, and tell me what would make you stop and change strategy.

### Create still-first video shots

Every video shot begins as an approved static image. When the final composition needs control, the workflow also creates an end image. Only after those frames work does it write the motion prompt.

Each generated clip represents one continuous camera shot. Separate angles and coverage are generated separately and edited together afterward.

### Keep the world believable

Public and social environments should normally feel occupied and operational. A restaurant has other patrons and staff; a busy beachfront has believable background life. Empty or private spaces are possible, but they should be intentional rather than an accidental AI default.

### Use references precisely

The assistant asks whether an available image should be used, left unused, or reviewed first. Every selected reference gets a specific job, such as identity, product, wardrobe, composition, lighting, palette, or texture.

When working in Magnific, the assistant asks for the exact node name before writing a prompt that refers to the image. It will use the confirmed name, such as `@Character_Closeup_02`, and never guess `@image1` from a filename.

### Maintain consistency

For multi-shot work, the assistant records the elements that must remain stable—characters, products, wardrobe, locations, palette, lighting logic, and optical style—while allowing approved changes between shots.

### Review and repair results

You can return generated images or clips for quality control. The assistant checks them against the approved direction, identifies the smallest failing dimension, and recommends a targeted prompt revision, reference change, localized edit, model change, shot redesign, or post-production fix.

## What can you start with?

Anything from this list is enough:

- a topic or one-sentence idea;
- a creative brief;
- a full script;
- a partial or complete shot list;
- one image you want to create;
- reference images;
- an existing generation that needs repair;
- a camera movement you can picture but cannot explain technically.

Blank information is acceptable. The assistant should notice what is missing and give you understandable choices instead of expecting you to know what to ask.

## What happens after you start?

1. **Brief check:** What are we making, for whom, and where will it be seen?
2. **Color check:** Is there a brand hex code or palette to integrate?
3. **Direction Check:** Does the mood and visual system fit the project?
4. **Shot Research, when needed:** What is relevant and interesting to show?
5. **Shot design:** How should each moment be framed, lit, focused, and moved?
6. **Model & Prompt Strategy:** Which model, mode, prompt form, fallback, reference plan, and iteration path best fit this shot?
7. **Reference check:** Which available images should be used, and what are their exact Magnific node names?
8. **Prompt Readiness Summary:** Are all important choices and mandatory stop checks resolved?
9. **Authorization:** Do you want the assistant to write the named prompt or batch now?
10. **Static prompting and review:** Build and approve the start image, then the end image when required.
11. **Video authorization and prompting:** Confirm the motion and model strategy against the actual frames, then write one continuous-shot video prompt.
12. **QC and revisions:** Accept, repair, simplify, change strategy, redesign, or finish in post.

The assistant does not need to make a simple image feel bureaucratic. It keeps the same safety and creative-control gates while shortening the presentation to fit the assignment.

## Four easy ways to begin

### 1. One image

> Help me create a happy, accessible key visual for a mobile game. I have no camera or lighting decisions yet. Guide me through the options before writing the prompt.

### 2. One video shot

> I want a five-second shot of a woman approaching a hotel window. Start with the static frame and help me describe the camera movement. I may want a controlled end frame.

### 3. A script without visuals

> Break down this script, research possible visual motifs, and propose a shot list. Preserve the copy and wait for my approval before developing prompts.

### 4. A bad generation

> Review this image. The main subject is good, but the location feels empty and artificial. Tell me the smallest changes needed without redesigning everything.

## Important rules you can rely on

- No production prompt before the relevant approval gate.
- Static images before video prompts.
- One uninterrupted camera shot per generated clip.
- Clear camera path, focus behavior, pacing, and landing state.
- Lived-in environments unless emptiness is deliberate.
- Brand colors used intentionally rather than as a blanket tint.
- References assigned specific jobs and exact Magnific node names.
- A recommended primary model, fallback, prompt form, and iteration strategy for every shot.
- Mandatory stop checks for conflicting references, risky brand/geographic details, incompatible video endpoints, premature expensive generation, and bloated prompts.
- No automatic history search, generation, transformation, variation, or upscaling.
- Any action that may consume credits requires separate explanation and authorization.

## Quick start

1. Keep this entire `cinematic-prompting` folder together.
2. Open [START-HERE.md](START-HERE.md) and follow the section for your AI platform.
3. Give the assistant your idea, brief, script, shot list, references, or existing output.
4. If useful, copy [Project-Brief-Template.md](templates/Project-Brief-Template.md) and fill in only what you already know.

A simple first message is enough:

> Use the cinematic-prompting workflow. Here is what I am trying to create. Guide me through the missing decisions and do not write production prompts until I approve the Prompt Readiness Summary.

## Where to look next

- [START-HERE.md](START-HERE.md) — complete beginner walkthrough and glossary.
- [Cross-Platform-Setup.md](Cross-Platform-Setup.md) — Codex, Claude, and other-platform setup.
- [Worked Example](examples/Worked-Example_Static-to-Video.md) — a simplified project from brief to final video prompt.
- [Project Brief Template](templates/Project-Brief-Template.md) — optional form for organizing what you know.
- [Generic Chat Starter](platforms/Generic-Chat-Starter.md) — copyable starter for file-aware AI chats.

The workflow is platform-neutral. Its instructions belong to you and can be used for personal or professional work wherever compatible AI assistants can read the files.
