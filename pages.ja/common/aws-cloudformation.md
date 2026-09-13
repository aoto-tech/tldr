# aws cloudformation

> インフラストラクチャをコードとして扱うことで、AWS およびサードパーティのリソースをモデル化、プロビジョニング、管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cloudformation/>。

- テンプレート ファイルからスタックを作成します:

`aws cloudformation create-stack --stack-name {{stack-name}} --region {{region}} --template-body {{file://path/to/file.yml}} --profile {{profile}}`

- スタックを削除します:

`aws cloudformation delete-stack --stack-name {{stack-name}} --profile {{profile}}`

- すべてのスタックをリストします:

`aws cloudformation list-stacks --profile {{profile}}`

- 実行中のすべてのスタックをリストします:

`aws cloudformation list-stacks --stack-status-filter CREATE_COMPLETE --profile {{profile}}`

- スタックのステータスを確認します:

`aws cloudformation describe-stacks --stack-name {{stack-id}} --profile {{profile}}`

- スタックのドリフト検出を開始します:

`aws cloudformation detect-stack-drift --stack-name {{stack-id}} --profile {{profile}}`

- 前のコマンド出力の `StackDriftDetectionId` を使用して、スタックのドリフト ステータス出力を確認します:

`aws cloudformation describe-stack-resource-drifts --stack-name {{stack-drift-detection-id}} --profile {{profile}}`
