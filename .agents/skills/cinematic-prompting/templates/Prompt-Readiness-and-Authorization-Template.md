# Prompt Readiness and Authorization Template

Use this gate before copy-ready prompt drafting. Do not place generation prompts in the authorization request. Re-run every mandatory stop check in `references/Model-and-Prompt-Strategy.md`.

## Static Prompt Readiness Summary

### Scope

- Shot IDs or batch:
- Prompt type: start image / end image / both

### Approved shot specification

- Purpose, emotional beat, subject, action, and continuity:
- Shot size, composition, camera position/height/angle, and lens behavior:
- Aspect ratio and safe area:
- Foreground/midground/background, occupancy, and visual hierarchy:
- Production design, wardrobe, and props:
- Lighting, palette, brand hex placement/material/prominence, texture, and grade:
- Depth of field and focus:
- Start state, end state, and separate-end-image decision:
- Video movement concept the endpoints must support:

### Model, prompt, and reference strategy

- Primary image model/mode and visible reason:
- Fallback and pivot condition:
- Prompt form and reason:
- Selected references, assigned jobs, priorities, and non-transfer traits:
- Exact Magnific node name and binding method for each selected reference:
- Output requirements and cost/iteration plan:
- Material risks:
- Mandatory stop checks: all clear / blocked by:
- Assumptions, defaults, deferred items, or unresolved conflicts:

### Authorization request

> Approve this specification and model/prompt strategy, and authorize static prompt drafting for [shot IDs or batch]?

Options: approve; request changes; choose the fallback; authorize a ready subset; or hold and revisit an earlier decision.

- User response:
- Authorized scope:
- Date/version:
## Video Prompt Readiness Summary

### Scope

- Shot IDs or batch:
- Approved start image IDs:
- Approved end image IDs:
- Exact node names and binding methods:

### Approved motion specification

- Support/stability and camera path:
- Orientation, framing evolution, and lens operation:
- Focus choreography:
- Subject and environmental motion:
- Duration, timing, easing, settle, and landing:
- Endpoint compatibility check:
- Changes caused by approved static images:

### Model and prompt strategy

- Primary video model/mode and visible reason:
- Fallback and pivot condition:
- Prompt form and reason:
- Reference jobs and dedicated start/end/additional slots:
- Output requirements and known credit consequence or uncertainty:
- Material risks:
- Mandatory stop checks: all clear / blocked by:
- Assumptions, defaults, or unresolved conflicts:

### Authorization request

> Approve this motion specification and model/prompt strategy, and authorize the final video prompt for [shot IDs or batch]?

Options: approve; request changes; choose the fallback; authorize a ready subset; simplify the move; or return to static repair.

- User response:
- Authorized scope:
- Date/version:
