# aws backup

> Amazon Web Servicesのサービスとその関連データを保護するために設計された統合バックアップサービス。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/backup/>。

- 特定の BackupPlanId の BackupPlan 詳細を返す:

`aws backup get-backup-plan --backup-plan-id {{id}}`

- 特定のバックアッププラン名とバックアップルールを使用してバックアッププランを作成する:

`aws backup create-backup-plan --backup-plan {{plan}}`

- 特定のバックアッププランを削除する:

`aws backup delete-backup-plan --backup-plan-id {{id}}`

- 現在のアカウントのアクティブなバックアッププランをすべて一覧表示する:

`aws backup list-backup-plans`

- レポートジョブに関する詳細を表示する:

`aws backup list-report-jobs`
