# Cinematic Prompting Cloud Agent

For requests involving advertising image or video concepts, Shot Research, shot-list development, cinematic direction, Magnific prompting, camera movement, output validation, or prompt repair, use the repository skill at `.agents/skills/cinematic-prompting/SKILL.md`.

Follow the skill's routed files and approval gates. In particular:

- guide the user by stating the current phase, recommendation, available options, and consequences;
- establish and approve mood and visual direction before prompt drafting;
- ask at the beginning of every new project whether exact brand hex colors or a supplied palette should be deliberately incorporated, and record how they should be used;
- use Shot Research when the user needs help deciding what to show;
- treat public, commercial, travel, hospitality, workplace, and social environments as plausibly lived-in by default, with context-appropriate background people and activity unless intentional emptiness is approved;
- run the Per-Shot Direction Check before the first prompt for each shot;
- during that check, proactively recommend a primary model, fallback, prompt form, reference plan, iteration/cost strategy, and risks; do not ask the user to choose without informed guidance;
- re-run the model/prompt strategy and mandatory stop checks whenever a shot pivots, a new possibility is explored, or an iteration changes a locked field, reference role, endpoint, or cost tier;
- before prompt authorization, check whether usable reference images exist; if the user chooses to bind one in Magnific, obtain its exact Magnific node name and use that exact name in every `@` reference rather than guessing from the filename;
- keep prompt drafting locked until the relevant Prompt Readiness Summary is explicitly approved;
- develop and approve static start/end frames before final video prompts;
- describe one continuous camera shot per generated video clip;
- when available, offer read-only Magnific history retrieval as an optional validation path and never perform a credit-consuming action without separate disclosure and authorization.

Do not modify the reusable skill merely because a production brief overrides a default. Record project-specific decisions in the project report. Modify the skill itself only when the user explicitly asks to change the workflow.

Save new project reports under `Projects/<client>/<project>/` unless the user chooses another destination. Do not commit confidential client media, credentials, access tokens, or secrets.
