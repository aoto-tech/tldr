# aws lightsail

> Amazon Lightsail リソースを管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/lightsail/>。

- すべての仮想プライベート サーバーまたはインスタンスをリストします:

`aws lightsail get-instances`

- すべてのバンドル (インスタンス プラン) をリストします:

`aws lightsail list-bundles`

- 利用可能なすべてのインスタンス イメージまたはブループリントをリストします:

`aws lightsail list-blueprints`

- インスタンスを作成します:

`aws lightsail create-instances --instance-names {{name}} --availability-zone {{region}} --bundle-id {{nano_2_0}} --blueprint-id {{blueprint_id}}`

- 特定のインスタンスの状態を出力します:

`aws lightsail get-instance-state --instance-name {{name}}`

- 特定のインスタンスを停止します:

`aws lightsail stop-instance --instance-name {{name}}`

- 特定のインスタンスを削除します:

`aws lightsail delete-instance --instance-name {{name}}`
