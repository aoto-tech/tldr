# jj operation restore

> リポジトリを操作ログ内の以前の状態に復元します。
> 「`jj undo`」、「`jj operation log`」、「`jj operation revert`」、「`jj operation show`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-operation-restore>。

- 特定の操作でリポジトリの状態を復元します:

`jj {{[op|operation]}} restore {{operation_id}}`

- リポジトリの状態とローカル ブックマークのみを復元します (リモート追跡ブックマークは無視します):

`jj {{[op|operation]}} restore --what repo {{operation_id}}`
