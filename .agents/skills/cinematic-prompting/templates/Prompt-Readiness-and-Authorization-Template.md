# Prompt Readiness and Authorization Template

Use this gate before copy-ready prompt drafting. Do not place generation prompts in the authorization request.

## Static Prompt Readiness Summary

### Scope

- Shot IDs or batch:
- Prompt type: start image / end image / both

### Approved shot specification

- Purpose and emotional beat:
- Subject and action:
- Continuity state:
- Shot size and composition:
- Camera position, height, and angle:
- Lens/perspective behavior:
- Aspect ratio:
- Foreground/midground/background and visual hierarchy:
- Lived-in occupancy and secondary human/environmental activity, or approved empty-space exception:
- Production design, wardrobe, and props:
- Lighting, palette, approved brand hex use, texture, and grade:
- Depth of field and focus:
- Start state:
- End state:
- Separate end image required and why:
- References and assigned roles:
- Target image model/mode and output requirements:
- Video movement concept the static frame must support:
- Material risks:
- Assumptions or recommended defaults:
- Unresolved conflicts:

### Authorization request

> Approve this specification and authorize static prompt drafting for [shot IDs or batch]?

Options:

- Approve and authorize the named scope.
- Request changes to specific fields.
- Authorize only selected ready shots.
- Hold and revisit an earlier decision.

- User response:
- Authorized scope:
- Date/version:

## Video Prompt Readiness Summary

### Scope

- Shot IDs or batch:
- Approved start image IDs:
- Approved end image IDs:

### Approved motion specification

- Support/stability:
- Camera path:
- Orientation and framing evolution:
- Lens operation:
- Focus choreography:
- Subject motion:
- Environmental motion:
- Duration, timing, and easing:
- Settle and landing frame:
- Target video model/mode:
- Changes caused by the approved static images:
- Material risks:
- Assumptions or recommended defaults:
- Unresolved conflicts:

### Authorization request

> Approve this motion specification and authorize the final video prompt for [shot IDs or batch]?

Options:

- Approve and authorize the named scope.
- Request changes to the movement, focus, timing, or landing.
- Authorize only selected ready shots.
- Simplify the move or return to static-frame repair.

- User response:
- Authorized scope:
- Date/version:
