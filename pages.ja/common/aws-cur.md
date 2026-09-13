# aws cur

> AWS 使用状況レポート定義を作成、クエリ、および削除する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cur/>。

- JSON ファイルから AWS のコストと使用状況のレポート定義を作成する:

`aws cur put-report-definition --report-definition file://{{path/to/report_definition.json}}`

- ログインしたアカウントに対して定義されている使用状況レポート定義を一覧表示する:

`aws cur describe-report-definitions`

- 使用状況レポート定義を削除する:

`aws cur --region {{aws_region}} delete-report-definition --report-name {{report}}`
