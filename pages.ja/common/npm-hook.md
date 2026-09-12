# npm hook

> パッケージの `npm` レジストリ フックを管理します。
> 注: このコマンドは非推奨になりました。
> 詳細情報: <https://docs.npmjs.com/cli/v10/hook/>。

- すべてのアクティブなフックをリストします:

`npm hook ls`

- パッケージに新しいフックを追加します:

`npm hook add {{package_name}} {{event}} {{target_url}}`

- ID によって特定のフックを削除します:

`npm hook rm {{hook_id}}`

- 新しい情報でフックを更新します:

`npm hook update {{hook_id}} {{target_url}}`
