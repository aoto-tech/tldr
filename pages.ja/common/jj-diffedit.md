# jj diffedit

> 差分エディターを使用して、リビジョン内の内容の変更を修正します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-diffedit>。

- 差分エディタを使用して現在のリビジョンの変更を編集します:

`jj diffedit`

- 特定のリビジョンの変更を編集します:

`jj diffedit {{[-r|--revision]}} {{revset}}`

- 「開始」リビジョンと「終了」リビジョンを比較して変更を編集します:

`jj diffedit {{[-f|--from]}} {{from_revset}} {{[-t|--to]}} {{to_revset}}`

- 特定のパスのみを編集します (一致しないパスは変更されません):

`jj diffedit {{filesets}}`

- 特定の差分エディタを使用します:

`jj diffedit --tool {{name}}`

- 子孫をリベースするときに diff ではなくコンテンツを保持します:

`jj diffedit --restore-descendants`
