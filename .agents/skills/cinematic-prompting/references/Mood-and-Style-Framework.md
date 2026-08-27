# Mood and Style Framework

## Purpose

Use this framework to turn subjective direction into concrete production choices. It owns the definition and fallback process for mood/style; other files should only invoke the gate.

## Distinguish the layers

- **Mood:** what the audience should feel during and immediately after the piece.
- **Style:** the visual and sonic system used to create that feeling.
- **Tone:** the attitude the brand or story takes toward the audience.
- **Production treatment:** the practical combination of design, performance, camera, light, texture, movement, and post decisions used to execute the style.

Do not substitute one layer for another. "Premium" is not a complete mood, and "ARRI with anamorphic lenses" is not a complete style.

## Brand-color check

At the beginning of every project, ask whether an exact brand hex code or defined palette should be incorporated. The user may supply codes, ask the agent to derive a palette from brand guidelines or references, or choose no locked brand color.

When a code is approved, translate it into an integration plan: decide whether it acts as a hero accent, recurring environmental echo, wardrobe or prop cue, practical-light note, product/UI color, or controlled grade relationship. Protect believable skin tones, material response, motivated light, and the natural identity of the location. If exact colorimetry is mandatory, plan a finishing or compositing check rather than promising perfect hex reproduction from generation alone.

## Direction dimensions

Define only the dimensions that materially shape the piece, but check all of them for contradictions:

1. **Emotional promise:** joyful, intimate, energetic, aspirational, reassuring, tense, mysterious, playful, quiet confidence, etc.
2. **Audience relationship:** inviting, peer-to-peer, authoritative, exclusive, irreverent, warm, ceremonial, observational.
3. **Realism level:** documentary, naturalistic commercial, heightened live action, stylized photorealism, graphic/illustrative, surreal.
4. **Narrative energy:** calm, measured, buoyant, chaotic, propulsive, suspenseful, contemplative.
5. **World and production design:** location character, scale, materials, cleanliness, plausible occupancy, background human activity, density, props, wardrobe, graphic language.
6. **Palette and light:** approved brand hex codes and their assigned roles, dominant hues, saturation, contrast, source motivation, softness, time of day, highlight/shadow character.
7. **Human performance:** candid, restrained, aspirational, comic, tactile, choreographed, spontaneous, intimate.
8. **Composition and optics:** graphic versus observational framing, distance, perspective, depth, lens character, focus strategy, negative space.
9. **Texture and finishing:** clean digital, tactile naturalism, filmic grain, diffusion, halation, sharpness, color treatment, controlled imperfections.
10. **Motion, edit, and sound:** camera support, movement energy, focus behavior, clip duration, cutting rhythm, ambience, dialogue, music, and sound design.

## When the brief is clear

Return one Direction Check that translates the user's words and references across the relevant dimensions. Include a short `This should feel like...` sentence and a short `This should not become...` sentence.

Ask for correction only when the translation introduces a meaningful interpretation the user has not already approved.

## When the brief is vague

Propose two or three materially different lanes. Put the strongest recommendation first.

Each lane must include:

- a concise name;
- emotional promise and audience reading;
- visual thesis;
- palette and lighting logic;
- production design and material language;
- performance energy;
- composition, optics, texture, movement, and pacing;
- what to avoid;
- why it fits the assignment.

The options must differ in creative logic, not merely color temperature or lens choice. Ask the user to select one, combine specific dimensions, or redirect them.

## Brand-category examples are prompts for questions, not presets

A happy and accessible gaming piece might use legible silhouettes, expressive performance, buoyant movement, clear color separation, tactile environments, and inviting social energy. It could also take a quieter or more cinematic approach if the campaign requires it.

A premium airline-class piece might use controlled compositions, quiet confidence, refined human gestures, tactile materials, motivated pools of light, measured movement, and restrained finishing. It could also be bright, celebratory, or culturally specific if that better serves the brief.

Never infer the final direction from `gaming`, `premium`, `Supercell`, `GOL`, or `INSIGNIA` alone. Use the category to formulate better options and questions.

## Reference decomposition

For every important reference, state which dimensions it governs:

- story or emotional tone;
- composition or camera distance;
- lens and depth behavior;
- lighting and color;
- production design, wardrobe, or materials;
- movement, performance, or pacing;
- texture, grade, or finishing.

Avoid relying only on a film, campaign, photographer, director, or artist name. Translate the reference into observable traits that can be approved and prompted.

## Continuity and intentional variation

Store one approved base `style_id` for the piece. When a scene needs a different mood or scenario, create a named `sequence_override` that states:

- what changes;
- what remains locked;
- why the change serves the narrative;
- how the piece returns to or evolves from the base system.

This preserves authorship without forcing every shot into an identical mood.
