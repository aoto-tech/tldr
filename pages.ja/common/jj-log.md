# jj log

> 変更履歴をグラフで表示します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-log>。

- リビジョン履歴をグラフで表示します:

`jj log`

- 指定されたリビジョンセットのみを表示します (例: `B::D`、`A..D`、`B|C|D` など):

`jj log {{[-r|--revisions]}} {{revsets}}`

- カスタムテンプレートを使用してログを表示します (例: 5 文字以上の一意なコミットハッシュ接頭辞と作成者):

`jj log {{[-T|--template]}} 'commit_id.shortest(5) ++ " " ++ author'`
