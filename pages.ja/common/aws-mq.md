# aws mq

> AWS でメッセージブローカーを定義して操作する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/mq/>。

- ブローカーを作成する:

`aws mq create-broker --host-instance-type {{instance_type}} --broker-name {{broker_name}} --engine-type {{ACTIVEMQ|RABBITMQ}} {{--publicly-accessible|--no-publicly-accessible}}`

- すべてのブローカーを一覧表示する:

`aws mq list-brokers`

- 特定のブローカーの詳細を表示する:

`aws mq describe-broker --broker-id {{broker_id}}`
