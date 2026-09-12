# git imerge

> 2つのGitブランチ間でマージまたはリベースを段階的に実行する。
> 競合解決を簡単にするため、ブランチ間の競合を個々のコミットの組み合わせまで追跡する。
> 詳細情報: <https://github.com/mhagger/git-imerge>。

- imergeによるリベースを開始する (先にリベースするブランチをチェックアウトする):

`git imerge rebase {{リベース先ブランチ}}`

- imergeによるマージを開始する (先にマージ先ブランチをチェックアウトする):

`git imerge merge {{マージするブランチ}}`

- 進行中のマージまたはリベースをASCII図で表示する:

`git imerge diagram`

- 競合を解決した後、imerge操作を続行する (先に競合したファイルを `git add` する):

`git imerge continue --no-edit`

- すべての競合を解決した後、imerge操作を完了する:

`git imerge finish`

- imerge操作を中止し、直前のブランチへ戻る:

`git imerge remove && git checkout {{直前のブランチ}}`
