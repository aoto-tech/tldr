# jj git

> `jj` リポジトリに対して Git 関連のコマンドを実行します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git>。

- 新しい Git ベースのリポジトリを作成します:

`jj git init`

- Git リポジトリのクローンを基にした新しいリポジトリを作成します:

`jj git clone {{source}}`

- Git リモートからフェッチします:

`jj git fetch`

- 追跡されたすべてのブックマークを Git リモートにプッシュします:

`jj git push`

- 指定されたブックマークを Git リモートにプッシュします:

`jj git push {{[-b|--bookmark]}} {{bookmark}}`
