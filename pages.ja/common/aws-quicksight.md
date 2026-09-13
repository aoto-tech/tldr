# aws quicksight

> AWS QuickSight エンティティを作成、削除、リスト、検索、更新します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>。

- データセットをリストします:

`aws quicksight list-data-sets --aws-account-id {{aws_account_id}}`

- ユーザーをリストします:

`aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default`

- グループをリストします:

`aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default`

- ダッシュボードをリストします:

`aws quicksight list-dashboards --aws-account-id {{aws_account_id}}`

- データセットに関する詳細情報を表示します:

`aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`

- データセットにアクセスできるユーザーと、データセットに対してどのようなアクションを実行できるかを表示します:

`aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`
