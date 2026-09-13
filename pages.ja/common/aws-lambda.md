# aws lambda

> サーバーのプロビジョニングや管理を行わずにコードを実行するためのコンピューティング サービスである AWS Lambda を使用します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/lambda/>。

- 関数を実行します:

`aws lambda invoke --function-name {{name}} {{path/to/response.json}}`

- JSON 形式の入力ペイロードを使用して関数を実行します:

`aws lambda invoke --function-name {{name}} --payload {{json}} {{path/to/response.json}}`

- リスト関数:

`aws lambda list-functions`

- 関数の構成を表示します:

`aws lambda get-function-configuration --function-name {{name}}`

- 関数エイリアスのリストを表示します:

`aws lambda list-aliases --function-name {{name}}`

- 関数の予約済み同時実行構成を表示します:

`aws lambda get-function-concurrency --function-name {{name}}`

- この関数を呼び出すことができる AWS サービスをリストします:

`aws lambda get-policy --function-name {{name}}`
