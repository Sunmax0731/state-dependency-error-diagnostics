# 要件定義

## 目的

状態可視化・依存関係・エラー診断 は、Blenderでシーン状態、依存、エラーを追う制作者 が シーン状態、依存関係、ログ、エラー候補を収集し、次の修復アクションへつなげる。

## Source

- PICKUP Rank: 57
- Domain / Idea No: BlenderAddon / 1
- Repository: state-dependency-error-diagnostics
- created_idea: `D:/AI/BlenderAddon/created_idea_001_state-dependency-error-diagnostics`
- ZIP: `D:/AI/BlenderAddon/created_idea_001_state-dependency-error-diagnostics/idea_001_state-dependency-error-diagnostics.zip`
- README確認: 開始時点では正式 repo が存在しないため、README.md は存在しない。

## Functional Requirements

- R1: sceneName、dependencyName、status、repairHint を必須項目として検査する。
- R2: 必須項目不足は fail として分類する。
- R3: `externalLinkMissing` が true の場合は warning として分類し、手動確認理由を返す。
- R4: 複数アイテムの mixed-batch を pass / warning / fail に集計する。
- R5: 結果を CLI と docs/release evidence で再利用できる形にする。

## Non Functional Requirements

- UTF-8 で Markdown / JSON / JS / HTML / Python を保存する。
- 外部通信を既定で行わず、サンプルとローカル入力だけで検証できる。
- 手動テスト未実施であることを release 前 docs に明記する。

