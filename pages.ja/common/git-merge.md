# git merge

> ブランチをマージする。
> 詳細情報: <https://git-scm.com/docs/git-merge>。

- 指定したブランチを現在のブランチへマージする:

`git merge {{branch_name1 branch_name2 ...}}`

- マージメッセージを編集する:

`git merge {{[-e|--edit]}} {{branch_name}}`

- ブランチをマージし、マージコミットを作成する:

`git merge --no-ff {{branch_name}}`

- コミットを作成せずに、ブランチのマージ結果をステージする:

`git merge --squash {{branch_name}}`

- コンフリクトが発生した場合にマージを中止する:

`git merge --abort`

- 指定した戦略を使ってマージする:

`git merge {{[-s|--strategy]}} {{strategy}} {{[-X|--strategy-option]}} {{strategy_option}} {{branch_name}}`
