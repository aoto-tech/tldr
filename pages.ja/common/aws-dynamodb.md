# aws dynamodb

> 予測可能なパフォーマンスとシームレスなスケーラビリティを備えた高速 NoSQL データベースである AWS DynamoDB データベースを操作します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/dynamodb/>。

- テーブルを作成します:

`aws dynamodb create-table --table-name {{table_name}} --attribute-definitions {{AttributeName=S,AttributeType=S}} --key-schema {{AttributeName=S,KeyType=HASH}} --provisioned-throughput {{ReadCapacityUnits=5,WriteCapacityUnits=5}}`

- DynamoDB 内のすべてのテーブルを一覧表示します:

`aws dynamodb list-tables`

- 特定のテーブルに関する詳細を取得します:

`aws dynamodb describe-table --table-name {{table_name}}`

- 項目をテーブルに追加します:

`aws dynamodb put-item --table-name {{table_name}} --item '{{{"AttributeName": {"S": "value"\}\}}}'`

- テーブルから項目を取得します:

`aws dynamodb get-item --table-name {{table_name}} --key '{{{"ID": {"N": "1"\}\}}}'`

- テーブル内の項目を更新します:

`aws dynamodb update-item --table-name {{table_name}} --key '{{{"ID": {"N": "1"\}\}}}' --update-expression "{{SET Name = :n}}" --expression-attribute-values '{{{":n": {"S": "Jane"\}\}}}'`

- テーブル内の項目をスキャンします:

`aws dynamodb scan --table-name {{table_name}}`

- テーブルから項目を削除します:

`aws dynamodb delete-item --table-name {{table_name}} --key '{{{"ID": {"N": "1"\}\}}}'`
