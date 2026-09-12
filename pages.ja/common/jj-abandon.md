# jj abandon

> リビジョンを破棄し、子孫をその親にリベースします。
> リビジョンを破棄すると、関連付けられている変更 ID が削除されます。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-abandon>。

- 指定されたリビジョンセット (`B::D`、`A..D`、`B|C|D` など) で指定されたリビジョンを破棄します:

`jj abandon {{revsets}}`

- リビジョンを放棄し、ブックマークを削除せずに親リビジョンに移動します:

`jj abandon --retain-bookmarks {{revsets}}`

- 子の内容を変更せずにリビジョンを破棄します:

`jj abandon --restore-descendants {{revsets}}`
