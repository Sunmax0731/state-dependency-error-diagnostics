# インストールガイド

## Closed Alpha Package

1. GitHub Release `v0.1.0-alpha.1` から assets を取得する。
2. `dist/state-dependency-error-diagnostics-docs.zip` を展開して README と manual-test を確認する。
3. repo を clone する場合:

```powershell
git clone https://github.com/Sunmax0731/state-dependency-error-diagnostics.git
cd state-dependency-error-diagnostics
npm test
```

## Host Setup

1. 作業ディレクトリ `D:\AI\BlenderAddon\state-dependency-error-diagnostics` で `npm test` を実行します。
2. Blender を起動し、Preferences > Add-ons > Install から `src/blender/__init__.py` を含むフォルダを読み込みます。
3. 3D View のサイドバーでアドオンパネルを開き、代表シナリオ相当の入力を確認します。

