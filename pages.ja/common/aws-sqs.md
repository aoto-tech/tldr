# aws sqs

> AWS SQS サービスのキューを作成、削除し、キューにメッセージを送信する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sqs/>。

- 使用可能なキューをすべて一覧表示する:

`aws sqs list-queues`

- 特定のキューの URL を表示する:

`aws sqs get-queue-url --queue-name {{queue_name}}`

- JSON 形式のファイルから特定の属性を持つキューを作成する:

`aws sqs create-queue --queue-name {{queue_name}} --attributes {{file://path/to/attributes_file.json}}`

- 特定のメッセージをキューに送信する:

`aws sqs send-message --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --message-body "{{message_body}}" --delay-seconds {{delay}} --message-attributes {{file://path/to/attributes_file.json}}`

- 指定されたメッセージをキューから削除する:

`aws sqs delete-message --queue-url {{https://queue_url}} --receipt-handle {{receipt_handle}}`

- 特定のキューを削除する:

`aws sqs delete-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- 指定されたキューからすべてのメッセージを削除する:

`aws sqs purge-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- 特定の AWS アカウントがメッセージをキューに送信できるようにする:

`aws sqs add-permission --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --label {{permission_name}} --aws-account-ids {{account_id}} --actions SendMessage`
