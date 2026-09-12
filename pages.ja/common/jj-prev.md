# jj prev

> 作業コピーのコミットを親リビジョンに移動します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-prev>。

- 作業コピーのコミットを前の親リビジョンに移動します:

`jj prev`

- 作業コピーのコミットをリビジョン数だけ後方に移動します:

`jj prev {{offset}}`

- 新しい作業コピーのコミットを作成する代わりに、親リビジョンを直接編集します:

`jj prev {{[-e|--edit]}}`

- 親リビジョンを直接編集する代わりに、新しい作業コピーのコミットを作成します:

`jj prev {{[-n|--no-edit]}}`

- 競合している前の親にジャンプします:

`jj prev --conflict`
