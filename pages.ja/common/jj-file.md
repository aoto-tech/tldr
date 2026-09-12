# jj file

> `jj` リポジトリ内のファイルを管理および検査します。
> `annotate`、`list`、`search`、`show` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file>。

- 作業コピー内で追跡されているファイルをリストします:

`jj file list`

- ファイルの内容を作業コピーに出力します:

`jj file show {{path/to/file}}`

- 追跡されたファイル全体でパターンを検索します:

`jj file search {{[-p|--pattern]}} "{{pattern}}"`

- ファイルのソース変更の注釈を行ごとに表示します:

`jj file annotate {{path/to/file}}`

- 作業コピー内の指定されたパスを追跡します:

`jj file track {{path/to/file_or_directory}}`

- 作業コピー内の指定されたパスの追跡を停止します:

`jj file untrack {{path/to/file_or_directory}}`

- ファイルの実行可能ビットを設定または削除します:

`jj file chmod {{[-x|--executable]}} {{path/to/file}}`
