# jj bookmark

> `jj` リポジトリでブックマークを管理します。
> Git バックエンドを使用する場合、ブックマークは Git ブランチに対応します。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-bookmark>。

- 指定されたリビジョンで新しいブックマークを作成します:

`jj {{[b|bookmark]}} {{[c|create]}} {{[-r|--revision]}} {{revision}} {{name}}`

- 既存のブックマークとそのターゲットをすべてリストします:

`jj {{[b|bookmark]}} {{[l|list]}}`

- 既存のブックマークを別のリビジョンに移動します:

`jj {{[b|bookmark]}} {{[m|move]}} {{[-t|--to]}} {{revision}} {{name}}`

- 指定されたリモート ブックマークを追跡します:

`jj {{[b|bookmark]}} {{[t|track]}} {{name}}@{{remote}}`

- ブックマークを削除し、次回のプッシュ時に削除をリモートに伝播します:

`jj {{[b|bookmark]}} {{[d|delete]}} {{name}}`

- 削除をプッシュするマークを付けずに、ブックマークをローカルで削除します:

`jj {{[b|bookmark]}} {{[f|forget]}} {{name}}`
