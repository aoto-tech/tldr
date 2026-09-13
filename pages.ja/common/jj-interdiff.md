# jj interdiff

> 2 つのリビジョンの変更を比較します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-interdiff>。

- リビジョンから作業コピーへの変更を比較します:

`jj interdiff {{[-f|--from]}} {{revset}}`

- あるリビジョンから別のリビジョンへの変更を比較します:

`jj interdiff {{[-f|--from]}} {{from_revset}} {{[-t|--to]}} {{to_revset}}`

- 特定のパス内の変更のみを比較します:

`jj interdiff {{[-f|--from]}} {{from_revset}} {{[-t|--to]}} {{to_revset}} {{filesets}}`

- 変更の概要を表示します:

`jj interdiff {{[-f|--from]}} {{revset}} {{[-s|--summary]}}`

- 差分の統計を表示します:

`jj interdiff {{[-f|--from]}} {{revset}} --stat`

- Git 形式の差分を表示します:

`jj interdiff {{[-f|--from]}} {{revset}} --git`

- 色のみで示される変更を含む単語レベルの差分を表示します:

`jj interdiff {{[-f|--from]}} {{revset}} --color-words`
