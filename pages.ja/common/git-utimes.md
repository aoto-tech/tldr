# git utimes

> ファイルの更新日時を最終コミット日時へ変更する。作業ツリーまたはインデックスにあるファイルは変更しない。
> `git-extras` の一部。
> 詳細情報: <https://github.com/tj/git-extras/blob/main/Commands.md#git-utimes>。

- すべてのファイルの更新日時を最終コミット日時へ変更する:

`git utimes`

- 最終コミット日時より新しいファイルの更新日時を変更し、ローカルリポジトリからコミットされたファイルの元の更新日時を保持する:

`git utimes --newer`
