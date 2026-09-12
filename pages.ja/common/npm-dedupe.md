# npm dedupe

> `node_modules` ディレクトリ内の重複を減らします。
> 詳細情報: <https://docs.npmjs.com/cli/npm-dedupe/>。

- `node_modules` のパッケージの重複を排除します:

`npm {{[ddp|dedupe]}}`

- 重複排除中に `package-lock.json` または `npm-shrinkwrap.json` に従います:

`npm {{[ddp|dedupe]}} --lock`

- 重複排除を厳密モードで実行します:

`npm {{[ddp|dedupe]}} --strict`

- 重複排除中にオプション/ピアの依存関係をスキップします:

`npm {{[ddp|dedupe]}} --omit {{optional|peer}}`

- トラブルシューティングのために詳細なログを有効にします:

`npm {{[ddp|dedupe]}} --loglevel verbose`

- 重複排除を特定のパッケージに制限します:

`npm {{[ddp|dedupe]}} {{package_name}}`
