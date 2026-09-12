# npm unstar

> パッケージからお気に入り/スターマークを削除します。
> 詳細情報: <https://docs.npmjs.com/cli/v11/npm-unstar>。

- デフォルトのレジストリからパブリック パッケージのスターを外します:

`npm unstar {{package_name}}`

- 特定のスコープ内のパッケージのスターを外します:

`npm unstar @{{scope}}/{{package_name}}`

- 特定のレジストリからパッケージのスターを外します:

`npm unstar {{package_name}} --registry {{registry_url}}`

- 認証が必要なプライベート パッケージのスターを外します:

`npm unstar {{package_name}} --auth-type {{legacy|oauth|web|saml}}`

- 2 要素認証用の OTP を提供して、パッケージのスターを解除します:

`npm unstar {{package_name}} --otp {{otp}}`

- 特定のログレベルでパッケージのスターを外します:

`npm unstar {{package_name}} --loglevel {{silent|error|warn|notice|http|timing|info|verbose|silly}}`
