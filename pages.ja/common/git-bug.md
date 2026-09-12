# git bug

> Gitの内部ストレージを使用する分散型バグトラッカー。プロジェクトにファイルを追加しない。
> コミットやブランチと同じように、共同作業で使用するGitリモートへ問題を送信できる。
> 詳細情報: <https://github.com/git-bug/git-bug/blob/master/doc/md/git-bug.md>。

- 新しいIDを作成する:

`git bug user create`

- 新しいバグを作成する:

`git bug add`

- 新しいバグ項目をリモートへプッシュする:

`git bug push`

- 更新をプルする:

`git bug pull`

- 既存のバグを一覧表示する:

`git bug ls`

- クエリを使用してバグを絞り込み、並べ替える:

`git bug ls "{{状態}}:{{open}} {{並べ替え}}:{{edit}}"`

- 本文の内容からバグを検索する:

`git bug ls "{{検索クエリ}}" baz`
