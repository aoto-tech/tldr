# jj file list

> `jj` リポジトリのリビジョン内のファイルを一覧表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file-list>。

- 現在の作業コピー内のすべてのファイルを一覧表示します:

`jj file list`

- 特定のリビジョン内のすべてのファイルをリストします:

`jj file list {{[-r|--revision]}} {{revision}}`

- 特定のプレフィックスまたはパスに一致するファイルをリストします:

`jj file list {{path/to/directory}}`

- カスタム テンプレートを使用してレンダリングされたファイルをリストします:

`jj file list {{[-T|--template]}} "{{template}}"`
