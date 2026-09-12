# npm star

> パッケージをお気に入りとしてマークします。
> 詳細情報: <https://docs.npmjs.com/cli/v11/npm-star>。

- デフォルトのレジストリからパブリック パッケージにスターを付けます:

`npm star {{package_name}}`

- 特定のスコープ内のパッケージにスターを付けます:

`npm star @{{scope}}/{{package_name}}`

- 特定のレジストリからパッケージにスターを付けます:

`npm star {{package_name}} --registry {{registry_url}}`

- 認証が必要なプライベート パッケージにスターを付けます:

`npm star {{package_name}} --auth-type {{legacy|oauth|web|saml}}`

- 2 要素認証用の OTP を提供してパッケージにスターを付けます:

`npm star {{package_name}} --otp {{otp}}`

- 詳細なログを含むパッケージにスターを付けます:

`npm star {{package_name}} --loglevel verbose`

- スター付きパッケージをすべてリストします:

`npm star --list`

- 特定のレジストリからスター付きパッケージを一覧表示します:

`npm star --list --registry {{registry_url}}`
