# Cinematic Prompting Agent

A personal, reusable AI-assisted directing workflow for developing high-quality images and single-shot video clips.

You do not need to know how to code, write technical prompts, name camera movements, or build an AI agent. Bring a rough idea, a script, a shot list, a reference image, or an output that is not working. The workflow helps you make the creative decisions first and writes the production prompts only after you approve them.

It is designed around Magnific workflows using image models such as Seedream and Nano Banana and video models such as Seedance and Kling, while keeping the underlying creative decisions platform-neutral.

## What is this for?

Image and video models can create attractive results quickly, but they often make important decisions on their own: the mood becomes generic, locations look empty, characters change, references are misused, or camera movement is left to chance.

This agent helps you direct those decisions deliberately. It can:

- turn a loose idea into a visual direction;
- research relevant things to show and propose a shot list;
- break down a script into practical shots;
- offer composition, lens, lighting, and camera-movement options;
- recommend a primary model, fallback model, prompt format, reference plan, and cost-conscious iteration strategy for each shot;
- translate an informal camera idea into clear movement instructions;
- write still-image prompts for approved start and end frames;
- write one continuous video-shot prompt after the stills are approved;
- keep characters, products, locations, wardrobe, lighting, and style consistent;
- bind Magnific image references to their exact node names;
- review generated outputs and recommend focused repairs;
- help reduce the polished-but-generic “AI look.”

It can be used for personal work, client projects, agency assignments, experiments, music videos, branded content, short films, social content, product imagery, or visual development.

## A simple example

You might begin with:

> I need a warm, accessible image of three friends having dinner in a good restaurant. It should feel energetic but not staged.

Instead of immediately producing a generic prompt, the agent helps decide:

- who the image is for and what it should communicate;
- whether a brand color should appear;
- how busy and lived-in the restaurant should feel;
- whether the camera is intimate at table height or more observational;
- which lens, focus, lighting, and composition support the mood;
- whether you have a useful reference image;
- what that reference should control and its exact Magnific node name;
- whether the complete shot specification is ready for prompt writing.

Only after you approve those decisions does it produce the copy-ready prompt.

## What can I give it?

Start with whatever you have:

- **Only a topic:** “A visual piece about the first direct flight between two cities.”
- **A rough visual idea:** “A runner crosses an empty-looking street, but I want the city to feel genuinely active.”
- **A script:** Ask it to identify beats, research visual opportunities, and propose coverage.
- **A complete shot list:** Ask it to preserve the shots and develop each one technically.
- **A reference image:** Ask whether it is useful for identity, product, composition, lighting, palette, texture, or another specific role.
- **A generated result:** Ask it to diagnose why the image or motion feels artificial and recommend the smallest repair.
- **A camera idea in ordinary language:** “Move closer and to the right while focus shifts to the object in front.”

You do not need to fill every field before starting. The agent is designed to identify missing decisions, explain your options, recommend a direction, and wait at important approval points.

## How the workflow behaves

The usual sequence is:

1. Understand the brief, audience, deliverables, mood, references, and constraints.
2. Ask whether exact brand colors should be incorporated.
3. Establish and approve the creative direction.
4. Research and propose a shot list when you do not yet know what to show.
5. Develop each shot's composition, lens, lighting, focus, occupancy, and camera intention.
6. Recommend the model, prompt form, reference plan, fallback, risks, and iteration/cost strategy.
7. Check for useful reference images and confirm exact Magnific node names for the ones you choose to use.
8. Present a Prompt Readiness Summary and ask for authorization.
9. Write the still prompt only after approval.
10. Generate and approve the start image; create an end image when the landing frame needs control.
11. Confirm the final camera, focus choreography, and video-model strategy.
12. Write one continuous video-shot prompt after separate video authorization.
13. Review the result, repair problems, and keep only intentional changes in continuity.

The amount of discussion scales with the project. One simple image can move quickly. A campaign, manifesto, or multi-shot film gets a production bible and more structured approvals.

## Important defaults

- Still images come before video prompts.
- One generated video clip contains one continuous camera shot, without baked-in cuts.
- The agent does not write production prompts until the relevant decisions are approved.
- Public, social, travel, hospitality, workplace, and commercial locations feel plausibly lived-in unless intentional emptiness is requested.
- References receive defined jobs instead of vaguely influencing everything.
- Model and prompt-format choices are recommended per shot instead of being treated as one fixed project-wide default.
- After repeated similar failures, the workflow stops adding instructions and recommends a cleaner reset, reference repair, model change, shot split, or post-production solution.
- A selected Magnific reference uses the exact node name shown in Magnific; the agent never invents `@image1` or another placeholder.
- Read-only history review is optional.
- Generation, editing, transformation, variation, upscaling, or other credit-consuming actions require separate approval.

## Start using it in Codex cloud

1. Connect this GitHub repository to Codex.
2. Create or select a cloud environment using the repository's default branch.
3. Start a cloud chat in that environment.
4. Send your topic, brief, script, shot list, reference, or generated output.
5. Invoke `$cinematic-prompting` explicitly when desired. Matching requests may also activate it automatically.

Example first message:

> Use `$cinematic-prompting`. I have a 30-second product film with a rough script but no shot list. Help me establish the visual direction, research possible imagery, and propose the shots. Do not write generation prompts until the workflow reaches its approval gate.

No local copy is required for Codex cloud chats. Only changes committed and pushed to this repository are available to newly started cloud environments.

## Use it with Claude or another AI platform

Download the current ZIP from [`Releases/`](Releases/) and keep the folder structure intact. The package contains platform-neutral instructions plus setup help for Claude and general file-aware AI assistants.

Begin with:

- [`README.md`](.agents/skills/cinematic-prompting/README.md) inside the portable package;
- [`START-HERE.md`](.agents/skills/cinematic-prompting/START-HERE.md) for a complete beginner walkthrough;
- [`Cross-Platform-Setup.md`](.agents/skills/cinematic-prompting/Cross-Platform-Setup.md) for installation choices.

## Magnific connection

The prompting workflow and a Magnific account connection are separate. The agent can write prompts without any connection.

When a session has read-only Magnific access, it may offer to retrieve a selected generation for review. If no connection is available, upload the result manually or provide a usable link. The agent must not search history automatically or perform a paid operation without your approval.

## Where everything lives

- `.agents/skills/cinematic-prompting/` — portable agent and documentation;
- `AGENTS.md` — routes matching Codex cloud tasks to the agent;
- `Projects/` — optional location for project reports;
- `Releases/` — current portable ZIP;
- `Releases/Outdated/` — previous versions.

For the most detailed beginner explanation, continue to [Start Here](.agents/skills/cinematic-prompting/START-HERE.md).
