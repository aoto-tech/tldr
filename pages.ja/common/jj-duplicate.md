# jj duplicate

> 既存のものと同じ内容で新しい変更を作成します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-duplicate>。

- 現在のリビジョンを既存の親に複製します:

`jj duplicate`

- 特定のリビジョンを既存の親に複製します:

`jj duplicate {{revset}}`

- リビジョンを別の親に複製します:

`jj duplicate {{[-d|--destination]}} {{dest_revset}} {{revset}}`

- リビジョンを複製し、他のリビジョンの後に挿入します:

`jj duplicate {{[-A|--insert-after]}} {{after_revset}} {{revset}}`

- リビジョンを複製し、他のリビジョンの前に挿入します:

`jj duplicate {{[-B|--insert-before]}} {{before_revset}} {{revset}}`

- 複数の親に複製します (マージコミットを作成します):

`jj duplicate {{[-d|--destination]}} {{destination1}} {{[-d|--destination]}} {{destination2}} {{revset}}`

- 複数のリビジョンを複製します:

`jj duplicate {{revset1 revset2 ...}}`
