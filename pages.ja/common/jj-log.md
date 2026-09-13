# jj log

> 変更履歴をグラフで表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-log>。

- リビジョン履歴をグラフで表示します:

`jj log`

- 指定されたリビジョンセットのみを表示します (例: `B::D`、`A..D`、`B|C|D` など):

`jj log {{[-r|--revisions]}} {{revsets}}`

- 各行に特定のテンプレートを使用してログを表示します (例: コミット ハッシュと作成者の 5 文字):

`jj log {{[-T|--template]}} 'commit_id.shortest(5) ++ " " ++ author'`
