# \# Personal Knowledge

# 

# 自分が実際に体験して学んだことを、未来の自分が見返せる形で整理する公開ナレッジベースです。

# 

# \## Categories

# 

# \- travel: 旅行で学んだこと

# \- detox: デジタルデトックス

# \- github: GitHub / Issue運用

# \- ai: ChatGPT・AI活用

# \- finance: 家計・固定費・自動化ログ


## サイト運用ルール

このサイトは GitHub Pages で公開している静的HTMLサイトです。

現時点では Jekyll や Markdown からの自動HTML変換は使用していません。
そのため、Webに公開される記事は各カテゴリ配下の `.html` ファイルです。

### 基本方針

- 公開記事は `.html` を正とする
- `.md` は下書き・原稿・メモ扱いとする
- `.md` だけを更新してもWebには反映されない
- 新規記事を公開する場合は、カテゴリ配下に `.html` を作成する
- 必要に応じて `index.html` の記事一覧リンクも更新する
- AIエージェントに作業させる場合も、MarkdownではなくHTMLを更新対象にする

### 下書きの扱い

下書きや原稿メモは `drafts/` 配下に置く。
カテゴリ配下に `.md` を置くと、公開記事と誤認しやすいため避ける。

### 作業確認

作業後は必ず以下を確認する。

```powershell
git status --short
git diff

公開記事を追加・更新した場合は、対象の .html と index.html の差分を確認してから commit / push する。


## サイト運用ルール

このサイトは GitHub Pages で公開している静的HTMLサイトです。

現時点では Jekyll や Markdown からの自動HTML変換は使用していません。
そのため、Webに公開される記事は各カテゴリ配下の .html ファイルです。

### 基本方針

- 公開記事は .html を正とする
- .md は下書き・原稿・メモ扱いとする
- .md だけを更新してもWebには反映されない
- 新規記事を公開する場合は、カテゴリ配下に .html を作成する
- 必要に応じて index.html の記事一覧リンクも更新する
- AIエージェントに作業させる場合も、MarkdownではなくHTMLを更新対象にする

### 下書きの扱い

下書きや原稿メモは drafts/ 配下に置く。
カテゴリ配下に .md を置くと、公開記事と誤認しやすいため避ける。

### 作業確認

作業後は必ず以下を確認する。

- git status --short
- git diff

公開記事を追加・更新した場合は、対象の .html と index.html の差分を確認してから commit / push する。

