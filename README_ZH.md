# SuperBlender

**一个仅65行的Skill，让使用Blender MCP的Agent告别粗糙的基础几何体堆砌，创作出建模细致、场景完整、富有电影感的Blender大作。**

> **其他语言:** [English](README.md) · [日本語](README_JP.md) · 简体中文

## 为Blender MCP而生

SuperBlender是[Blender MCP](https://github.com/ahujasid/blender-mcp)的配套Skill；后者是一个让AI Agent控制Blender的开源桥梁。Blender MCP提供工具，SuperBlender则教Agent以更接近专业制作的方式使用这些工具——持续设计、构建、检查和打磨，直到作品不再是匆忙拼出的基础几何体，而是细节丰富、镜头完整、经得起观看的Blender场景。

## 效果对比

每组分别展示直接使用Blender MCP的结果，以及加载SuperBlender之后的增强结果。

<table>
  <thead>
    <tr>
      <th width="50%" align="center">Raw · 未使用SuperBlender</th>
      <th width="50%" align="center">Enhanced · 使用SuperBlender</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/raw_artificial_sun.mp4"><img src="assets/raw_artificial_sun.gif" alt="未使用SuperBlender制作的Artificial Sun Raw动画" width="100%"></a><br>
        <sub><a href="assets/raw_artificial_sun.mp4">播放完整Raw MP4</a></sub>
      </td>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/enhanced_artificial_sun.mp4"><img src="assets/enhanced_artificial_sun.gif" alt="使用SuperBlender制作的Artificial Sun Enhanced动画" width="100%"></a><br>
        <sub><a href="assets/enhanced_artificial_sun.mp4">播放完整Enhanced MP4</a></sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/raw_whale.mp4"><img src="assets/raw_whale.gif" alt="未使用SuperBlender制作的Whale Raw动画" width="100%"></a><br>
        <sub><a href="assets/raw_whale.mp4">播放完整Raw MP4</a></sub>
      </td>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/enhanced_whale.mp4"><img src="assets/enhanced_whale.gif" alt="使用SuperBlender制作的Whale Enhanced动画" width="100%"></a><br>
        <sub><a href="assets/enhanced_whale.mp4">播放完整Enhanced MP4</a></sub>
      </td>
    </tr>
  </tbody>
</table>

为确保在GitHub中稳定播放，表格使用轻量的动态预览；点击任意预览即可播放原始的全分辨率MP4。

## 原理

SuperBlender本身不提供几何模型，也不直接编写Blender代码；它改变的是Agent的创作循环。Agent会在建模前先设计视觉风格、完整场景、镜头、灯光和材质，研究真实参考与可复用资产，分批创建并检查每项资产，最后通过多张完整画面的截图进行视觉验收和返工。它还明确拒绝一些常见捷径，例如保留未经设计的默认项、留下空洞背景、只用基础几何体拼装、让动画长时间静止，或用雾、辉光等特效替代真正设计过的环境。正是这种对构图、空间、运动与完成度的持续打磨，让“技术上完成”升级为真正细致的Blender大作。

## 欢迎贡献

欢迎参与贡献：你可以改进现有的[`cinematic-blender` Skill](skills/cinematic-blender/SKILL.md)，也可以在[`skills/`](skills/)下新增更专注的Skill。请让每项改动保持简洁、可执行，并建立在真实的Blender MCP工作流之上。
