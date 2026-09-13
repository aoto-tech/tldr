# aws s3 website

> バケットの Web サイト設定を設定する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/website.html>。

- バケットを静的 Web サイトとして設定する:

`aws s3 website {{s3://bucket-name}} --index-document {{index.html}}`

- Web サイトのエラーページを設定する:

`aws s3 website {{s3://bucket-name}} --index-document {{index.html}} --error-document {{error.html}}`
