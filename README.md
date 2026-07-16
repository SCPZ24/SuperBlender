# SuperBlender

**A 65-line skill that pushes Blender MCP agents beyond rough primitives and into richly modeled, fully staged, cinematic Blender work.**

> **Read this in:** English · [日本語](README_JP.md) · [简体中文](README_ZH.md)

## Made for Blender MCP

SuperBlender is a companion skill for [Blender MCP](https://github.com/ahujasid/blender-mcp), the open-source bridge that lets AI agents control Blender. Blender MCP provides the tools; SuperBlender gives the agent a production-minded way to use them—so it keeps designing, building, inspecting, and refining until the result feels like a detailed Blender set piece rather than a quick collection of primitives.

## See the Difference

Each pair compares a direct Blender MCP run with a run enhanced by SuperBlender.

<table>
  <thead>
    <tr>
      <th width="50%" align="center">Raw · Without SuperBlender</th>
      <th width="50%" align="center">Enhanced · With SuperBlender</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/raw_artificial_sun.mp4"><img src="assets/raw_artificial_sun.gif" alt="Raw Artificial Sun animation without SuperBlender" width="100%"></a><br>
        <sub><a href="assets/raw_artificial_sun.mp4">Play the full raw MP4</a></sub>
      </td>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/enhanced_artificial_sun.mp4"><img src="assets/enhanced_artificial_sun.gif" alt="Enhanced Artificial Sun animation made with SuperBlender" width="100%"></a><br>
        <sub><a href="assets/enhanced_artificial_sun.mp4">Play the full enhanced MP4</a></sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/raw_whale.mp4"><img src="assets/raw_whale.gif" alt="Raw Whale animation without SuperBlender" width="100%"></a><br>
        <sub><a href="assets/raw_whale.mp4">Play the full raw MP4</a></sub>
      </td>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/enhanced_whale.mp4"><img src="assets/enhanced_whale.gif" alt="Enhanced Whale animation made with SuperBlender" width="100%"></a><br>
        <sub><a href="assets/enhanced_whale.mp4">Play the full enhanced MP4</a></sub>
      </td>
    </tr>
  </tbody>
</table>

The table uses lightweight animated previews for reliable playback inside GitHub. Select any preview to open the original full-resolution MP4.

## How It Works

SuperBlender adds no geometry and writes no Blender code by itself. It changes the agent's creative loop: plan the visual style, full scene, camera, lighting, and materials before modeling; research references and reusable assets; build and review assets in focused batches; then inspect multiple full-frame screenshots and revise. It also rejects shortcuts such as untouched defaults, empty backgrounds, primitive-only construction, static stretches of animation, or visual effects used in place of an actually designed environment. That persistent attention to composition, context, motion, and finish is what turns a technically complete scene into a meticulously crafted Blender production.

## Contributions Welcome

Contributions are warmly welcome. Improve the existing [`cinematic-blender` skill](skills/cinematic-blender/SKILL.md), or add a new focused skill under [`skills/`](skills/). Please keep additions concise, actionable, and grounded in real Blender MCP workflows.
