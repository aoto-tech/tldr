# npm version

> ノードパッケージのバージョンを上げます。
> 詳細情報: <https://docs.npmjs.com/cli/npm-version/>。

- 表示バージョン:

`npm version`

- マイナー バージョンをバンプします:

`npm version minor`

- 特定のバージョンを設定します:

`npm version {{version}}`

- Git タグを作成せずにパッチ バージョンをバンプします:

`npm version patch --no-git-tag-version`

- カスタム コミット メッセージを使用してメジャー バージョンをバンプします:

`npm version major {{[-m|--message]}} "{{Upgrade to %s for reasons}}"`
