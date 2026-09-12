# aws route53

> AWS Route53 の CLI - Route 53 は、可用性が高く、スケーラブルなドメイン ネーム システム (DNS) Web サービスです。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/route53/>。

- すべてのホストゾーン (プライベートおよびパブリック) をリストします:

`aws route53 list-hosted-zones`

- ゾーン内のすべてのレコードを表示します:

`aws route53 list-resource-record-sets --hosted-zone-id {{zone_id}}`

- リクエスト識別子を使用して新しいパブリック ゾーンを作成し、操作を安全に再試行します:

`aws route53 create-hosted-zone --name {{name}} --caller-reference {{request_identifier}}`

- ゾーンを削除します (ゾーンにデフォルト以外の SOA および NS レコードがある場合、コマンドは失敗します):

`aws route53 delete-hosted-zone --id {{zone_id}}`

- 指定されたゾーンの Amazon サーバーによる DNS 解決をテストします:

`aws route53 test-dns-answer --hosted-zone-id {{zone_id}} --record-name {{name}} --record-type {{type}}`
