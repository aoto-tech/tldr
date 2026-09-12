# git changelog

> リポジトリのコミットとタグから変更履歴レポートを生成する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-changelog>。

- 既存のファイルを更新するか、最新のGitタグ以降のコミットメッセージを含む `History.md` を作成する:

`git changelog`

- 現在のバージョンのコミットを一覧表示する:

`git changelog {{[-l|--list]}}`

- `2.1.0` タグから現在までのコミットを一覧表示する:

`git changelog {{[-l|--list]}} {{[-s|--start-tag]}} 2.1.0`

- `0.5.0` タグから `1.0.0` タグまでのコミットを整形して一覧表示する:

`git changelog {{[-s|--start-tag]}} 0.5.0 {{[-f|--final-tag]}} 1.0.0`

- `0b97430` コミットから `1.0.0` タグまでのコミットを整形して一覧表示する:

`git changelog --start-commit 0b97430 {{[-f|--final-tag]}} 1.0.0`

- 出力ファイルとして `CHANGELOG.md` を指定する:

`git changelog CHANGELOG.md`

- 現在の変更履歴ファイルの内容をすべて置き換える:

`git changelog {{[-p|--prune-old]}}`
