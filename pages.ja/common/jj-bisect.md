# jj bisect

> 二等分して不良リビジョンを見つけます。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-bisect>。

- テスト コマンドを実行して、範囲内の最初の不良リビジョンを見つけます:

`jj bisect run {{[-r|--range]}} {{good_revision}}..{{bad_revision}} {{command}}`

- シェル コマンドを使用して、最初の不良リビジョンを見つけます:

`jj bisect run {{[-r|--range]}} {{good_revision}}..{{bad_revision}} -- bash -c "{{command}}"`

- 最初の悪いリビジョンではなく、最初の正常なリビジョンを見つけます:

`jj bisect run {{[-r|--range]}} {{good_revision}}..{{bad_revision}} --find-good {{command}}`

- ファイルが追加された最初のリビジョンを見つけます:

`jj bisect run {{[-r|--range]}} {{good_revision}}..{{bad_revision}} --find-good -- test -f {{path/to/file}}`
