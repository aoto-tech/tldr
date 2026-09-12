# git obliterate

> Gitリポジトリからファイルを削除し、その履歴を消去する。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-obliterate>。

- 指定したファイルが存在した履歴を消去する:

`git obliterate {{ファイル1 ファイル2 ...}}`

- 2つのコミット間から、指定したファイルが存在した履歴を消去する:

`git obliterate {{ファイル1 ファイル2 ...}} -- {{コミットハッシュ1}}..{{コミットハッシュ2}}`
