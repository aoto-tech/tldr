# jj tag list

> `jj` リポジトリ内のタグをリストします。
> 「`jj tag delete`」、「`jj tag set`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-tag-list>。

- すべてのタグをリストします:

`jj tag {{[l|list]}}`

- パターンに一致するタグをリストします:

`jj tag {{[l|list]}} "{{pattern}}"`

- 部分文字列パターンに一致するタグをリストします:

`jj tag {{[l|list]}} "{{substring:release}}"`

- タグをコミッターの日付順に並べ替えてリストします (新しいものから順):

`jj tag {{[l|list]}} --sort committer-date-`

- タグを名前の降順で並べ替えてリストします:

`jj tag {{[l|list]}} --sort name-`

- カスタム テンプレートを使用してタグをリストします:

`jj tag {{[l|list]}} {{[-T|--template]}} "{{template}}"`
