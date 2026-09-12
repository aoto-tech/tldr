# aws cognito-idp

> Amazon Cognito ユーザープールとそのユーザーとグループを設定し、認証します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cognito-idp/>。

- 新しい Cognito ユーザー プールを作成します:

`aws cognito-idp create-user-pool --pool-name {{name}}`

- すべてのユーザープールをリストします:

`aws cognito-idp list-user-pools --max-results {{10}}`

- 特定のユーザープールを削除します:

`aws cognito-idp delete-user-pool --user-pool-id {{user_pool_id}}`

- 特定のプールにユーザーを作成します:

`aws cognito-idp admin-create-user --username {{username}} --user-pool-id {{user_pool_id}}`

- 特定のプールのユーザーをリストします:

`aws cognito-idp list-users --user-pool-id {{user_pool_id}}`

- 特定のプールからユーザーを削除します:

`aws cognito-idp admin-delete-user --username {{username}} --user-pool-id {{user_pool_id}}`
