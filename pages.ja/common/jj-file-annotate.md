# jj file annotate

> `jj` リポジトリ内のターゲット ファイルの各行のソース変更を表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file-annotate>。

- 作業コピー内のファイルに 1 行ずつ注釈を付けます:

`jj file annotate {{path/to/file}}`

- 特定のリビジョンから始まるファイルに注釈を付けます:

`jj file annotate {{[-r|--revision]}} {{revision}} {{path/to/file}}`

- カスタム テンプレートを使用してファイルに注釈を付けます:

`jj file annotate {{[-T|--template]}} "{{template}}" {{path/to/file}}`
