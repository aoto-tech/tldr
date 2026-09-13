# aws s3 sync

> ローカルシステムと S3 バケット間、または S3 バケット間でファイルとディレクトリを再帰的に同期する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/sync.html>。

- ディレクトリ内のファイルをローカルからバケットに同期する:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}}/{{path/to/remote_location}}`

- ディレクトリ内のファイルをバケットからローカルに同期する:

`aws s3 sync s3://{{bucket_name}}/{{path/to/remote_location}} {{path/to/directory}}`

- 2 つのバケット間でオブジェクトを同期する:

`aws s3 sync s3://{{bucket_source_name}}/{{path/to/remote_location}} s3://{{bucket_target_name}}/{{path/to/remote_location}}`

- 特定のファイルまたはディレクトリを除外しながら、ローカルファイルを S3 に同期する:

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}}/{{path/to/remote_location}} --exclude {{path/to/file}} --exclude {{path/to/directory}}/*`

- バケット間でオブジェクトを同期し、ソースにない宛先ファイルを削除する:

`aws s3 sync s3://{{bucket_source_name}}/{{path/to/remote_location}} s3://{{bucket_target_name}}/{{path/to/remote_location}} --delete`

- 詳細オプションを使用して S3 に同期する (ACL とストレージクラスを設定):

`aws s3 sync {{path/to/local_directory}} s3://{{bucket_name}}/{{path/to/remote_location}} --acl {{private|public-read}} --storage-class {{STANDARD_IA|GLACIER}}`

- ファイルを S3 に同期し、変更されていないファイルをスキップする (サイズと変更時間を比較):

`aws s3 sync {{path/to/directory}} s3://{{bucket_name}}/{{path/to/remote_location}} --size-only`

- ヘルプを表示する:

`aws s3 sync help`
