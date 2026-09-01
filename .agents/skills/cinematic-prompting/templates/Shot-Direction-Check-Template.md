# Per-Shot Direction Check Template

Use this before writing the first static prompt for a shot. Read `references/Model-and-Prompt-Strategy.md` and recommend a strategy rather than asking the user to choose without guidance.

## Shot context

- Scene ID / Shot ID:
- Narrative purpose:
- Purpose in the final edit:
- Emotional beat:
- Approved base style or sequence override:
- Expected duration, if video:

## Direction path

Choose one: user-described; agent proposes two or three options; or hybrid.

## Static viewpoint check

- Shot size/composition:
- Camera height/angle:
- Lens/perspective behavior:
- Subject placement:
- Foreground/midground/background:
- Background occupancy and secondary action:
- Approved reason for intentional emptiness, if applicable:
- Depth of field and initial focus plane:
- How this viewpoint expresses the mood and shot purpose:

## Video movement check

Complete only for video shots.

- Support/stability:
- Start frame:
- Three-dimensional path and orientation:
- Pan/tilt/roll/orbit/tracking behavior:
- Optical zoom:
- Framing evolution/parallax:
- Focus target A -> target B, cue, speed, landing, and hold:
- Timing/easing:
- End frame:
- Endpoint compatibility: clear / blocked by:
- Generation difficulty/risk:

## Model & Prompt Strategy Card

- Primary model/mode and why:
- Fallback and pivot condition:
- Prompt form and why: labeled natural prose / change-preserve-reference / object-by-object structured / master-plus-delta / concise motion
- Reference plan: exact candidate -> one assigned job and priority:
- Traits that must not transfer:
- Iteration/cost plan:
- Principal risks:
- Live capability or credit check required:
- Stop status: clear / blocked by which mandatory check:

## Agent recommendation

- Recommended direction:
- Why it fits:
- What it makes the audience feel or notice:
- Simplest fallback if generation struggles:

## Reference-image choice

- Is a usable image available for this shot?
- Decision: use / leave unused / review first / none available
- Selected reference and assigned job:
- Traits that must not transfer:
- Exact Magnific node name, if selected for use:
- Binding method: `@` mention / dedicated reference setting / start or end setting / other
- Binding resolved before Prompt Readiness Summary: yes / no

## Approval

- Approved direction and strategy:
- Requested changes:
- Date/version:

Approval here confirms direction and model/prompt strategy but does not authorize copy-ready prompt drafting. Continue to `Prompt-Readiness-and-Authorization-Template.md`.
