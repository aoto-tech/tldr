# aws sts

> セキュリティ トークン サービス (STS) を使用すると、IAM ユーザーまたはフェデレーション ユーザーは一時的な認証情報を要求できます。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sts/>。

- 特定の AWS リソースにアクセスするための一時的なセキュリティ認証情報を取得します:

`aws sts assume-role --role-arn {{aws_role_arn}}`

- オペレーションを呼び出すために認証情報が使用される IAM ユーザーまたはロールを取得します:

`aws sts get-caller-identity`
