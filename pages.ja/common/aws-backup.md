# aws backup

> アマゾン ウェブ サービスのサービスとその関連データを保護するために設計された統合バックアップ サービス。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/backup/>。

- 特定の BackupPlanId の BackupPlan 詳細を返します:

`aws backup get-backup-plan --backup-plan-id {{id}}`

- 特定のバックアップ プラン名とバックアップ ルールを使用してバックアップ プランを作成します:

`aws backup create-backup-plan --backup-plan {{plan}}`

- 特定のバックアップ計画を削除します:

`aws backup delete-backup-plan --backup-plan-id {{id}}`

- 現在のアカウントのアクティブなバックアップ プランをすべてリストします:

`aws backup list-backup-plans`

- レポート ジョブに関する詳細を表示します:

`aws backup list-report-jobs`
