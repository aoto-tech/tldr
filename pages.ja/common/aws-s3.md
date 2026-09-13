# aws s3

> CLI for AWS S3 - Web サービス インターフェイスを通じてストレージを提供します。
> `cp` などの一部のサブコマンドには、独自の使用法ドキュメントがあります。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/>。

- バケット内のファイルを表示します:

`aws s3 ls {{bucket_name}}`

- ディレクトリ内のファイルをローカルからバケットに同期します:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}}`

- ファイルとディレクトリをバケットからローカルに同期します:

`aws s3 sync s3://{{bucket_name}} {{path/to/target}}`

- 除外を含むディレクトリ内のファイルを同期します:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*`

- バケットからファイルを削除します:

`aws s3 rm s3://{{bucket}}/{{path/to/file}}`

- 変更のみをプレビュー:

`aws s3 {{any_command}} --dryrun`
