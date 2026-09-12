# aws batch

> AWS Batch サービスを通じてバッチ コンピューティング ワークロードを実行します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/batch/>。

- 実行中のバッチ ジョブをリストします:

`aws batch list-jobs --job-queue {{queue_name}}`

- コンピューティング環境を作成します:

`aws batch create-compute-environment --compute-environment-name {{compute_environment_name}} --type {{type}}`

- バッチ ジョブ キューを作成します:

`aws batch create-job-queue --job-queue-name {{queue_name}} --priority {{priority}} --compute-environment-order {{compute_environment}}`

- ジョブを送信します:

`aws batch submit-job --job-name {{job_name}} --job-queue {{job_queue}} --job-definition {{job_definition}}`

- バッチ ジョブのリストを説明します:

`aws batch describe-jobs --jobs {{jobs}}`

- ジョブをキャンセルします:

`aws batch cancel-job --job-id {{job_id}} --reason {{reason}}`
