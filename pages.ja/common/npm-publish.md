# npm publish

> パッケージを npm レジストリに発行します。
> 詳細情報: <https://docs.npmjs.com/cli/publish/>。

- 現在のパッケージをデフォルトの npm レジストリに公開します:

`npm publish`

- 特定のディレクトリからパッケージを公開します:

`npm publish {{path/to/package_directory}}`

- スコープ指定されたパッケージをパブリック アクセスで公開します:

`npm publish --access public`

- 制限された (プライベート) アクセスを使用してスコープ指定されたパッケージを公開します:

`npm publish --access restricted`

- パッケージをカスタム レジストリに公開します:

`npm publish --registry {{https://registry.npmjs.org/}}`

- ドライランを実行して、アップロードせずに何が公開されるかを確認します:

`npm publish --dry-run`

- 特定の配布タグ (ベータ版など) を使用してパッケージを公開します:

`npm publish --tag {{beta}}`

- 2FA が有効なアカウントのワンタイム パスワードを使用して公開します:

`npm publish --otp {{one_time_password}}`
