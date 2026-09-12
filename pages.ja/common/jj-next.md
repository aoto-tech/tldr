# jj next

> 作業コピーのコミットを子リビジョンに移動します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-next>。

- 作業コピーのコミットを次の子リビジョンに移動します:

`jj next`

- 作業コピーのコミットをリビジョン数だけ前に移動します:

`jj next {{offset}}`

- 新しい作業コピーのコミットを作成する代わりに、子リビジョンを直接編集します:

`jj next {{[-e|--edit]}}`

- 子リビジョンを直接編集する代わりに、新しい作業コピーのコミットを作成します:

`jj next {{[-n|--no-edit]}}`

- 次の競合している子にジャンプします:

`jj next --conflict`
