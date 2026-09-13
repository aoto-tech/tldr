# aws lightsail

> Amazon Lightsail リソースを管理する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/lightsail/>。

- すべての仮想プライベートサーバーまたはインスタンスを一覧表示する:

`aws lightsail get-instances`

- すべてのバンドル (インスタンスプラン) を一覧表示する:

`aws lightsail list-bundles`

- 利用可能なすべてのインスタンスイメージまたはブループリントを一覧表示する:

`aws lightsail list-blueprints`

- インスタンスを作成する:

`aws lightsail create-instances --instance-names {{name}} --availability-zone {{region}} --bundle-id {{nano_2_0}} --blueprint-id {{blueprint_id}}`

- 特定のインスタンスの状態を出力する:

`aws lightsail get-instance-state --instance-name {{name}}`

- 特定のインスタンスを停止する:

`aws lightsail stop-instance --instance-name {{name}}`

- 特定のインスタンスを削除する:

`aws lightsail delete-instance --instance-name {{name}}`
