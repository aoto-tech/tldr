# jj resolve

> 外部マージ ツールを使用して競合したファイルを解決します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-resolve>。

- すべての競合を解決します:

`jj resolve`

- すべての競合をリストします:

`jj resolve {{[-l|--list]}}`

- 特定のリビジョン内の競合を解決します:

`jj resolve {{[-r|--revision]}} {{revset}}`

- 指定されたファイル内の競合を解決します:

`jj resolve {{file1 file2 ...}}`

- 受信バージョンを受け入れることを解決します:

`jj resolve --tool :theirs`

- 送信バージョンを受け入れることを解決します:

`jj resolve --tool :ours`
