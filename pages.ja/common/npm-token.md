# npm token

> npm レジストリの認証トークンを管理および生成します。
> 詳細情報: <https://docs.npmjs.com/cli/npm-token/>。

- 新しい認証トークンを作成します:

`npm token create`

- アカウントに関連付けられているすべてのトークンをリストします:

`npm token list`

- トークン ID を使用して特定のトークンを削除します:

`npm token revoke {{token_id}}`

- 読み取り専用アクセスを持つトークンを作成します:

`npm token create --read-only`

- 公開アクセス権を持つトークンを作成します:

`npm token create --publish`

- ログイン時に、グローバル `.npmrc` ファイルに npm トークンを自動的に構成します:

`npm login`

- グローバル構成からトークンを削除します:

`npm token revoke {{token_id}}`
