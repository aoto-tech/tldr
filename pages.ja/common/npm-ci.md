# npm ci

> 自動環境用の `npm` プロジェクトの依存関係をクリーン インストールします。
> `package-lock.json` または `npm-shrinkwrap.json` に基づいてパッケージをインストールします。
> 詳細情報: <https://docs.npmjs.com/cli/npm-ci/>。

- `package-lock.json` または `npm-shrinkwrap.json` からプロジェクトの依存関係をインストールします:

`npm ci`

- プロジェクトの依存関係をインストールしますが、指定された依存関係の種類はスキップします:

`npm ci --omit {{dev|optional|peer}}`

- `package.json` で定義された前後スクリプトを実行せずに、プロジェクトの依存関係をインストールします:

`npm ci --ignore-scripts`
