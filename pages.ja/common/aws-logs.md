# aws logs

> さまざまな AWS サービスからのログ ファイルを操作します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/logs/>。

- ロググループをリストします:

`aws logs list-log-groups`

- CloudWatch ログ グループのログを継続的にポーリングします:

`aws logs tail {{log_group_name}} --follow`

- フィルターに基づいて CloudWatch ログ グループのログを追跡します:

`aws logs tail {{log_group_name}} --filter-pattern {{pattern}}`

- ログ グループからほぼリアルタイムのログをストリーミングします:

`aws logs start-live-tail --log-group-identifiers {{log_group_name}}`

- ログを S3 バケットにエクスポートします:

`aws logs create-export-task --log-group-name {{log_group_name}} --from {{start_time}} --to {{end_time}} --destination {{s3_bucket_name}}`
