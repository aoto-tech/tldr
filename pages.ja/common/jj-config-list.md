# jj config list

> 構成ファイルに設定されている変数をその値とともにリストします。
> `jj config get` も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-config-list>。

- すべての構成変数とその値をリストします:

`jj config {{[l|list]}}`

- 特定の構成オプションをリストします:

`jj config {{[l|list]}} {{name}}`

- ユーザーレベルの構成変数をリストします:

`jj config {{[l|list]}} --user`

- リポジトリレベルの構成変数をリストします:

`jj config {{[l|list]}} --repo`

- 組み込みのデフォルト値を含む構成変数をリストします:

`jj config {{[l|list]}} --include-defaults`

- オーバーライドされた値を含む構成変数をリストします:

`jj config {{[l|list]}} --include-overridden`

- カスタム テンプレートを使用して構成変数を一覧表示します:

`jj config {{[l|list]}} {{[-T|--template]}} {{template}}`
