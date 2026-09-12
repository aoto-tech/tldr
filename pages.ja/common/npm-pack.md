# npm pack

> パッケージから tarball を作成します。
> 詳細情報: <https://docs.npmjs.com/cli/pack/>。

- 現在のパッケージから現在のディレクトリに tarball を作成します:

`npm pack`

- 特定のパッケージ フォルダーから tarball を作成します:

`npm pack {{path/to/package_directory}}`

- ドライランを実行して、tarball の内容を作成せずにプレビューします:

`npm pack --dry-run`

- ライフサイクル スクリプトを実行せずに tarball を作成します:

`npm pack --ignore-scripts`

- パッケージのメタデータを取得するカスタム レジストリを指定します:

`npm pack --registry {{https://registry.npmjs.org/}}`
