# aws s3 website

> バケットの Web サイト構成を設定します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/s3/website.html>。

- バケットを静的 Web サイトとして設定します:

`aws s3 website {{s3://bucket-name}} --index-document {{index.html}}`

- Web サイトのエラー ページを構成します:

`aws s3 website {{s3://bucket-name}} --index-document {{index.html}} --error-document {{error.html}}`
