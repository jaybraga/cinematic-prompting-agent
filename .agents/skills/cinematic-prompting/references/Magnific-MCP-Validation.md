# Magnific MCP Validation

## Purpose

Use this reference only when generated outputs need review and the current AI platform may have a Magnific MCP, connector, or equivalent account integration. It defines an optional read-only acquisition path; it does not make Magnific access mandatory and does not authorize generation.

## Capability check

At the beginning of a static or video QC handoff, inspect the tools or connected services already available in the current session. Look specifically for read-only capabilities equivalent to:

- search or list creation history;
- retrieve one creation by link, selection, or identifier;
- read prompt/model/settings metadata;
- access a preview or full-resolution result;
- read account balance or operation cost when relevant.

Do not claim that a connection is active merely because Magnific is mentioned in the project. If no usable connection is available, continue with manual upload or a user-supplied link/file.

## Guided choice before retrieval

Do not search history automatically. Present a compact choice at the review handoff:

```text
CURRENT STEP — Output selection for validation
Decision: How should I access the generated result?
Recommendation: [best path based on the active capabilities and why]

Your options:
A. Magnific history — search recent creations read-only, show likely matches, and let you select.
B. Direct selection — give me a Magnific creation link or identify the result already shown.
C. Manual upload — attach the image/video file or start/end frames.
D. Skip validation for now — continue only where the workflow safely allows it.

Retrieval and critique do not generate or transform media. I will request separate approval before any action that could consume Magnific credits.
```

If the connector is unavailable, omit option A and say why in one sentence. Always allow the user to describe another route.

## Read-only retrieval procedure

After the user chooses Magnific history:

1. Search only the scope needed: recent history, a tool type, date range, or prompt fragment when supported.
2. Present a short candidate list using human-readable information such as thumbnail, date/time, media type, model/mode, dimensions/duration, and a shortened prompt. Avoid exposing internal identifiers unless the user needs them.
3. Let the user choose the exact result or map each result to a shot ID. Do not silently assume that the newest creation belongs to the current shot.
4. Retrieve the selected preview or full-resolution output and the metadata required for review.
5. Record the source, creation link or stable reference, model/mode, prompt version when available, settings, date, and assigned shot ID in the revision/generation log.

For start/end-frame workflows, retrieve and label both endpoints separately. For video, retrieve the clip when supported; otherwise ask for a playable file or enough representative frames to perform an honest review and state any limitation.

## Credit and authorization boundary

Read-only history search, creation lookup, metadata access, and result retrieval do not normally consume Magnific generation credits. Verify the current connector's description or reported cost if it exposes that information; platform or assistant usage may still be counted separately from Magnific credits.

The following are not validation-only actions and must never be called implicitly:

- image or video generation;
- edits, transforms, variations, or relighting;
- upscaling or enhancement;
- extending, interpolating, or repairing a clip through Magnific;
- any operation described by the connector as credit-consuming or paid.

Before one of those actions, state the exact operation, selected source, expected output, known credit cost or uncertainty, and whether the connector reports that unlimited mode applies. Obtain a separate explicit authorization naming the operation and scope. Prompt Authorization alone does not authorize an MCP generation call.

## Validation pass

Compare the retrieved output with the approved production bible, canonical shot specification, reference assignments, and acceptance criteria. Review only dimensions relevant to the result:

- mood, visual thesis, and shot function;
- identity, product, wardrobe, prop, location, and continuity fidelity;
- composition, viewpoint, blocking, depth, focus, and visual hierarchy;
- lighting direction, palette, materials, texture, reflections, shadows, typography, logos, hands, and topology;
- start/end compatibility and plausible motion path;
- for video: camera path, framing evolution, focus choreography, performance, physics, temporal stability, duration, and landing frame;
- anti-AI-look failures and any accidental drift.

Classify the result as:

- **Accepted:** meets the visible criteria and may update the approved continuity state.
- **Repairable:** the core shot works; identify the smallest correction while preserving successful dimensions.
- **Rejected:** the result conflicts with a locked decision or has failures that make local repair inefficient.

End with guided options appropriate to the finding: accept, request prompt-only repair instructions, upload another result, retrieve another history candidate, change a reference or model strategy, use post-production, redesign the shot, or stop. Regeneration may be discussed, but it remains a separate credit-consuming action requiring explicit authorization.
