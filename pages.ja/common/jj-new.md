# jj new

> 新しい空の変更を作成します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-new>。

- 現在のリビジョンの上に新しい空の変更を作成します:

`jj new`

- 特定のリビジョンの上に新しい空の変更を作成します:

`jj new {{revision}}`

- 複数のリビジョンの上に新しいマージ変更を作成します:

`jj new {{revset1 revset2 ...}}`

- 指定されたリビジョン間に新しい空の変更を挿入します:

`jj new {{[-B|--insert-before]}} {{revsets}} {{[-A|--insert-after]}} {{revsets}}`
