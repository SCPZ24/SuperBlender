---
name: cinematic-blender
description: Operating guide for blender-mcp. Use it to create, rework, or improve Blender scenes, cinematography, animation, lighting, materials, and models.
---

# Cinematic Blender

## Core principles

- Prioritize quality: Favor the quality of the imagery or model over build speed. Produce masterful, production-grade work. Avoid assembling scenes from combinations of simple primitives such as spheres and cubes.

- Build the full scene: Unless the user explicitly requests an isolated model or deliberate negative space, design every camera-visible area, including the horizon, sky or enclosure, and distant backdrop. Fill it with geometry, materials, backgrounds, and other assets. Do not be overly conservative with computing resources.

- Validate visually: Do not rely only on code or component checks. Use blender-mcp screenshots to inspect the entire frame; reject large black or featureless areas unless intentional, and confirm that the subject, backdrop, lighting, and colors form a coherent composition.

- Finish the design before building: Define the following first:
    1. Visual style
    2. Scene layout, including foreground, midground, and backdrop
    3. Camera design
    4. Lighting design
    5. Material design
  Only then begin modeling in Blender. If the user provides these specifications, use them directly. Otherwise, design them first or use a question tool to align with the user's requirements.

## Workflow

### 1. Generate visual references

Diffusion models are generally better than VLMs at generating visual references that people find convincing.
If an image-generation tool is available, such as GPT Image 2, give it the requirements and generate reference images first. Use them to make better decisions about scene composition, lighting, materials, and style.

### 2. Research before modeling

- Before designing, use search tools to study the real-world appearance, structure, and materials of the target object.

- Before building, search BlenderKit, Poly Haven, and Sketchfab for usable public models, materials, textures, HDRIs, decals, animations, and Geometry Nodes resources.

### 3. Create assets one at a time

Create any required assets that you could not find and download.
Never create all assets in a single pass. Build them one at a time and ensure that each asset meets the design requirements.
If your harness supports multiple agents, delegate generously to subagents.

Render and inspect each completed batch of assets. Revise anything that fails review.

### 4. Implement the design

Implement the planned scene layout, camera design, lighting design, and material design in Blender.

To produce masterful work, do not be overly conservative with tokens or the user's computing resources. Do not over-optimize for minimalism or rendering speed.

### 5. Inspect renders and deliver

Capture multiple screenshots of the scene and verify that they meet the design requirements.
If they do not, return to the scene and revise it.

After the work passes inspection, show the user every captured screenshot. A final production render takes substantial time, so do not produce one unless the user explicitly requests it.

## Anti-patterns

- First remove any default materials, lights, and other undesigned defaults.

- Do not use a flat World background, glow, fog, particles, or a light cone as a substitute for a finished backdrop.

- If the user requests an animation, distribute motion throughout the entire timeline. Avoid long periods of stillness before the next movement.

- For animations, account for how moving objects affect the surrounding scene. For example, an explosion's shockwave should push nearby objects outward and shake the camera; a fast-moving object should generate airflow that makes nearby lightweight objects sway.