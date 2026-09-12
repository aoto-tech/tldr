# aws pricing

> アマゾン ウェブ サービスのサービス、製品、価格情報をクエリします。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/pricing/>。

- 特定の地域のサービス コードを一覧表示します:

`aws pricing describe-services --region {{us-east-1}}`

- 特定のリージョン内の特定のサービス コードの属性をリストします:

`aws pricing describe-services --service-code {{AmazonEC2}} --region {{us-east-1}}`

- 特定の地域のサービス コードの価格情報を出力します:

`aws pricing get-products --service-code {{AmazonEC2}} --region {{us-east-1}}`

- 特定のリージョンのサービス コードの特定の属性の値をリストします:

`aws pricing get-attribute-values --service-code {{AmazonEC2}} --attribute-name {{instanceType}} --region {{us-east-1}}`

- インスタンスのタイプと場所のフィルターを使用して、サービス コードの価格情報を出力します:

`aws pricing get-products --service-code {{AmazonEC2}} --filters "{{Type=TERM_MATCH,Field=instanceType,Value=m5.xlarge}}" "{{Type=TERM_MATCH,Field=location,Value=US East (N. Virginia)}}" --region {{us-east-1}}`
