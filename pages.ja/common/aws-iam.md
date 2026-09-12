# aws iam

> AWS サービスへのアクセスを安全に制御するための Web サービスである Identity and Access Management (IAM) と対話します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/iam/>。

- ユーザーをリストします:

`aws iam list-users`

- ポリシーをリストします:

`aws iam list-policies`

- グループをリストします:

`aws iam list-groups`

- ユーザーをグループに追加します:

`aws iam get-group --group-name {{group_name}}`

- IAM ポリシーを説明します:

`aws iam get-policy --policy-arn arn:aws:iam::aws:policy/{{policy_name}}`

- アクセスキーをリストします:

`aws iam list-access-keys`

- 特定のユーザーのアクセス キーを一覧表示します:

`aws iam list-access-keys --user-name {{user_name}}`

- ヘルプを表示する:

`aws iam help`
