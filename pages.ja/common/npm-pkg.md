# npm pkg

> `package.json` プロパティを表示または変更します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-pkg/>。

- 特定のプロパティの値を取得します:

`npm pkg get {{name}}`

- 複数のプロパティを一度に取得します:

`npm pkg get {{name|version|...}}`

- すべてのワークスペースにわたって複数の値を取得します:

`npm pkg get {{name}} {{version}} {{[--ws|--workspaces]}}`

- ネストされたプロパティ値または配列プロパティ値を取得します:

`npm pkg get {{contributors[0].email}}`

- プロパティを特定の値に設定します:

`npm pkg set {{property}}={{value}}`

- 複数のプロパティを一度に設定します:

`npm pkg set {{property1}}={{value1}} {{property2}}={{value2}}`

- `package.json` からプロパティを削除します:

`npm pkg delete {{scripts.build}}`

- `package.json` の一般的なエラーを自動修正します:

`npm pkg fix`
