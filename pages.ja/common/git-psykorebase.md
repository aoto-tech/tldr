# git psykorebase

> マージコミットを使用し、競合処理を1回だけ行って、あるブランチを別のブランチ上へリベースする。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-psykorebase>。

- マージコミットを使用し、競合処理を1回だけ行って、現在のブランチを別のブランチ上へリベースする:

`git psykorebase {{上流ブランチ}}`

- 競合を解決した後に続行する:

`git psykorebase --continue`

- リベースするブランチを指定する:

`git psykorebase {{上流ブランチ}} {{対象ブランチ}}`
