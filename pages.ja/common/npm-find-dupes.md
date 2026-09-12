# npm find-dupes

> `node_modules` 内の重複した依存関係を特定します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-find-dupes/>。

- `node_modules` 内のすべての重複パッケージをリストします:

`npm find-dupes`

- 重複検出に `devDependencies` を含めます:

`npm find-dupes --include dev`

- `node_modules` 内の特定のパッケージの重複インスタンスをすべてリストします:

`npm find-dupes {{package_name}}`

- オプションの依存関係を重複検出から除外します:

`npm find-dupes --omit optional`

- 出力のログレベルを設定します:

`npm find-dupes --loglevel {{silent|error|warn|info|verbose}}`

- 重複した情報を JSON 形式で出力します:

`npm find-dupes --json`

- 重複検索を特定の範囲に制限します:

`npm find-dupes --scope {{@scope1,@scope2}}`

- 特定のスコープを重複検出から除外します:

`npm find-dupes --omit-scope {{@scope1,@scope2}}`
