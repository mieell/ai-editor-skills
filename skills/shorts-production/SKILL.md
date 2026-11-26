---
name: shorts-production
description: Script, storyboard, generate keyframes for, or animate Shorts for doomv12, Flipbook, and Timeline Anomalies. Use for shot planning, ImageGen, Google Flow, or local comic animation.
---

# Shorts production

1. Start with a concrete hook and payoff. Lock dialogue or voiceover timing before expensive animation. Map each beat to a shot with start and end times, framing, action, story-critical props, and the state carried into the next shot.
2. Develop the look from the user's approved references. Keep character proportions, wardrobe, prop ownership, facing, and screen direction consistent. For a reveal or change in ownership, plan the starting pose, visible transition, and ending state. Use an insert or reaction when it makes the transition clearer.
3. Pick the channel workflow below. For a stills request, deliver numbered keyframes in timeline order. For motion, inspect the source and finished clips against the shot list. Explain any substitution and identify beats absent from the deliverable.
4. Cut to the dialogue, add captions and sound in the edit, and visibly check the hook, action transitions, and final hold. Use the project's existing export conventions.

## doomv12

- Default to vertical 1080 × 1920 and a 35–52 second episode when the brief leaves those choices open. Open with the theory or feat in the first three seconds. For lore, anchor each main claim to a verifiable comic or film moment and signal where original speculation begins.
- Use ImageGen to generate full-bleed PNG keyframes. Match the established flat cel shading, crisp outlines, and recognizable designs. Simplify staging, keep glow restrained, and leave space for captions. Match framing and pose between start and end frames when the animation needs a specific landing point.
- In Google Flow, animate action that changes the story, typically the hook and payoff. Use timed stills, push-ins, or parallax for explanation. Generate additional moving shots when the user's shot list calls for them. When the user specifies ImageGen only, deliver image assets.
- If Flow credits are unavailable, keep completed clips and use the existing HyperFrames + GSAP articulated SVG workflow for character action or Skia/Python for illustrated parallax. In the AI Editor workspace, use `channels/doomv12/spiderman-doom-short/README.md` and `channels/doomv12/doomv-doomsday-prediction/BLUEPRINT.md` as local implementation references. Reuse the approved script, timing, and compatible art.

## Flipbook

- **2D Animated Stories:** Build each shot as a full-bleed HyperFrames scene with a defined place, props, support surfaces, and coordinated character motion. Use look-development mockups as references for the local rigs by default.
- **3D Tactile Clay-Vinyl Diorama + AE Finishing:** Build smooth rounded polymer-clay/vinyl rigs and miniature sets in Blender 5.2+ EEVEE (`AgX - Punchy`, shallow tilt-shift DoF, zero Roblox blocks), inspect a 6-shot 3D look-dev proof sheet before rendering animated clips (15 fps stop-motion on twos encoded to 30 fps H.264 with `-g 30`), and finish in HyperFrames + GSAP with After Effects-grade whip-pans, impact flashes, damped camera shakes, animated live story HUDs, kinetic callouts, and color-coded captions.
- **Strict Quoted-Only Lip-Sync Gate:** Never drive on-screen character mouth movement from narrator voiceover lines. Keep character mouths cleanly closed (smiling, frowning, reacting silently via eyes/brows/hands) during all narrator lines, and open/animate lip-sync mouths strictly on the exact millisecond timestamps of quoted dialogue spoken by that on-screen character.
- Check contact sheets for missing props, floating objects, facing/occlusion errors, unintended lip-sync, and caption overlap before export.

## Timeline Anomalies

Use articulated SVG rigs in one HyperFrames + GSAP stage. Favor vertical 1080 × 1920 at 60 fps and natural-speed dialogue with room for reveals and reactions. Show the canon feats and signature defenses that explain the outcome. Keep labels limited to dialogue and speaker identifiers.
