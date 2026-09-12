# npm cache

> npm パッケージのキャッシュを管理します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-cache/>。

- 特定のパッケージをキャッシュに追加します:

`npm cache add {{package_name}}`

- キーによって特定のキャッシュされたアイテムをクリアします:

`npm cache clean {{key}}`

- npm キャッシュ全体をクリアします:

`npm cache clean {{[-f|--force]}}`

- キャッシュされたパッケージをリストします:

`npm cache ls`

- 特定の名前とバージョンに一致するキャッシュされたパッケージをリストします:

`npm cache ls {{name}}@{{version}}`

- npm キャッシュの整合性を確認します:

`npm cache verify`

- npx キャッシュ内のすべてのエントリを一覧表示します:

`npm cache npx ls`
