# aws s3 ls

> AWS S3 バケット、フォルダー (プレフィックス)、およびファイル (オブジェクト) を一覧表示します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/ls.html>。

- すべてのバケットをリストします:

`aws s3 ls`

- バケットのルートにあるファイルとフォルダーを一覧表示します (`s3://` はオプション):

`aws s3 ls s3://{{bucket_name}}`

- ディレクトリ内のファイルとフォルダーを直接一覧表示します:

`aws s3 ls {{bucket_name}}/{{path/to/directory}}/`

- バケット内のすべてのファイルをリストします:

`aws s3 ls --recursive {{bucket_name}}`

- 指定されたプレフィックスを持つパス内のすべてのファイルをリストします:

`aws s3 ls --recursive {{bucket_name}}/{{path/to/directory}}/{{prefix}}`

- ヘルプを表示する:

`aws s3 ls help`
