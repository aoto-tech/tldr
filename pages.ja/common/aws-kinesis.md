# aws kinesis

> Amazon Kinesis Data Streams と対話します。これは、ストリーミングビッグデータのリアルタイム処理のために弾力的に拡張するサービスです。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/kinesis/index.html#cli-aws-kinesis>。

- アカウント内のすべてのストリームを表示します:

`aws kinesis list-streams`

- 1 つのレコードを Kinesis ストリームに書き込みます:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data {{base64_encoded_message}}`

- インライン Base64 エンコーディングを使用してレコードを Kinesis ストリームに書き込みます:

`aws kinesis put-record --stream-name {{name}} --partition-key {{key}} --data "$( echo "{{my raw message}}" | base64 )"`

- ストリームで利用可能なシャードをリストします:

`aws kinesis list-shards --stream-name {{name}}`

- ストリームのシャード内の最も古いメッセージから読み取るためのシャード イテレータを取得します:

`aws kinesis get-shard-iterator --shard-iterator-type TRIM_HORIZON --stream-name {{name}} --shard-id {{id}}`

- シャード反復子を使用して、シャードからレコードを読み取ります:

`aws kinesis get-records --shard-iterator {{iterator}}`
