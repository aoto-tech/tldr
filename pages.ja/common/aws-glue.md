# aws glue

> AWS Glue の CLI。
> AWS Glue サービスのパブリックエンドポイントを定義する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/glue/>。

- ジョブを一覧表示する:

`aws glue list-jobs`

- ジョブを開始する:

`aws glue start-job-run --job-name {{job_name}}`

- ワークフローの実行を開始する:

`aws glue start-workflow-run --name {{workflow_name}}`

- トリガーを一覧表示する:

`aws glue list-triggers`

- トリガーを開始する:

`aws glue start-trigger --name {{trigger_name}}`

- 開発エンドポイントを作成する:

`aws glue create-dev-endpoint --endpoint-name {{name}} --role-arn {{role_arn_used_by_endpoint}}`
