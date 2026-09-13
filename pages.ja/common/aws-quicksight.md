# aws quicksight

> AWS QuickSight エンティティを作成、削除、一覧表示、検索、更新する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/quicksight/>。

- データセットを一覧表示する:

`aws quicksight list-data-sets --aws-account-id {{aws_account_id}}`

- ユーザーを一覧表示する:

`aws quicksight list-users --aws-account-id {{aws_account_id}} --namespace default`

- グループを一覧表示する:

`aws quicksight list-groups --aws-account-id {{aws_account_id}} --namespace default`

- ダッシュボードを一覧表示する:

`aws quicksight list-dashboards --aws-account-id {{aws_account_id}}`

- データセットに関する詳細情報を表示する:

`aws quicksight describe-data-set --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`

- データセットにアクセスできるユーザーと、データセットに対してどのようなアクションを実行できるかを表示する:

`aws quicksight describe-data-set-permissions --aws-account-id {{aws_account_id}} --data-set-id {{data_set_id}}`
