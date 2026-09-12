# aws sso

> シングル サインオン (SSO) 認証情報を使用して AWS リソースへのアクセスを管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sso/>。

- SSO セッションを開始し、アクセス トークンを更新します。 `aws configure sso` を使用したセットアップが必要です:

`aws sso login`

- SSO セッションを終了し、キャッシュされたアクセス トークンをクリアします:

`aws sso logout`

- ユーザーがアクセスできるすべての AWS アカウントをリストします:

`aws sso list-accounts`

- 特定の AWS アカウントのユーザーがアクセスできるすべてのロールを一覧表示します:

`aws sso list-account-roles --account-id {{account}} --access-token {{token}}`

- 特定のアカウントの短期認証情報を取得します:

`aws sso get-role-credentials --account-id {{account}} --role-name {{role}} --access-token {{token}}`
