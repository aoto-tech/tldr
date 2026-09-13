# aws sts

> セキュリティトークンサービス (STS) を使用すると、IAM ユーザーまたはフェデレーションユーザーは一時的な認証情報を要求できる。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sts/>。

- 特定の AWS リソースにアクセスするための一時的なセキュリティ認証情報を取得する:

`aws sts assume-role --role-arn {{aws_role_arn}}`

- オペレーションを呼び出すために認証情報が使用される IAM ユーザーまたはロールを取得する:

`aws sts get-caller-identity`
