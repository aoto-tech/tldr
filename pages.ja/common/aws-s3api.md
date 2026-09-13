# aws s3api

> Amazon S3 バケットを作成および削除し、バケットのプロパティを編集します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3api/>。

- 特定のリージョンにバケットを作成します:

`aws s3api create-bucket --bucket {{bucket_name}} --region {{region}} --create-bucket-configuration LocationConstraint={{region}}`

- バケットを削除します:

`aws s3api delete-bucket --bucket {{bucket_name}}`

- バケットをリストします:

`aws s3api list-buckets`

- バケット内のオブジェクトをリストし、各オブジェクトのキーとサイズのみを表示します:

`aws s3api list-objects --bucket {{bucket_name}} --query '{{Contents[].{Key: Key, Size: Size}}}'`

- オブジェクトをバケットに追加します:

`aws s3api put-object --bucket {{bucket_name}} --key {{object_key}} --body {{path/to/file}}`

- バケットからオブジェクトをダウンロードします (出力ファイルは常に最後の引数です):

`aws s3api get-object --bucket {{bucket_name}} --key {{object_key}} {{path/to/output_file}}`

- Amazon S3 バケット ポリシーを指定したバケットに適用します:

`aws s3api put-bucket-policy --bucket {{bucket_name}} --policy file://{{path/to/bucket_policy.json}}`

- 指定したバケットから Amazon S3 バケット ポリシーをダウンロードします:

`aws s3api get-bucket-policy --bucket {{bucket_name}} --query Policy --output {{json|table|text|yaml|yaml-stream}} > {{path/to/bucket_policy}}`
