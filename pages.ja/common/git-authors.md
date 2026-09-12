# git authors

> Gitリポジトリのコミッター一覧を生成する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-authors>。

- コミッターの完全な一覧を `AUTHORS` ファイルではなく `stdout` に出力する:

`git authors {{[-l|--list]}}`

- コミッター一覧を `AUTHORS` ファイルに追記し、既定のエディターで開く:

`git authors`

- メールアドレスを除いたコミッター一覧を `AUTHORS` ファイルに追記し、既定のエディターで開く:

`git authors --no-email`
