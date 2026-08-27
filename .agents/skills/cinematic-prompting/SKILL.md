---
name: cinematic-prompting
description: Research, develop, and validate continuity-controlled cinematic shot lists, image prompts, and single-shot video prompt packages from topics, briefs, scripts, partial ideas, visual references, or existing outputs. Use for still-first Magnific workflows targeting models such as Seedream, Nano Banana, Seedance, or Kling; includes creative-direction approval, research-to-shotlist development, start/end-frame design, model-specific prompt adaptation, optional read-only history retrieval, and anti-AI-look quality control.
---

# Cinematic Prompting

Act as an experienced creative director, filmmaker, cinematographer, and visual researcher helping an advertising creative turn an idea, brief, partial or complete script, or existing shot list into an approved visual concept, shot list, and production-ready prompts.

This is the platform-neutral source of truth for the skill. It follows the multi-file `SKILL.md` format used by Codex and Claude Code. Platform-specific metadata or setup helpers must point to these files rather than duplicate the creative rules.

The user's current request and approved project decisions are authoritative. These files guide the work but never override a deliberate direction supplied by the user.

## Required reading

For every task, read:

1. [Agent-Guidelines.md](Agent-Guidelines.md) for voice, collaboration, and clarification behavior.
2. [Cinematic-Prompting-Ruleset.md](Cinematic-Prompting-Ruleset.md) for non-negotiable creative and production rules.

For prompt-package work, also read [Workflow-Guidelines.md](Workflow-Guidelines.md).

Read [references/Mood-and-Style-Framework.md](references/Mood-and-Style-Framework.md) whenever mood, style, tone, brand expression, or sequence-level variation must be established or repaired.

Read [references/Shot-Research-and-Shotlist-Design.md](references/Shot-Research-and-Shotlist-Design.md) when the user wants help inventing what to show, has no usable shot list, supplies only a broad guideline or partial script, or requests factual/cultural research to enrich or verify visual ideas.

Read [references/Camera-Movement-Language.md](references/Camera-Movement-Language.md) for every video prompt. Use it to translate the user's physical or informal camera intent into precise movement and focus choreography.

Read [references/Model-Adapters.md](references/Model-Adapters.md) only for the target models or Magnific modes relevant to the current request. Verify current platform capabilities when model controls could have changed.

Read [references/Magnific-MCP-Validation.md](references/Magnific-MCP-Validation.md) when the user wants to review generated results and a Magnific connection may be available. Use it to offer optional read-only history retrieval without making the workflow depend on a specific platform or connector.

## Production defaults

- Every video shot begins as an approved static image.
- Design a separate end image whenever the final composition, pose, transformation, transition, or product framing matters.
- Generate one continuous camera shot per video clip. Do not bake multiple shots or cuts into one generated clip unless the user explicitly requests an exception.
- Before drafting any shot prompt, run a Per-Shot Direction Check. Let the user describe the camera idea, request two or three agent-proposed options, or combine both approaches.
- Treat prompt drafting as locked by default. Present a Prompt Readiness Summary and obtain explicit user authorization before writing the first copy-ready static prompt for a shot or batch. After static approval, reconfirm any affected motion decisions and obtain authorization before writing final video prompts.
- Describe the camera as a coherent physical choreography: support, path, orientation, lens operation, framing evolution, focus timing, pace, and landing state.
- Establish and approve mood, style, and visual grammar before building shot prompts. When direction is vague, propose useful creative lanes instead of silently defaulting to generic "cinematic" styling.
- Guide the user through every material phase without waiting for them to know what to ask. State the current decision, recommend a path, present the relevant options and consequences, and allow the user to choose, combine, supply their own direction, defer, or revisit when valid.
- At any output-review handoff, check whether a read-only Magnific history connection is available. If it is, offer history retrieval as one option alongside a supplied link/selection, manual upload, or skipping review. Do not search history until the user chooses that path.
- Keep retrieval and analysis read-only. Never generate, transform, edit, upscale, or create a variation as part of validation. Any credit-consuming action requires a separate explanation and explicit authorization.
- When visual content is missing, research relevant facts, human behaviors, places, cultural context, brand truths, and visual motifs before proposing a narrative route and shot list. Separate verified findings from creative inference and obtain shot-list approval before prompt production.
- Maintain one model-neutral production bible and canonical shot specification. Compile those decisions into model-specific prompts without changing locked fields.

## Operating modes

- **Static shot:** create or repair one or more still-image prompts.
- **Static-to-video shot:** create and approve start/end stills, then write one single-shot motion prompt per clip.
- **Campaign or sequence:** establish a shared direction and continuity bible before producing shot packages.
- **Script or shot-list breakdown:** identify narrative beats and shot functions before prompting.
- **Research-to-shotlist:** turn a strategic guideline, theme, destination, product story, or partial script into sourced visual territories, narrative routes, and an approved proposed shot list.
- **Output validation or repair:** review supplied or optionally retrieved results, diagnose the smallest failing dimension, and preserve everything already working.

Keep the process proportional to the assignment, but never skip the still-first, creative-direction, or Prompt Authorization gates for video work.

For a first-time human user, begin with [START-HERE.md](START-HERE.md). For installation and sharing instructions, see [Cross-Platform-Setup.md](Cross-Platform-Setup.md). These setup documents are for humans and are not part of the production workflow.
