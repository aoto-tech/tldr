# jj diff

> 2 つのリビジョン間でファイルの内容を比較します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-diff>。

- 現在のリビジョンの変更を表示します:

`jj diff`

- 指定されたリビジョンセットの変更を表示します (例: `B::D`、`A..D`、`B|C|D` など):

`jj diff {{[-r|--revisions]}} {{revsets}}`

- 指定されたリビジョンから指定されたリビジョンへの変更を表示します:

`jj diff {{[-f|--from]}} {{from_revset}} {{[-t|--to]}} {{to_revset}}`

- 差分の統計を表示します:

`jj diff --stat`

- Git 形式の差分を表示します:

`jj diff --git`
