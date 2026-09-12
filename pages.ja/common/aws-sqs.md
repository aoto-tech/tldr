# aws sqs

> AWS SQS サービスのキューを作成、削除し、キューにメッセージを送信します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/sqs/>。

- 使用可能なキューをすべてリストします:

`aws sqs list-queues`

- 特定のキューの URL を表示します:

`aws sqs get-queue-url --queue-name {{queue_name}}`

- JSON 形式のファイルから特定の属性を持つキューを作成します:

`aws sqs create-queue --queue-name {{queue_name}} --attributes {{file://path/to/attributes_file.json}}`

- 特定のメッセージをキューに送信します:

`aws sqs send-message --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --message-body "{{message_body}}" --delay-seconds {{delay}} --message-attributes {{file://path/to/attributes_file.json}}`

- 指定されたメッセージをキューから削除します:

`aws sqs delete-message --queue-url {{https://queue_url}} --receipt-handle {{receipt_handle}}`

- 特定のキューを削除します:

`aws sqs delete-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- 指定されたキューからすべてのメッセージを削除します:

`aws sqs purge-queue --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}}`

- 特定の AWS アカウントがメッセージをキューに送信できるようにします:

`aws sqs add-permission --queue-url https://sqs.{{region}}.amazonaws.com/{{queue_name}} --label {{permission_name}} --aws-account-ids {{account_id}} --actions SendMessage`
