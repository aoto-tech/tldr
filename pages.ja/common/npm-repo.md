# npm repo

> ブラウザでパッケージのリポジトリ ページを開きます。
> 詳細情報: <https://docs.npmjs.com/cli/npm-repo/>。

- 現在のプロジェクトのリポジトリ ページを開きます (`package.json` に基づく):

`npm repo`

- レジストリから特定のパッケージのリポジトリ ページを開きます:

`npm repo {{package_name}}`

- 複数のパッケージのリポジトリ ページを開きます:

`npm repo {{package_name1 package_name2 ...}}`

- リポジトリ URL をブラウザで開く代わりに印刷します:

`npm repo --browser false`

- 特定のブラウザでパッケージのリポジトリ ページを開きます:

`npm repo --browser {{browser_name}}`

- 特定のワークスペースでパッケージのリポジトリ ページを開きます:

`npm repo --workspace {{workspace_name}}`
