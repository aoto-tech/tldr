# aws sns

> Amazon Simple Notice Service のトピックとサブスクリプションを作成し、メッセージを送受信し、イベントとログを監視します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sns/>。

- 特定のタイプのすべてのオブジェクトをリストします:

`aws sns list-{{origination-numbers|phone-numbers-opted-out|platform-applications|sms-sandbox-phone-numbers|subscriptions|topics}}`

- 特定の名前でトピックを作成し、その Amazon リソースネーム (ARN) を表示します:

`aws sns create-topic --name {{name}}`

- 特定の ARN を使用してトピックに電子メール アドレスをサブスクライブし、サブスクリプション ARN を表示します:

`aws sns subscribe --topic-arn {{topic_ARN}} --protocol email --notification-endpoint {{email}}`

- 特定のトピックまたは電話番号にメッセージをパブリッシュし、メッセージ ID を表示します:

`aws sns publish {{--topic-arn "arn:aws:sns:us-west-2:123456789012:topic-name"||--phone-number +1-555-555-0100}} --message file://{{path/to/file}}`

- 特定の ARN を持つサブスクリプションをトピックから削除します:

`aws sns unsubscribe --subscription-arn {{subscription_ARN}}`

- プラットフォーム エンドポイントを作成します:

`aws sns create-platform-endpoint --platform-application-arn {{platform_application_ARN}} --token {{token}}`

- トピックのアクセス制御ポリシーにステートメントを追加します:

`aws sns add-permission --topic-arn {{topic_ARN}} --label {{topic_label}} --aws-account-id {{account_id}} --action-name {{AddPermission|CreatePlatformApplication|DeleteEndpoint|GetDataProtectionPolicy|GetEndpointAttributes|Subscribe|...}}`

- 特定の ARN を使用してトピックにタグを追加します:

`aws sns tag-resource --resource-arn {{topic_ARN}} --tags {{Key=tag1_key Key=tag2_key,Value=tag2_value ...}}`
