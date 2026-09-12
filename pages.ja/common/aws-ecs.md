# aws ecs

> Elastic Container Service (ECS) クラスターを管理します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ecs/>。

- タスク定義をリストします:

`aws ecs list-task-definitions`

- タスク定義を説明します:

`aws ecs describe-task-definition --task-definition {{task_definition}}`

- タスク定義を作成するか、改訂を行います:

`aws ecs register-task-definition --cli-input-json file://{{path_to_file.json}}`

- タスク定義を INACTIVE としてマークして登録を解除します:

`aws ecs deregister-task-definition --task-definition {{task_definition}}:{{revision_number}}`

- 特定のクラスター内のサービスをリストします:

`aws ecs list-services --cluster {{cluster_name}}`

- クラスター内の 1 つ以上のサービスを説明します:

`aws ecs describe-services --services {{service_name}} {{service_name}} --cluster {{cluster_name}}`

- サービスを更新し、新しいデプロイメントを強制します:

`aws ecs update-service --cluster {{cluster_name}} --service {{service_name}} --task-definition {{task_definition_arn}} --force-new-deployment`

- 1 つ以上のサービスが成功するまで待ちます:

`aws ecs wait services-stable --cluster {{cluster_name}} --services {{service_name}} {{service_name}}`
