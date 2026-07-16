# SuperBlender

**わずか65行で、Blender MCPを使うエージェントを単純なプリミティブの寄せ集めから、緻密に作り込まれたシネマティックなBlender作品へ導くSkillです。**

> **ほかの言語:** [English](README.md) · 日本語 · [简体中文](README_ZH.md)

## Blender MCPのためのSkill

SuperBlenderは、AIエージェントからBlenderを操作できるオープンソースの橋渡し役、[Blender MCP](https://github.com/ahujasid/blender-mcp)のためのコンパニオンSkillです。Blender MCPが操作ツールを提供し、SuperBlenderがその使い方を制作志向に変えます。エージェントは設計、構築、確認、改善を繰り返し、プリミティブを急いで並べただけのシーンではなく、細部まで意図の通ったBlenderの大作を目指します。

## 効果の比較

各ペアは、Blender MCPをそのまま使った結果と、SuperBlenderで強化した結果を比較しています。

<table>
  <thead>
    <tr>
      <th width="50%" align="center">Raw · SuperBlenderなし</th>
      <th width="50%" align="center">Enhanced · SuperBlenderあり</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/raw_artificial_sun.mp4"><img src="assets/raw_artificial_sun.gif" alt="SuperBlenderなしで制作したArtificial SunのRawアニメーション" width="100%"></a><br>
        <sub><a href="assets/raw_artificial_sun.mp4">Rawの完全版MP4を再生</a></sub>
      </td>
      <td align="center">
        <strong>Artificial Sun</strong><br><br>
        <a href="assets/enhanced_artificial_sun.mp4"><img src="assets/enhanced_artificial_sun.gif" alt="SuperBlenderで制作したArtificial SunのEnhancedアニメーション" width="100%"></a><br>
        <sub><a href="assets/enhanced_artificial_sun.mp4">Enhancedの完全版MP4を再生</a></sub>
      </td>
    </tr>
    <tr>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/raw_whale.mp4"><img src="assets/raw_whale.gif" alt="SuperBlenderなしで制作したWhaleのRawアニメーション" width="100%"></a><br>
        <sub><a href="assets/raw_whale.mp4">Rawの完全版MP4を再生</a></sub>
      </td>
      <td align="center">
        <strong>Whale</strong><br><br>
        <a href="assets/enhanced_whale.mp4"><img src="assets/enhanced_whale.gif" alt="SuperBlenderで制作したWhaleのEnhancedアニメーション" width="100%"></a><br>
        <sub><a href="assets/enhanced_whale.mp4">Enhancedの完全版MP4を再生</a></sub>
      </td>
    </tr>
  </tbody>
</table>

GitHub上で確実に再生できるよう、表内には軽量なアニメーションプレビューを表示しています。プレビューを選択すると、元のフル解像度MP4を再生できます。

## 仕組み

SuperBlender自体がジオメトリやBlenderコードを生成するわけではありません。代わりに、エージェントの制作ループを変えます。モデリング前にビジュアルスタイル、シーン全体、カメラ、照明、マテリアルを設計し、参考資料や再利用可能なアセットを調査します。アセットは小さな単位で制作・確認し、最後はフレーム全体を複数のスクリーンショットで検証して修正します。初期設定の放置、空の背景、プリミティブだけの造形、長く静止したままのアニメーション、設計済みの環境の代わりにエフェクトだけで埋める、といった近道も避けます。構図、空間、動き、仕上げを粘り強く磨くことで、「一応完成したシーン」を緻密なBlender作品へ引き上げます。

## コントリビューション歓迎

コントリビューションを歓迎します。既存の[`cinematic-blender` Skill](skills/cinematic-blender/SKILL.md)を改善することも、[`skills/`](skills/)以下に新しい専門Skillを追加することもできます。変更は簡潔かつ実行可能で、実際のBlender MCPワークフローに基づくものにしてください。
