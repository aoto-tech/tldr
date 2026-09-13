# jj git fetch

> Git リモートからフェッチし、リモート リポジトリからオブジェクトと参照をダウンロードします。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-git-fetch>。

- デフォルトのリモート リポジトリから最新の変更を取得します:

`jj git fetch`

- 指定されたリモート リポジトリから最新の変更を取得します:

`jj git fetch --remote {{remote}}`

- 指定されたブランチからのみ最新の変更をフェッチします:

`jj git fetch {{[-b|--branch]}} {{branch}}`

- すべてのリモートから最新の変更を取得します:

`jj git fetch --all-remote`
