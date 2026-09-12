# jj config

> 構成オプションを管理します。
> `edit`、`get`、`list`、`path`、`set`、`unset` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-config>。

- ユーザーレベルの構成ファイルでエディタを起動します:

`jj config {{[e|edit]}} --user`

- 構成オプションの値を取得します:

`jj config {{[g|get]}} {{name}}`

- すべての構成変数とその値をリストします:

`jj config {{[l|list]}}`

- 特定の構成オプションの値をリストします:

`jj config {{[l|list]}} {{name}}`

- ユーザーレベルの設定ファイルへのパスを出力します:

`jj config {{[p|path]}} --user`

- ユーザーレベルの設定で設定オプションを設定します:

`jj config {{[s|set]}} --user {{name}} {{value}}`

- ユーザーレベルの設定で設定オプションの設定を解除します:

`jj config {{[u|unset]}} --user {{name}}`

- 古いリポレベルの構成ディレクトリを見つけて削除します:

`jj config gc`
