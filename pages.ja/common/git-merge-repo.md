# git merge-repo

> 2つのリポジトリの履歴をマージする。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-merge-repo>。

- リポジトリのブランチを現在のリポジトリのディレクトリへマージする:

`git merge-repo {{リポジトリへのパス}} {{ブランチ名}} {{ディレクトリ/サブディレクトリ}}`

- リモートリポジトリのブランチを、履歴を保持せずに現在のリポジトリのディレクトリへマージする:

`git merge-repo {{リモートリポジトリへのパス}} {{ブランチ名}} .`
