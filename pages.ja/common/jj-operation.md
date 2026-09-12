# jj operation

> `jj` リポジトリの操作ログを操作します。
> `abandon`、`diff`、`integrate`、`log`、`restore`、`revert`、`show` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation>。

- 操作ログを表示:

`jj {{[op|operation]}} log`

- 特定の操作を放棄します:

`jj {{[op|operation]}} abandon {{operation}}`

- リポジトリを特定の操作時の状態に復元します:

`jj {{[op|operation]}} restore {{operation}}`

- 以前の操作を逆に適用して元に戻します:

`jj {{[op|operation]}} revert {{operation}}`

- 操作中のリポジトリへの変更を表示します:

`jj {{[op|operation]}} show {{operation}}`

- 操作の統計、概要、および変更のパッチを表示します:

`jj {{[op|operation]}} show {{--stat}} {{[-s|--summary]}} {{[-p|--patch]}} {{operation}}`

- 2 つの操作間のリポジトリの変更を比較します:

`jj {{[op|operation]}} diff {{[-f|--from]}} {{from_op}} {{[-t|--to]}} {{to_op}}`

- diff を変更のヒストグラムとして表示します:

`jj {{[op|operation]}} diff {{--stat}} {{[--op|--operation]}} {{operation_id}}`
