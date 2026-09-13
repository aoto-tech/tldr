# aws s3 mv

> ローカル ファイルまたは S3 オブジェクトをローカルまたは S3 内の別の場所に移動します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/mv.html>。

- ファイルをローカルから指定したバケットに移動します:

`aws s3 mv {{path/to/local_file}} s3://{{bucket_name}}/{{path/to/remote_file}}`

- 特定の S3 オブジェクトを別のバケットに移動します:

`aws s3 mv s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}/{{path/to/target}}`

- 特定の S3 オブジェクトを元の名前を維持したまま別のバケットに移動します:

`aws s3 mv s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}`

- ヘルプを表示する:

`aws s3 mv help`
