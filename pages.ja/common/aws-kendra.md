# aws kendra

> AWS Kendra の CLI。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kendra/>。

- インデックスを作成します:

`aws kendra create-index --name {{name}} --role-arn {{role_arn}}`

- リストインデックス:

`aws kendra list-indexes`

- インデックスを説明します:

`aws kendra describe-index --id {{index_id}}`

- データ ソースをリストします:

`aws kendra list-data-sources`

- データソースを説明します:

`aws kendra describe-data-source --id {{data_source_id}}`

- リスト検索クエリ:

`aws kendra list-query-suggestions --index-id {{index_id}} --query-text {{query_text}}`
