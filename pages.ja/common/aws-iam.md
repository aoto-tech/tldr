# aws iam

> AWS サービスへのアクセスを安全に制御するための Web サービスである Identity and Access Management (IAM) と対話する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/iam/>。

- ユーザーを一覧表示する:

`aws iam list-users`

- ポリシーを一覧表示する:

`aws iam list-policies`

- グループを一覧表示する:

`aws iam list-groups`

- グループ内のユーザーを一覧表示する:

`aws iam get-group --group-name {{group_name}}`

- IAM ポリシーの詳細を表示する:

`aws iam get-policy --policy-arn arn:aws:iam::aws:policy/{{policy_name}}`

- アクセスキーを一覧表示する:

`aws iam list-access-keys`

- 特定のユーザーのアクセスキーを一覧表示する:

`aws iam list-access-keys --user-name {{user_name}}`

- ヘルプを表示する:

`aws iam help`
