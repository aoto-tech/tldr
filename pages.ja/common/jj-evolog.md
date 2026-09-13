# jj evolog

> 変更が時間の経過とともにどのように変化したかを示し、その変更が指す以前のコミットをリストします。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-evolog>。

- リビジョンが時間の経過とともにどのように進化したかを示します:

`jj evolog {{[-r|--revisions]}} {{revsets}}`

- 進化ログの差分統計を表示します:

`jj evolog {{[-r|--revisions]}} {{revsets}} --stat`

- 進化ログ内の各変更の概要を表示します:

`jj evolog {{[-r|--revisions]}} {{revsets}} {{[-s|--summary]}}`
