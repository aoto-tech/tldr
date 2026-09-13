# aws lambda

> サーバーのプロビジョニングや管理を行わずにコードを実行するためのコンピューティングサービスである AWS Lambda を使用する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/lambda/>。

- 関数を実行する:

`aws lambda invoke --function-name {{name}} {{path/to/response.json}}`

- JSON 形式の入力ペイロードを使用して関数を実行する:

`aws lambda invoke --function-name {{name}} --payload {{json}} {{path/to/response.json}}`

- 関数を一覧表示する:

`aws lambda list-functions`

- 関数の設定を表示する:

`aws lambda get-function-configuration --function-name {{name}}`

- 関数エイリアスを一覧表示する:

`aws lambda list-aliases --function-name {{name}}`

- 関数の予約済み同時実行設定を表示する:

`aws lambda get-function-concurrency --function-name {{name}}`

- この関数を呼び出すことができる AWS サービスを一覧表示する:

`aws lambda get-policy --function-name {{name}}`
