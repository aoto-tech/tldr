# aws mq

> AWS でメッセージ ブローカーを定義して操作します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/mq/>。

- ブローカーを作成します:

`aws mq create-broker --host-instance-type {{instance_type}} --broker-name {{broker_name}} --engine-type {{ACTIVEMQ|RABBITMQ}} {{--publicly-accessible|--no-publicly-accessible}}`

- すべてのブローカーをリストします:

`aws mq list-brokers`

- 特定のブローカーについて説明します:

`aws mq describe-broker --broker-id {{broker_id}}`
