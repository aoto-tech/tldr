# jj revert

> 指定されたリビジョンの逆を適用します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-revert>。

- 指定されたリビジョンセット (`B::D`、`A..D`、`B|C|D` など) で指定されたリビジョンの逆を適用します:

`jj revert {{[-r|--revisions]}} {{revsets}}`

- 指定したリビジョンの上に反転を適用します:

`jj revert {{[-r|--revisions]}} {{revsets}} {{[-d|--destination]}} {{revsets}}`

- 指定したリビジョンの前または後に逆を適用します:

`jj revert {{[-r|--revisions]}} {{revsets}} {{[-B|--insert-before]}} {{revsets}} {{[-A|--insert-after]}} {{revsets}}`
