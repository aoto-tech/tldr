# aws s3 rm

> S3 オブジェクトを削除する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/rm.html>。

- 特定の S3 オブジェクトを削除する:

`aws s3 rm s3://{{bucket_name}}/{{path/to/file}}`

- 特定の S3 オブジェクトを削除せずに削除をプレビューする (ドライラン):

`aws s3 rm s3://{{bucket_name}}/{{path/to/file}} --dryrun`

- 特定の S3 アクセスポイントからオブジェクトを削除する:

`aws s3 rm s3://arn:aws:s3:{{region}}:{{account_id}}:{{access_point}}/{{access_point_name}}/{{object_key}}`

- バケットからすべてのオブジェクトを削除する (バケットを空にする):

`aws s3 rm s3://{{bucket_name}} --recursive`

- ヘルプを表示する:

`aws s3 rm help`
