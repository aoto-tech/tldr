# aws s3 presign

> Amazon S3 オブジェクトの署名付き URL を生成します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/presign.html>。

- 1 時間有効な、特定の S3 オブジェクトの署名付き URL を生成します:

`aws s3 presign s3://{{bucket_name}}/{{path/to/file}}`

- 特定の有効期間中有効な署名付き URL を生成します:

`aws s3 presign s3://{{bucket_name}}/{{path/to/file}} --expires-in {{duration_in_seconds}}`

- ヘルプを表示する:

`aws s3 presign help`
