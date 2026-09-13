# jj operation show

> 操作におけるリポジトリの変更を表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-show>。

- 現在の操作におけるリポジトリの変更を親と比較して表示します:

`jj {{[op|operation]}} show`

- 特定の操作でのリポジトリの変更を表示します:

`jj {{[op|operation]}} show {{operation_id}}`

- リポジトリの変更をパッチの詳細とともに表示します:

`jj {{[op|operation]}} show {{[-p|--patch]}} {{operation_id}}`

- 操作で変更されたパスの概要を表示します:

`jj {{[op|operation]}} show {{[-s|--summary]}} {{operation_id}}`

- 操作における変更のヒストグラムを表示します:

`jj {{[op|operation]}} show --stat {{operation_id}}`

- グラフなしで変化を表示します:

`jj {{[op|operation]}} show {{[-G|--no-graph]}} {{operation_id}}`
