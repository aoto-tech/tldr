# jj tag set

> `jj` リポジトリでタグを作成または更新します。
> 「`jj tag delete`」、「`jj tag list`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-tag-set>。

- 現在の作業コピー リビジョンを指すタグを作成します:

`jj tag {{[s|set]}} {{tag_name}}`

- 特定のリビジョンを指すタグを作成します:

`jj tag {{[s|set]}} {{tag_name}} {{[-r|--revision]}} {{revision}}`

- 同じリビジョンを指す複数のタグを作成します:

`jj tag {{[s|set]}} {{tag1 tag2 ...}} {{[-r|--revision]}} {{revision}}`

- 既存のタグを別のリビジョンに移動します:

`jj tag {{[s|set]}} {{tag_name}} {{[-r|--revision]}} {{revision}} --allow-move`

- 現在のリビジョンの親を指すタグを作成します:

`jj tag {{[s|set]}} {{tag_name}} {{[-r|--revision]}} @-`
