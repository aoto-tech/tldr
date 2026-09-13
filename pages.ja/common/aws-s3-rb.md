# aws s3 rb

> 空の S3 バケットを削除する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/rb.html>。

- 空の S3 バケットを削除する:

`aws s3 rb s3://{{bucket_name}}`

- S3 バケットとそのバージョン管理されていないオブジェクトを強制的に削除する (バージョン管理されたオブジェクトが存在する場合は失敗する):

`aws s3 rb s3://{{bucket_name}} --force`
