# npm search

> `npm` レジストリでパッケージを検索します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-search/>。

- 名前でパッケージを検索します:

`npm {{[s|search]}} {{package}}`

- 特定のキーワードでパッケージを検索します:

`npm {{[s|search]}} {{keyword}}`

- 詳細情報 (説明、作成者、バージョンなど) を含むパッケージを検索します:

`npm {{[s|search]}} {{package}} --long`

- 特定の作成者によって管理されているパッケージを検索します:

`npm {{[s|search]}} --author {{author}}`

- 特定の組織のパッケージを検索します:

`npm {{[s|search]}} --scope {{organization}}`

- 特定の用語の組み合わせを含むパッケージを検索します:

`npm {{[s|search]}} {{term1 term2 ...}}`
