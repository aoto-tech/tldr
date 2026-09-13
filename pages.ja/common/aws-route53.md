# aws route53

> AWS Route53 の CLI - Route 53 は、可用性が高く、スケーラブルなドメインネームシステム (DNS) Web サービスである。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/route53/>。

- すべてのホストゾーン (プライベートおよびパブリック) を一覧表示する:

`aws route53 list-hosted-zones`

- ゾーン内のすべてのレコードを表示する:

`aws route53 list-resource-record-sets --hosted-zone-id {{zone_id}}`

- 操作を安全に再試行できるよう、リクエスト識別子を指定して新しいパブリックゾーンを作成する:

`aws route53 create-hosted-zone --name {{name}} --caller-reference {{request_identifier}}`

- ゾーンを削除する (ゾーンにデフォルト以外の SOA および NS レコードがある場合、コマンドは失敗する):

`aws route53 delete-hosted-zone --id {{zone_id}}`

- 指定されたゾーンの Amazon サーバーによる DNS 解決をテストする:

`aws route53 test-dns-answer --hosted-zone-id {{zone_id}} --record-name {{name}} --record-type {{type}}`
