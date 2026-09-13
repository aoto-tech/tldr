# aws pricing

> Amazon Web Servicesのサービス、製品、価格情報をクエリする。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/pricing/>。

- 特定のリージョンのサービスコードを一覧表示する:

`aws pricing describe-services --region {{us-east-1}}`

- 特定のリージョン内の特定のサービスコードの属性を一覧表示する:

`aws pricing describe-services --service-code {{AmazonEC2}} --region {{us-east-1}}`

- 特定のリージョンのサービスコードの価格情報を出力する:

`aws pricing get-products --service-code {{AmazonEC2}} --region {{us-east-1}}`

- 特定のリージョンのサービスコードの特定の属性の値を一覧表示する:

`aws pricing get-attribute-values --service-code {{AmazonEC2}} --attribute-name {{instanceType}} --region {{us-east-1}}`

- インスタンスのタイプと場所のフィルターを使用して、サービスコードの価格情報を出力する:

`aws pricing get-products --service-code {{AmazonEC2}} --filters "{{Type=TERM_MATCH,Field=instanceType,Value=m5.xlarge}}" "{{Type=TERM_MATCH,Field=location,Value=US East (N. Virginia)}}" --region {{us-east-1}}`
