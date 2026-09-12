# npm prune

> `node_modules` から無関係なパッケージを削除します。
> 注: 無関係なパッケージとは、どのパッケージの依存関係リストにもリストされていない、node_modules フォルダー内に存在するパッケージです。
> 詳細情報: <https://docs.npmjs.com/cli/npm-prune/>。

- 依存関係にリストされていない無関係なパッケージをすべて削除します:

`npm prune`

- 無関係なパッケージと devDependency を削除します (運用ビルドに役立ちます):

`npm prune --production`

- 変更を加えずに削除されるものを示します:

`npm prune --dry-run`

- 変更を JSON として出力します:

`npm prune --json`

- 特定のパッケージを名前で削除します:

`npm prune {{package_name}}`
