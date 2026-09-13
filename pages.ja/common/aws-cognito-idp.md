# aws cognito-idp

> Amazon Cognito ユーザープールとそのユーザーとグループを設定し、認証する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cognito-idp/>。

- 新しい Cognito ユーザープールを作成する:

`aws cognito-idp create-user-pool --pool-name {{name}}`

- すべてのユーザープールを一覧表示する:

`aws cognito-idp list-user-pools --max-results {{10}}`

- 特定のユーザープールを削除する:

`aws cognito-idp delete-user-pool --user-pool-id {{user_pool_id}}`

- 特定のプールにユーザーを作成する:

`aws cognito-idp admin-create-user --username {{username}} --user-pool-id {{user_pool_id}}`

- 特定のプールのユーザーを一覧表示する:

`aws cognito-idp list-users --user-pool-id {{user_pool_id}}`

- 特定のプールからユーザーを削除する:

`aws cognito-idp admin-delete-user --username {{username}} --user-pool-id {{user_pool_id}}`
