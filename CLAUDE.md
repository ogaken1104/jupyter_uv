# CLAUDE.md

## Language

- Think in English internally, but always respond in Japanese
- Code comments and variable names are in English
- Markdown cells in notebooks are written in Japanese

## MCP

- context7 を使ってライブラリのドキュメントを参照すること
- code-simplifier plugin を使い、冗長なコードを避けること

## Jupyter Notebook コーディング規約

### コードスタイル

- 不要な `print` 文を入れない（確認用の print は使い終わったら削除）
- コメントアウトしたコードを残さない（不要なら削除する）
- 1セルは短く保つ。1つの目的に1セル

### 変数管理

- 同じ変数の編集は1つのセルの中で完結させる（セルをまたいで同じ変数を上書きしない）
- DataFrame は `df_` プレフィックスをつける（例: `df_org`, `df_train`, `df_result`）

### ノートブック構成

- Markdown セルでセクションを区切る
- 記事用ノートブックは上から順に実行して再現できる状態を保つ
