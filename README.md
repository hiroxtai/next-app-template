# Next.js App Template

[Next.js](https://nextjs.org) をベースにしたモダンな Web アプリケーションテンプレートです。

## 技術スタック

- **フレームワーク**: [Next.js 16](https://nextjs.org) (App Router)
- **言語**: [TypeScript](https://www.typescriptlang.org)
- **パッケージマネージャー**: [pnpm](https://pnpm.io)
- **スタイリング**: [Tailwind CSS v4](https://tailwindcss.com)
- **リンター/フォーマッター**: [Biome](https://biomejs.dev)
- **コンパイラ**: [React Compiler](https://react.dev/learn/react-compiler)

## プロジェクト構成

```
next-app-template/
├── .devcontainer/          # Dev Container 設定
├── .vscode/                # VS Code 設定
│   ├── extensions.json     # 推奨拡張機能
│   ├── launch.json         # デバッグ設定
│   └── settings.json       # エディター設定
├── public/                 # 静的ファイル
├── src/
│   └── app/                # App Router
│       ├── globals.css     # グローバルスタイル
│       ├── layout.tsx      # ルートレイアウト
│       └── page.tsx        # トップページ
├── biome.json              # Biome 設定
├── next.config.ts          # Next.js 設定
├── postcss.config.mjs      # PostCSS 設定
└── tsconfig.json           # TypeScript 設定
```

## 開発環境のセットアップ

### ローカル環境

1. 依存関係のインストール:

```bash
pnpm install
```

2. 開発サーバーの起動:

```bash
pnpm dev
```

3. ブラウザで [http://localhost:3000](http://localhost:3000) を開く

### Dev Container

VS Code の Dev Container 機能を使用して、統一された開発環境で作業できます。

1. VS Code で拡張機能 [Dev Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) をインストール
2. プロジェクトを開く
3. コマンドパレット (`Cmd+Shift+P`) から `Dev Containers: Reopen in Container` を選択

Dev Container には以下が含まれます:

- Node.js 22
- pnpm
- 推奨 VS Code 拡張機能の自動インストール
- 統一されたエディター設定

## スクリプト

```bash
# 開発サーバーの起動
pnpm dev

# プロダクションビルド
pnpm build

# プロダクションサーバーの起動
pnpm start

# コードのリント
pnpm lint

# コードのフォーマット
pnpm format
```

## VS Code 拡張機能

以下の拡張機能の使用を推奨します（Dev Container では自動インストールされます）:

- [Biome](https://marketplace.visualstudio.com/items?itemName=biomejs.biome) - リンター/フォーマッター
- [Tailwind CSS IntelliSense](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) - Tailwind CSS の補完
- [Auto Rename Tag](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag) - HTML/JSX タグの自動リネーム
- [Path Intellisense](https://marketplace.visualstudio.com/items?itemName=christian-kohler.path-intellisense) - ファイルパスの補完
- [Code Spell Checker](https://marketplace.visualstudio.com/items?itemName=streetsidesoftware.code-spell-checker) - スペルチェック

## デバッグ

VS Code のデバッグ機能を使用できます:

- **Next.js: debug server-side** - サーバーサイドのデバッグ
- **Next.js: debug client-side** - クライアントサイドのデバッグ（Chrome）
- **Next.js: debug full stack** - フルスタックデバッグ

## コード規約

- **フォーマット**: Biome による自動フォーマット（保存時に実行）
- **インポート**: 自動整理（保存時に実行）
- **インデント**: 2 スペース
- **Import Alias**: `@/*` で `src/` を参照

## 参考リソース

- [Next.js Documentation](https://nextjs.org/docs) - Next.js の機能と API
- [React Documentation](https://react.dev) - React の公式ドキュメント
- [Tailwind CSS Documentation](https://tailwindcss.com/docs) - Tailwind CSS の使い方
- [Biome Documentation](https://biomejs.dev) - Biome の設定方法
- [TypeScript Documentation](https://www.typescriptlang.org/docs) - TypeScript ガイド

## デプロイ

### Vercel

最も簡単な方法は [Vercel Platform](https://vercel.com/new) を使用することです。

詳細は [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) を参照してください。

## ライセンス

MIT
