# aws logs

> さまざまな AWS サービスからのログファイルを操作する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/logs/>。

- ロググループを一覧表示する:

`aws logs list-log-groups`

- CloudWatch ロググループのログを継続的にポーリングする:

`aws logs tail {{log_group_name}} --follow`

- フィルターに基づいて CloudWatch ロググループのログを追跡する:

`aws logs tail {{log_group_name}} --filter-pattern {{pattern}}`

- ロググループからほぼリアルタイムのログをストリーミングする:

`aws logs start-live-tail --log-group-identifiers {{log_group_name}}`

- ログを S3 バケットにエクスポートする:

`aws logs create-export-task --log-group-name {{log_group_name}} --from {{start_time}} --to {{end_time}} --destination {{s3_bucket_name}}`
