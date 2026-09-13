# aws s3

> AWS S3 の CLI。Web サービスインターフェイスを通じてストレージを提供する。
> `cp` のような一部のサブコマンドには、独自の使用法ドキュメントがある。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/>。

- バケット内のファイルを表示する:

`aws s3 ls {{bucket_name}}`

- ディレクトリ内のファイルをローカルからバケットに同期する:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}}`

- ファイルとディレクトリをバケットからローカルに同期する:

`aws s3 sync s3://{{bucket_name}} {{path/to/target}}`

- 除外を含むディレクトリ内のファイルを同期する:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*`

- バケットからファイルを削除する:

`aws s3 rm s3://{{bucket}}/{{path/to/file}}`

- 変更のみをプレビュー:

`aws s3 {{any_command}} --dryrun`
