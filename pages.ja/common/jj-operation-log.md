# jj operation log

> `jj` リポジトリ内の操作ログを表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-log>。

- 操作ログを表示します:

`jj {{[op|operation]}} log`

- 表示する操作の数を制限します:

`jj {{[op|operation]}} log {{[-n|--limit]}} {{count}}`

- 操作を逆順に表示します (古いものから順):

`jj {{[op|operation]}} log --reversed`

- グラフなしで操作を表示します:

`jj {{[op|operation]}} log {{[-G|--no-graph]}}`

- カスタム テンプレートを使用して操作ログをレンダリングします:

`jj {{[op|operation]}} log {{[-T|--template]}} "{{template}}"`
