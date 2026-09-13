# aws s3 cp

> ローカルファイルまたは S3 オブジェクトをローカルまたは S3 内の別の場所にコピーする。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/cp.html>。

- ファイルをローカルから特定のバケットにコピーする:

`aws s3 cp {{path/to/file}} s3://{{bucket_name}}/{{path/to/remote_file}}`

- 特定の S3 オブジェクトを別のバケットにコピーする:

`aws s3 cp s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}/{{path/to/target}}`

- 特定の S3 オブジェクトを元の名前を維持したまま別のバケットにコピーする:

`aws s3 cp s3://{{bucket_name1}}/{{path/to/file}} s3://{{bucket_name2}}`

- S3 オブジェクトをローカルディレクトリに再帰的にコピーする:

`aws s3 cp s3://{{bucket_name}} . --recursive`

- ヘルプを表示する:

`aws s3 cp help`
