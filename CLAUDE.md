# Claude / AI Agent Operation Guide

このリポジトリは personal-knowledge です。
GitHub Pages で公開している個人ブログ・生活ナレッジサイトです。

## 最重要ルール

このサイトは Jekyll や Markdown 変換を使っていません。
GitHub Pages では HTML ファイルを直接公開しています。

そのため、公開記事の正本は .html です。

- .md だけを作成・更新してはいけない
- .md だけを更新してもWebには反映されない
- 公開記事を作成・更新する場合は、必ずカテゴリ配下の .html を編集する
- 新規記事を追加する場合は、必要に応じて index.html の記事一覧リンクも更新する

## サイト構成

ルートに以下がある。

- index.html
- style.css
- README.md
- CLAUDE.md

カテゴリ配下に記事HTMLがある。

例:

- life/*.html
- travel/*.html
- reading/*.html
- detox/*.html
- fashion/*.html
- finance/*.html
- photography/*.html
- walk/*.html

## Markdownの扱い

.md は公開記事ではなく、下書き・原稿・メモ扱いとする。

- 下書きは drafts/ に置く
- カテゴリ配下に .md を置かない
- 公開する場合は .html に変換してカテゴリ配下へ置く

## 作業前に必ず確認すること

PowerShellで以下を確認する。

- git status --short
- Get-ChildItem -Recurse -File -Include *.html | Where-Object { $_.FullName -notmatch "\\.git\\" }
- Get-ChildItem -Recurse -File -Include *.md | Where-Object { $_.FullName -notmatch "\\.git\\" }

## 作業後に必ず確認すること

PowerShellで以下を確認する。

- git status --short
- git diff

確認ポイント:

- 意図した .html が更新されているか
- .md だけの更新になっていないか
- 新規記事の場合、index.html にリンクを追加したか
- 文字化けしていないか
- 不要な一時ファイルを作っていないか

## 禁止事項

- Jekyll化しない
- _config.yml を勝手に作らない
- _layouts, _includes, _posts を勝手に作らない
- GitHub Actions を勝手に追加しない
- package.json やビルド環境を勝手に追加しない
- Markdownだけで記事を完成扱いにしない
- サイト全体の構造変更を勝手に行わない

## 基本方針

このサイトでは、凝った静的サイトジェネレータよりも、事故りにくいHTML直管理を優先する。
目的はサイト基盤の高度化ではなく、生活・旅行・読書・デジタルデトックス・買い物判断などの記録を安定して残すことである。
