# npm bugs

> Web ブラウザでパッケージのバグを報告します。
> パッケージのバグ トラッカー URL またはサポート電子メールを開こうとします。
> 詳細情報: <https://docs.npmjs.com/cli/npm-bugs/>。

- 特定のパッケージのバグ トラッカーを開いて、特定のパッケージのバグを報告します:

`npm bugs {{package_name}}`

- `package.json` ファイルを検索し、その名前を使用して、現在のパッケージのバグ トラッカーを開きます:

`npm bugs`

- `npm` コマンドに優先ブラウザを設定して、URL を開くために使用するブラウザを構成します:

`npm {{[c|config]}} set browser {{browser_name}}`

- URL オープンの制御: システム URL オープナーの場合は `browser` を `true` に設定し、端末で URL を出力する場合は `false` を設定します:

`npm {{[c|config]}} set browser {{true|false}}`
