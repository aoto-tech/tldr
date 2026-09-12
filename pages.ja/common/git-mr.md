# git mr

> GitLabのマージリクエストをローカルにチェックアウトする。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-mr>。

- 指定したマージリクエストをチェックアウトする:

`git mr {{マージリクエスト番号}}`

- 指定したリモートからマージリクエストをチェックアウトする:

`git mr {{マージリクエスト番号}} {{リモート}}`

- URLからマージリクエストをチェックアウトする:

`git mr {{URL}}`

- 古いマージリクエストのブランチを消去する:

`git mr clean`
