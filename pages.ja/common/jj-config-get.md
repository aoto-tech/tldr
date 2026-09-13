# jj config get

> 指定された構成オプションの値を取得します。
> `jj config list` とは異なり、結果はスクリプトで使用するための追加の書式設定なしで出力されます。
> `jj config list` も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-config-get>。

- 構成オプションの値を取得します:

`jj config {{[g|get]}} {{name}}`

- 設定されたユーザー名を取得します:

`jj config {{[g|get]}} user.name`

- 設定されたユーザーの電子メールを取得します:

`jj config {{[g|get]}} user.email`

- ログ コマンドのデフォルトの Revset を取得します:

`jj config {{[g|get]}} revsets.log`
