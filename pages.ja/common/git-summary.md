# git summary

> Gitリポジトリに関する情報を表示する。
> `git-extras` の一部。
> 詳細情報: <https://manned.org/git-summary>。

- Gitリポジトリに関するデータを表示する:

`git summary`

- 指定したコミット、ブランチ、タグ以降のGitリポジトリに関するデータを表示する:

`git summary {{コミット|ブランチ名|タグ名}}`

- 異なるメールアドレスのコミッターを作成者ごとに1つの統計へまとめて、Gitリポジトリに関するデータを表示する:

`git summary --dedup-by-email`

- 各貢献者が変更した行数を含む、Gitリポジトリに関するデータを表示する:

`git summary --line`
