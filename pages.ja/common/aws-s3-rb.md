# aws s3 rb

> 空の S3 バケットを削除します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/rb.html>。

- 空の S3 バケットを削除します:

`aws s3 rb s3://{{bucket_name}}`

- S3 バケットとそのバージョン管理されていないオブジェクトを強制的に削除します (バージョン管理されたオブジェクトが存在する場合はクラッシュします):

`aws s3 rb s3://{{bucket_name}} --force`
