# aws sso

> シングルサインオン (SSO) 認証情報を使用して AWS リソースへのアクセスを管理する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sso/>。

- SSO セッションを開始し、アクセストークンを更新する (`aws configure sso` によるセットアップが必要):

`aws sso login`

- SSO セッションを終了し、キャッシュされたアクセストークンをクリアする:

`aws sso logout`

- ユーザーがアクセスできるすべての AWS アカウントを一覧表示する:

`aws sso list-accounts --access-token {{token}}`

- 特定の AWS アカウントのユーザーがアクセスできるすべてのロールを一覧表示する:

`aws sso list-account-roles --account-id {{account}} --access-token {{token}}`

- 特定のアカウントの短期認証情報を取得する:

`aws sso get-role-credentials --account-id {{account}} --role-name {{role}} --access-token {{token}}`
