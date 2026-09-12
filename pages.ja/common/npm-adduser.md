# npm adduser

> レジストリ ユーザー アカウントを追加します。
> 詳細情報: <https://docs.npmjs.com/cli/v11/npm-adduser>。

- 指定したレジストリに新しいユーザーを作成し、資格情報を `.npmrc` に保存します:

`npm adduser --registry {{registry_url}}`

- 特定のスコープでプライベート レジストリにログインします:

`npm login --scope {{@organization}} --registry {{https://registry.example.com}}`

- 特定のスコープからログアウトし、認証トークンを削除します:

`npm logout --scope {{@organization}}`

- 初期化中にスコープ指定されたパッケージを作成します:

`npm init --scope {{@organization}} {{[-y|--yes]}}`
