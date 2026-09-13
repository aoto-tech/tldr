# jj operation diff

> 2 つの操作間のリポジトリへの変更を比較します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-diff>。

- 特定の操作におけるリポジトリの変更をその親と比較します:

`jj {{[op|operation]}} diff {{[--op|--operation]}} {{operation_id}}`

- 2 つの特定の操作間のリポジトリの変更を比較します:

`jj {{[op|operation]}} diff {{[-f|--from]}} {{from_op}} {{[-t|--to]}} {{to_op}}`

- 変更に対する修正パッチを含む diff を表示します:

`jj {{[op|operation]}} diff {{[-p|--patch]}} {{[--op|--operation]}} {{operation_id}}`

- diff を変更のヒストグラムとして表示します:

`jj {{[op|operation]}} diff --stat {{[--op|--operation]}} {{operation_id}}`

- グラフなしで差分を表示します:

`jj {{[op|operation]}} diff {{[-G|--no-graph]}} {{[--op|--operation]}} {{operation_id}}`
