# git flow

> 高レベルなリポジトリ操作を提供するGit拡張機能集。
> 詳細情報: <https://github.com/nvie/gitflow>。

- 既存のGitリポジトリ内で初期化する:

`git flow init`

- `develop` を基点とする機能ブランチで開発を開始する:

`git flow feature start {{機能}}`

- 機能ブランチでの開発を完了し、`develop` ブランチへマージして削除する:

`git flow feature finish {{機能}}`

- 機能をリモートサーバーへ公開する:

`git flow feature publish {{機能}}`

- 別のユーザーが公開した機能を取得する:

`git flow feature pull origin {{機能}}`
