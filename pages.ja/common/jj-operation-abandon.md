# jj operation abandon

> `jj` リポジトリ内の操作履歴を破棄します。
> 「`jj operation log`」、「`jj operation restore`」、「`jj operation revert`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-abandon>。

- 特定の操作を放棄します:

`jj {{[op|operation]}} abandon {{operation_id}}`

- 特定の操作とその祖先をすべて破棄します:

`jj {{[op|operation]}} abandon ..{{operation_id}}`

- 以前の状態に復元した後、最近の操作を破棄します:

`jj {{[op|operation]}} abandon {{operation_id}}..@-`
