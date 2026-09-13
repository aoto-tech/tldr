# aws kendra

> AWS Kendra の CLI。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kendra/>。

- インデックスを作成する:

`aws kendra create-index --name {{name}} --role-arn {{role_arn}}`

- インデックスを一覧表示する:

`aws kendra list-indexes`

- インデックスの詳細を表示する:

`aws kendra describe-index --id {{index_id}}`

- データソースを一覧表示する:

`aws kendra list-data-sources`

- データソースの詳細を表示する:

`aws kendra describe-data-source --id {{data_source_id}}`

- クエリ候補を取得する:

`aws kendra get-query-suggestions --index-id {{index_id}} --query-text {{query_text}}`
