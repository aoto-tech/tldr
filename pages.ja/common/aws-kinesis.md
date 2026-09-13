# aws kinesis

> Amazon Kinesis Data Streams と対話する。これは、ストリーミングビッグデータのリアルタイム処理のために弾力的に拡張するサービスである。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>。

- アカウント内のすべてのストリームを表示する:

`aws kinesis list-streams`

- 1 つのレコードを Kinesis ストリームに書き込む:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data {{base64_encoded_message}}`

- インライン Base64 エンコーディングを使用してレコードを Kinesis ストリームに書き込む:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data "$( echo "{{my raw message}}" | base64 )"`

- ストリームで利用可能なシャードを一覧表示する:

`aws kinesis list-shards --stream-name {{name}}`

- ストリームのシャード内の最も古いメッセージから読み取るためのシャードイテレータを取得する:

`aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}`

- シャードイテレータを使用して、シャードからレコードを読み取る:

`aws kinesis get-records --shard-iterator {{iterator}}`
