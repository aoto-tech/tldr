# git graft

> あるブランチのコミットを別のブランチへマージし、元のブランチを削除する。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-graft>。

- 元のブランチにあり対象ブランチにないすべてのコミットを対象ブランチへマージし、元のブランチを削除する:

`git graft {{元のブランチ}} {{対象ブランチ}}`
