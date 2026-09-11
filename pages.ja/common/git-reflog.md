# git reflog

> `HEAD`、ブランチ、タグなどのローカル参照に対する変更履歴を表示する。
> 詳細情報: <https://git-scm.com/docs/git-reflog>。

- `HEAD` の reflog を表示する:

`git reflog`

- 指定したブランチの reflog を表示する:

`git reflog {{branch_name}}`

- reflog の最新5件だけを表示する:

`git reflog {{[-n|--max-count]}} 5`
