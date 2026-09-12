# jj operation revert

> 以前の操作を元に戻すには、`jj` リポジトリでその逆操作を適用します。
> 「`jj operation log`」、「`jj operation restore`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-revert>。

- 最新の操作を元に戻します:

`jj {{[op|operation]}} revert`

- 特定の操作を元に戻します:

`jj {{[op|operation]}} revert {{operation_id}}`

- 操作のリポジトリ状態とローカル ブックマークのみを元に戻します:

`jj {{[op|operation]}} revert --what repo {{operation_id}}`
