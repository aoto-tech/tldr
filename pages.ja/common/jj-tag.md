# jj tag

> `jj` リポジトリでタグを管理します。
> `delete`、`list`、`set` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-tag>。

- 現在の作業コピー リビジョンを指すタグを作成します:

`jj tag {{[s|set]}} {{tag_name}}`

- 特定のリビジョンを指すタグを作成します:

`jj tag {{[s|set]}} {{tag_name}} {{[-r|--revision]}} {{revision}}`

- すべてのタグをリストします:

`jj tag {{[l|list]}}`

- パターンに一致するタグをコミッターの日付順に並べてリストします (新しいものから順):

`jj tag {{[l|list]}} --sort committer-date- "{{pattern}}"`

- 既存のタグを別のリビジョンに移動します:

`jj tag {{[s|set]}} {{tag_name}} {{[-r|--revision]}} {{revision}} --allow-move`

- タグを削除します:

`jj tag {{[d|delete]}} {{tag_name}}`

- glob パターンに一致するタグを削除します:

`jj tag {{[d|delete]}} "{{glob:v1.*}}"`

- ヘルプを表示する:

`jj tag {{[-h|--help]}}`
