# Strict Manual Test Addendum

Codex 側では手動テスト未実施です。

## 作業ディレクトリ

`D:\AI\BlenderAddon\state-dependency-error-diagnostics`

## 必要ファイル

- `samples/representative-suite.json`
- `src/product-profile/profile.json`
- `src/blender/`
- `docs/manual-test.md`
- `dist/state-dependency-error-diagnostics-docs.zip`

## セットアップ手順

1. 作業ディレクトリ `D:\AI\BlenderAddon\state-dependency-error-diagnostics` で `npm test` を実行します。
2. Blender を起動し、Preferences > Add-ons > Install から `src/blender/__init__.py` を含むフォルダを読み込みます。
3. 3D View のサイドバーでアドオンパネルを開き、代表シナリオ相当の入力を確認します。

## ローカルサーバーやホストアプリ起動手順

Blenderを起動し、アドオンをインストールして有効化する。

## 実施手順

1. `npm test` を再実行する。
2. 実データ1件を `samples/representative-suite.json` と同じ形式で作成する。
3. CLIで検証する。
4. ホストUIまたは補助UIで表示する。
5. warning と fail の理由がユーザーに説明可能か確認する。

## 期待結果

- 自動テストが通る。
- docs ZIP が存在する。
- 実ホストまたは補助UIで最低1件の結果を確認できる。
- 未確認項目が release notes と一致する。

## 未実施の手動確認項目

- 実ホストUI表示
- 実素材/実ページ/実ファイルでの検査
- 配布導線のユーザー環境確認
- ストア/BOOTH向けスクリーンショット確認

