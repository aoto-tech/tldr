# aws batch

> AWS Batch サービスを通じてバッチコンピューティングワークロードを実行する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/batch/>。

- 実行中のバッチジョブを一覧表示する:

`aws batch list-jobs --job-queue {{queue_name}}`

- コンピューティング環境を作成する:

`aws batch create-compute-environment --compute-environment-name {{compute_environment_name}} --type {{type}}`

- バッチジョブキューを作成する:

`aws batch create-job-queue --job-queue-name {{queue_name}} --priority {{priority}} --compute-environment-order {{compute_environment}}`

- ジョブを送信する:

`aws batch submit-job --job-name {{job_name}} --job-queue {{job_queue}} --job-definition {{job_definition}}`

- バッチジョブの詳細を表示する:

`aws batch describe-jobs --jobs {{jobs}}`

- ジョブをキャンセルする:

`aws batch cancel-job --job-id {{job_id}} --reason {{reason}}`
