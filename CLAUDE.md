# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Git運用ルール

- コードに変更を加えたら、そのたびにコミットしてGitHubリモート（`origin`）にプッシュすること。
- 変更を未プッシュのまま放置しない。

## デプロイ先

https://mikioujio-gif.github.io/task-board/

## 技術スタック

- React 18 + Vite（`@vitejs/plugin-react`）
- JavaScript（JSX）。TypeScriptは未導入
- スタイリングはプレーンCSS（`App.css`）
- 状態管理はReactの`useState`/`useEffect`のみ
- データ永続化はブラウザの`localStorage`
- GitHub Actionsで`main`へのpush時に自動ビルド・GitHub Pagesへデプロイ

## コンポーネントの命名規約

- コンポーネント名はPascalCase、ファイル名もコンポーネント名に合わせる（例: `App` → `App.jsx`）
- イベントハンドラ・状態更新関数はcamelCaseの動詞＋名詞（例: `addTask`, `toggleTask`, `deleteTask`）
- CSSクラス名はkebab-case（例: `task-form`, `task-list`, `delete-button`）
