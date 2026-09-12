# npm login

> レジストリ ユーザー アカウントにログインします。
> `npm logout` も参照してください。
> 詳細情報: <https://docs.npmjs.com/cli/npm-login/>。

- レジストリ ユーザー アカウントにログインし、資格情報を `.npmrc` ファイルに保存します:

`npm login`

- カスタム レジストリを使用してログインします:

`npm login --registry {{registry_url}}`

- 特定の認証戦略を使用してログインします:

`npm login --auth-type {{legacy|web}}`
