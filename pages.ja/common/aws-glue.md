# aws glue

> AWS Glue の CLI。
> AWS Glue サービスのパブリック エンドポイントを定義します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/glue/>。

- ジョブのリストを表示します:

`aws glue list-jobs`

- ジョブを開始します:

`aws glue start-job-run --job-name {{job_name}}`

- ワークフローの実行を開始します:

`aws glue start-workflow-run --name {{workflow_name}}`

- トリガーのリスト:

`aws glue list-triggers`

- トリガーを開始します:

`aws glue start-trigger --name {{trigger_name}}`

- 開発エンドポイントを作成します:

`aws glue create-dev-endpoint --endpoint-name {{name}} --role-arn {{role_arn_used_by_endpoint}}`
