# aws cloudwatch

> AWS リソースを監視して、リソースの使用率、アプリケーションのパフォーマンス、運用の健全性をシステム全体で可視化する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cloudwatch/>。

- アカウントのダッシュボードを一覧表示する:

`aws cloudwatch list-dashboards`

- 指定したダッシュボードの詳細を表示する:

`aws cloudwatch get-dashboard --dashboard-name {{dashboard_name}}`

- メトリクスを一覧表示する:

`aws cloudwatch list-metrics`

- アラームを一覧表示する:

`aws cloudwatch describe-alarms`

- アラームを作成または更新し、メトリックに関連付ける:

`aws cloudwatch put-metric-alarm --alarm-name {{alarm_name}} --evaluation-periods {{evaluation_periods}} --comparison-operator {{comparison_operator}}`

- 指定したアラームを削除する:

`aws cloudwatch delete-alarms --alarm-names {{alarm_names}}`

- 指定されたダッシュボードを削除する:

`aws cloudwatch delete-dashboards --dashboard-names {{dashboard_names}}`
