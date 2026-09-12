# aws rds

> リレーショナル データベースをセットアップ、操作、スケーリングするための Web サービスである AWS Relational Database Service を使用します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/rds/>。

- 特定の RDS サブコマンドのヘルプを表示します:

`aws rds {{subcommand}} help`

- インスタンスを停止します:

`aws rds stop-db-instance --db-instance-identifier {{instance_identifier}}`

- インスタンスを開始します:

`aws rds start-db-instance --db-instance-identifier {{instance_identifier}}`

- RDS インスタンスを変更します:

`aws rds modify-db-instance --db-instance-identifier {{instance_identifier}} {{parameters}} --apply-immediately`

- RDS インスタンスに更新を適用します:

`aws rds apply-pending-maintenance-action --resource-identifier {{database_arn}} --apply-action {{system-update}} --opt-in-type {{immediate}}`

- インスタンス識別子を変更します:

`aws rds modify-db-instance --db-instance-identifier {{old_instance_identifier}} --new-db-instance-identifier {{new_instance_identifier}}`

- インスタンスを再起動します:

`aws rds reboot-db-instance --db-instance-identifier {{instance_identifier}}`

- インスタンスを削除します:

`aws rds delete-db-instance --db-instance-identifier {{instance_identifier}} --final-db-snapshot-identifier {{snapshot_identifier}} --delete-automated-backups`
