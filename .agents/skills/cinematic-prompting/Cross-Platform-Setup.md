# Cross-Platform Setup

If you have never used an AI assistant or this workflow before, read `START-HERE.md` first. This file covers installation and platform-specific setup.

## Purpose

This package uses one shared set of creative instructions across Codex, Claude Code, Claude Projects, and other file-aware assistants. Do not fork the rules by platform.

The portable source of truth is:

- `SKILL.md` — entrypoint, routing, and essential defaults;
- `Agent-Guidelines.md` — professional stance and collaboration behavior;
- `Cinematic-Prompting-Ruleset.md` — non-negotiable production rules;
- `Workflow-Guidelines.md` — chronological process and deliverable structure;
- `references/` — mood/style, Shot Research, camera movement, model-specific guidance, and optional Magnific history validation.

The `agents/openai.yaml` file is optional OpenAI/Codex interface metadata. Other platforms can ignore it.

## Optional Magnific connection

The workflow does not require a Magnific MCP or connector. When the current AI platform has an authenticated integration that exposes read-only creation history, the agent can offer to search recent results and retrieve a selected image or video for QC. The user may always choose a direct creation link/current selection or upload files manually instead.

Connections and available operations differ by platform and account. The agent must detect actual capabilities at runtime, wait before searching account history, and keep retrieval separate from generation. Read-only search/retrieval does not normally consume Magnific generation credits; generation, editing, transformation, variations, upscaling, and video creation require a separate cost or credit explanation and explicit authorization. An unlimited Magnific plan must not be assumed to apply through a connector.

## Codex

Copy the complete `cinematic-prompting` folder to your personal Codex skills directory:

```text
~/.codex/skills/cinematic-prompting/
```

Keep the directory structure intact. Invoke it explicitly as `$cinematic-prompting`, or let Codex select it automatically when the request matches its description.

For a shared project-specific installation, use the skill location supported by that Codex workspace or distribute the same folder through your team's normal plugin/skill mechanism.

## Claude Code

Claude Code supports multi-file `SKILL.md` packages using the Agent Skills open standard. Copy the same folder without rewriting it.

Personal installation, available across projects:

```text
~/.claude/skills/cinematic-prompting/
```

Project installation, shared with a team:

```text
<project>/.claude/skills/cinematic-prompting/
```

Invoke it as `/cinematic-prompting`, or let Claude load it automatically when the request matches the description.

A separate `CLAUDE.md` is intentionally not required for the skill. Claude Code reads `SKILL.md` natively and loads skills on demand; duplicating the full workflow in `CLAUDE.md` would create maintenance drift and consume context in every session.

Official Claude Code skill documentation: <https://code.claude.com/docs/en/slash-commands>

## Claude Projects on claude.ai

Claude Projects use project knowledge and project instructions rather than a local skills directory.

1. Create or open a Claude Project.
2. Upload `SKILL.md`, the three core Markdown files, and the five files under `references/` to Project Knowledge. Also upload `START-HERE.md`, `templates/`, and `examples/` when you want the beginner guide and reusable forms available inside the project.
3. Open `platforms/Claude-Project-Instructions.md` from this package.
4. Copy its contents into **Set project instructions**.
5. Start a new project chat and provide a topic, brief, references, script, or shot list.

The project instructions are deliberately short. They direct Claude to retrieve the shared core files instead of maintaining a second version of the creative rules.

Official Claude Projects documentation: <https://support.anthropic.com/en/articles/9519177-how-can-i-create-and-manage-projects>

## Claude chat or another file-aware assistant

When a platform does not support installable skills:

1. Attach `SKILL.md` and the core/reference files relevant to the task.
2. Start with: `Use the attached cinematic-prompting SKILL.md as the governing workflow for this task. Read the files it routes to before producing prompts.`
3. Keep the folder/file names unchanged so references remain easy to resolve.

If you are unsure what to write first, copy the message from `platforms/Generic-Chat-Starter.md` and then fill in `templates/Project-Brief-Template.md`.

For a quick static-only task, the minimum useful set is:

- `SKILL.md`;
- `Agent-Guidelines.md`;
- `Cinematic-Prompting-Ruleset.md`;
- `Workflow-Guidelines.md`;
- `references/Mood-and-Style-Framework.md`;
- the relevant section of `references/Model-Adapters.md`.

For any video task, also include `references/Camera-Movement-Language.md`.

For research-to-shotlist work, also include `references/Shot-Research-and-Shotlist-Design.md` and, when useful, `templates/Shot-Research-Template.md`.

## Team distribution

Share the entire package or its versioned ZIP. Do not send coworkers only one supporting file, because the workflow relies on explicit routing and separated responsibilities.

When updating the workflow:

1. Edit the shared core or reference file that owns the rule.
2. Keep `SKILL.md`, `agents/openai.yaml`, and `platforms/Claude-Project-Instructions.md` as thin adapters.
3. Validate the skill.
4. increment the package version and redistribute the full folder or ZIP.
