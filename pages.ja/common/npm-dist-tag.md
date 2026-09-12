# npm dist-tag

> パッケージの配布タグを管理します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-dist-tag/>。

- パッケージのすべての配布タグをリストします:

`npm dist-tag ls {{package_name}}`

- 現在のパッケージのすべての配布タグをリストします:

`npm dist-tag ls`

- 特定のパッケージ バージョンに配布タグを追加します:

`npm dist-tag add {{package_name}}@{{version}} {{tag}}`

- パッケージから配布タグを削除します:

`npm dist-tag rm {{package_name}} {{tag}}`

- npm config から設定されたタグを使用してタグを追加します:

`npm dist-tag add {{package_name}}@{{version}}`

- 2 要素認証を使用してタグを追加します:

`npm dist-tag add {{package_name}}@{{version}} {{tag}} --otp {{one_time_password}}`
