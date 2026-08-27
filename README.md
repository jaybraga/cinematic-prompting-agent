# Cinematic Prompting Agent

Cloud-ready source for the DRUID cinematic image and video prompting workflow.

The reusable skill lives at:

`/.agents/skills/cinematic-prompting/`

Codex automatically discovers repository-scoped skills from `.agents/skills`. The root `AGENTS.md` routes relevant cloud chats to this workflow and protects its approval gates.

## Use in Codex cloud

1. Connect this private GitHub repository to Codex.
2. Create a cloud environment using this repository and its default branch.
3. Start a cloud chat in that environment.
4. Provide a topic, brief, script, shot list, references, or existing generated output.
5. Invoke the workflow explicitly with `$cinematic-prompting` when desired. Matching requests may also activate it automatically.

No local copy is required for cloud chats. The repository is the shared source of truth across computers. Only committed and pushed changes are available to a newly started cloud environment.

## Magnific connection

The agent workflow and the Magnific account connection are separate. When a cloud chat has read-only Magnific access, the agent offers history retrieval as one validation option. When it does not, upload the selected output or provide a usable link. Generation, editing, transformation, variation, upscaling, and video creation always require separate authorization and credit disclosure.

## Package documentation

Beginner and cross-platform documentation is inside the skill folder:

- `START-HERE.md`
- `Cross-Platform-Setup.md`
- `platforms/Claude-Project-Instructions.md`
- `platforms/Generic-Chat-Starter.md`

Versioned ZIP packages are stored under `Releases/`, with previous releases under `Releases/Outdated/`.

## Updating the workflow

Edit the source under `.agents/skills/cinematic-prompting/`, validate the skill, commit the changes, and push them to GitHub. Prefer a branch and pull request when coworkers are contributing.
