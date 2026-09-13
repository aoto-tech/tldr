# aws s3 mb

> S3バケットを作成する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/mb.html>。

- S3 バケットを作成する:

`aws s3 mb s3://{{bucket_name}}`

- 特定のリージョンに S3 バケットを作成する:

`aws s3 mb s3://{{bucket_name}} --region {{region}}`

- ヘルプを表示する:

`aws s3 mb help`
