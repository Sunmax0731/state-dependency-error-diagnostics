# 状態可視化・依存関係・エラー診断

state-dependency-error-diagnostics は Blenderでシーン状態、依存、エラーを追う制作者 向けの closed alpha プロダクトです。シーン状態、依存関係、ログ、エラー候補を収集し、次の修復アクションへつなげる。

## Source

- PICKUP Rank: 57
- Domain / Idea No: BlenderAddon / 1
- Repository: state-dependency-error-diagnostics
- 主な公開先: GitHub Release / BOOTH
- created_idea: `D:/AI/BlenderAddon/created_idea_001_state-dependency-error-diagnostics`
- 同梱ZIP: `D:/AI/BlenderAddon/created_idea_001_state-dependency-error-diagnostics/idea_001_state-dependency-error-diagnostics.zip`
- 開始時 README: 存在しない


## Alpha Scope

- 代表シナリオ4件の自動検証
- 必須項目不足、警告、混在バッチの分類
- src/blender/ のホスト連携シェル
- QCDS、security/privacy、traceability、release checklist、manual test docs
- docs ZIP: `dist/state-dependency-error-diagnostics-docs.zip`

## Commands

```powershell
npm test
node src/cli/index.js samples/representative-suite.json
npm run build:docs
```

手動テストは Codex 側では未実施です。手順は `docs/manual-test.md` と `docs/strict-manual-test-addendum.md` にあります。

