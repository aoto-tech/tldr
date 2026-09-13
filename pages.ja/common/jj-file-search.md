# jj file search

> `jj` リポジトリ内のファイル内のコンテンツを検索します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file-search>。

- 作業コピー内のファイルから `regex` に一致する行を検索します:

`jj file search {{[-p|--pattern]}} "{{regex}}"`

- 作業コピー内のファイルから glob パターンに一致する行を検索します:

`jj file search {{[-p|--pattern]}} "{{glob:*pattern*}}"`

- 特定のリビジョンのファイル内のコンテンツを検索します:

`jj file search {{[-r|--revision]}} {{revision}} {{[-p|--pattern]}} "{{pattern}}"`

- 特定のパスまたはファイル内のみを検索します:

`jj file search {{[-p|--pattern]}} "{{pattern}}" {{path/to/file_or_directory}}`
