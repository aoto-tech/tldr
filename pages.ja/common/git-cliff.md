# git cliff

> 高度にカスタマイズ可能な変更履歴ジェネレーター。
> 詳細情報: <https://git-cliff.org/docs/usage/args/>。

- Gitリポジトリのすべてのコミットから変更履歴を生成し、`CHANGELOG.md` に保存する:

`git cliff > {{CHANGELOG.md}}`

- 最新のタグ以降のコミットから変更履歴を生成し、`stdout` に出力する:

`git cliff {{[-l|--latest]}}`

- 現在のタグに属するコミットから変更履歴を生成する (事前にタグを `git checkout` する):

`git cliff --current`

- タグに属していないコミットから変更履歴を生成する:

`git cliff {{[-u|--unreleased]}}`

- 既定の設定ファイルを現在のディレクトリの `cliff.toml` に書き込む:

`git cliff {{[-i|--init]}}`
