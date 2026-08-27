# Magnific Reference Node Bindings

## Purpose

Use this file whenever an available image may be used as a reference in a Magnific prompt or reference slot. It prevents prompts from pointing to the wrong node and keeps reference use intentional rather than automatic.

## Reference availability check

Before the Prompt Readiness Summary, ask whether a usable reference image exists for the shot or batch. Show these paths:

1. **Use the image:** assign what it should control and bind it in Magnific.
2. **Do not use it:** preserve the current direction without that reference.
3. **Review first:** inspect the image's usefulness, conflicts, and likely role before deciding.
4. **No image available:** continue without a reference or identify what kind of reference would materially help.

An available image is not automatically a good reference. Evaluate whether it supports identity, product fidelity, wardrobe, location, composition, pose, lighting, palette, texture, camera behavior, or another approved job without importing unwanted traits.

## Mandatory node-name check

If the user chooses to use an image in Magnific:

- ask whether it is already present in the relevant Magnific canvas, workflow, or node graph;
- ask the user to copy the exact node name as it appears in Magnific;
- record the image, exact node name, assigned job, priority, and any traits that must not transfer;
- preserve spelling, capitalization, spaces, punctuation, and numbering exactly;
- never guess the node name from a filename, upload label, visual description, or earlier project shorthand;
- do not write a copy-ready prompt containing that reference until the exact node name is resolved.

If the image has not yet been uploaded, mark the node name as pending. The user may upload and name it, choose not to use it, or authorize a different reference strategy. Do not place placeholders such as `@reference`, `@image1`, or `@TBD` in a production prompt.

## Prompt and settings compilation

- When the active Magnific interface supports prompt mentions, use the exact confirmed node name in the interface-recognized `@` token, such as `@ExactNodeName` when that is the accepted representation.
- If Magnific presents autocomplete or a structured mention, tell the user to select the node that exactly matches the confirmed name rather than relying on plain text alone.
- If the active mode binds the image through a dedicated reference, start-frame, or end-frame control, place the exact node assignment in the Magnific settings card. Do not add a redundant `@` mention unless the mode genuinely uses both.
- When several images are used, bind each separately and state which visual property each controls. Do not let one reference silently override another.
- If a node is renamed, update every affected prompt and settings card before generation.

This check is a prompt-authoring requirement and does not depend on an MCP connection. It does not authorize uploading, generating, editing, or transforming media.
