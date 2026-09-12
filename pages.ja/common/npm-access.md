# npm access

> 公開されたパッケージにアクセス レベルを設定します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-access/>。

- ユーザーまたはスコープのパッケージをリストします:

`npm access list packages {{user|scope|scope:team}} {{package_name}}`

- パッケージの共同編集者をリストします:

`npm access list collaborators {{package_name}} {{username}}`

- パッケージのステータスを取得します:

`npm access get status {{package_name}}`

- パッケージのステータスを設定します (パブリックまたはプライベート):

`npm access set status={{public|private}} {{package_name}}`

- パッケージへのアクセスを許可します:

`npm access grant {{read-only|read-write}} {{scope:team}} {{package_name}}`

- パッケージへのアクセスを取り消します:

`npm access revoke {{scope:team}} {{package_name}}`

- 2 要素認証要件を構成します:

`npm access set mfa={{none|publish|automation}} {{package_name}}`
