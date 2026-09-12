# jj tag delete

> `jj` リポジトリ内のタグを削除します。
> 「`jj tag list`」、「`jj tag set`」も参照してください。
> 詳細情報: <https://docs.jj-vcs.dev/latest/cli-reference/#jj-tag-delete>。

- タグを削除します:

`jj tag {{[d|delete]}} {{tag_name}}`

- 複数のタグを削除します:

`jj tag {{[d|delete]}} {{tag1 tag2 ...}}`

- glob パターンに一致するタグを削除します:

`jj tag {{[d|delete]}} "{{glob:v1.*}}"`

- 部分文字列パターンに一致するタグを削除します:

`jj tag {{[d|delete]}} "{{substring:release}}"`

- 正確な名前でタグを削除します:

`jj tag {{[d|delete]}} "{{exact:v1.0.0}}"`
