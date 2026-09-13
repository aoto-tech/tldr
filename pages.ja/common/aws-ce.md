# aws ce

> AWS Cost Explorer サービスを通じてコスト管理操作を実行する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ce/>。

- 異常モニターを作成する:

`aws ce create-anomaly-monitor --monitor {{monitor_name}} --monitor-type {{monitor_type}}`

- 異常サブスクリプションを作成する:

`aws ce create-anomaly-subscription --subscription {{subscription_name}} --monitor-arn {{monitor_arn}} --subscribers {{subscribers}}`

- 異常を取得する:

`aws ce get-anomalies --monitor-arn {{monitor_arn}} --start-time {{start_time}} --end-time {{end_time}}`

- コストと使用量を取得する:

`aws ce get-cost-and-usage --time-period {{start_date}}/{{end_date}} --granularity {{granularity}} --metrics {{metrics}}`

- コスト予測を取得する:

`aws ce get-cost-forecast --time-period {{start_date}}/{{end_date}} --granularity {{granularity}} --metric {{metric}}`

- 予約使用率を取得する:

`aws ce get-reservation-utilization --time-period {{start_date}}/{{end_date}} --granularity {{granularity}}`

- コストカテゴリの定義を一覧表示する:

`aws ce list-cost-category-definitions`

- リソースにタグを付ける:

`aws ce tag-resource --resource-arn {{resource_arn}} --tags {{tags}}`
