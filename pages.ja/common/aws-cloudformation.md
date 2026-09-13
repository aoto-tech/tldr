# aws cloudformation

> インフラストラクチャをコードとして扱うことで、AWS およびサードパーティのリソースをモデル化、プロビジョニング、管理する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cloudformation/>。

- テンプレートファイルからスタックを作成する:

`aws cloudformation create-stack --stack-name {{stack-name}} --region {{region}} --template-body {{file://path/to/file.yml}} --profile {{profile}}`

- スタックを削除する:

`aws cloudformation delete-stack --stack-name {{stack-name}} --profile {{profile}}`

- すべてのスタックを一覧表示する:

`aws cloudformation list-stacks --profile {{profile}}`

- 実行中のすべてのスタックを一覧表示する:

`aws cloudformation list-stacks --stack-status-filter CREATE_COMPLETE --profile {{profile}}`

- スタックのステータスを確認する:

`aws cloudformation describe-stacks --stack-name {{stack-id}} --profile {{profile}}`

- スタックのドリフト検出を開始する:

`aws cloudformation detect-stack-drift --stack-name {{stack-id}} --profile {{profile}}`

- 前のコマンド出力の `StackDriftDetectionId` を使用して、スタックのドリフトステータス出力を確認する:

`aws cloudformation describe-stack-resource-drifts --stack-name {{stack-drift-detection-id}} --profile {{profile}}`
