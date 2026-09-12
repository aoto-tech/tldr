# npm profile

> npm プロファイルと関連設定を管理します。
> 注: このコマンドはワークスペースを認識しません。
> 詳細情報: <https://docs.npmjs.com/cli/npm-profile/>。

- npm プロファイルの詳細を表示します:

`npm profile get`

- プロファイルの特定のプロパティを表示します:

`npm profile get {{property}}`

- プロファイル プロパティを設定または更新します:

`npm profile set {{property}} {{value}}`

- パブリック電子メール アドレスを設定します:

`npm profile set email {{email}}`

- パブリック名を設定します:

`npm profile set fullname {{name}}`

- 新しいパスワードを対話的に設定します:

`npm profile set password`

- 2 要素認証 (2FA) を有効にします (デフォルトは `auth-and-writes`):

`npm profile enable-2fa {{auth-only|auth-and-writes}}`

- 2 要素認証 (2FA) を無効にします:

`npm profile disable-2fa`
