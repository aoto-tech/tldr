# jj file search

> `jj` リポジトリ内のファイル内のコンテンツを検索します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-file-search>。

- 作業コピーで `regex` を含むファイルを検索します:

`jj file search {{[-p|--pattern]}} "{{regex}}"`

- glob パターンを含むファイルを検索します:

`jj file search {{[-p|--pattern]}} "{{glob:*pattern*}}"`

- 特定のリビジョンのファイル内のコンテンツを検索します:

`jj file search {{[-r|--revision]}} {{revision}} {{[-p|--pattern]}} "{{pattern}}"`

- 特定のパスまたはファイル内のみを検索します:

`jj file search {{[-p|--pattern]}} "{{pattern}}" {{path/to/file_or_directory}}`
