# jj file show

> `jj` リポジトリのリビジョン内のファイルの内容を出力します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file-show>。

- ファイルの内容を作業コピーに出力します:

`jj file show {{path/to/file}}`

- 特定のリビジョンのファイルの内容を出力します:

`jj file show {{[-r|--revision]}} {{revision}} {{path/to/file}}`

- ディレクトリ以下のファイル内容を再帰的に出力します:

`jj file show {{path/to/directory}}`

- カスタム テンプレートを使用してファイルのメタデータを印刷します:

`jj file show {{[-T|--template]}} "{{template}}" {{path/to/file}}`
