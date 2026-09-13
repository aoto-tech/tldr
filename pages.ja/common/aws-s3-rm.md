# aws s3 rm

> S3 オブジェクトを削除します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/rm.html>。

- 特定の S3 オブジェクトを削除します:

`aws s3 rm s3://{{bucket_name}}/{{path/to/file}}`

- 特定の S3 オブジェクトを削除せずに削除をプレビューします (ドライラン):

`aws s3 rm s3://{{bucket_name}}/{{path/to/file}} --dryrun`

- 特定の S3 アクセス ポイントからオブジェクトを削除します:

`aws s3 rm s3://arn:aws:s3:{{region}}:{{account_id}}:{{access_point}}/{{access_point_name}}/{{object_key}}`

- バケットからすべてのオブジェクトを削除します (バケットを空にします):

`aws s3 rm s3://{{bucket_name}} --recursive`

- ヘルプを表示する:

`aws s3 rm help`
