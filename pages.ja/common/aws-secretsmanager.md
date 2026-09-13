# aws secretsmanager

> シークレットを保存、管理、取得する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/secretsmanager/>。

- 現在のアカウントのシークレットマネージャーによって保存されているシークレットを表示する:

`aws secretsmanager list-secrets`

- すべてのシークレットを一覧表示するが、シークレット名と ARN のみを表示する (簡単に表示できる):

`aws secretsmanager list-secrets --query 'SecretList[*].{Name: Name, ARN: ARN}'`

- シークレットを作成する:

`aws secretsmanager create-secret --name {{name}} --description "{{secret_description}}" --secret-string '{{secret}}'`

- シークレットを削除する (回復期間なしですぐに削除するには、`--force-delete-without-recovery` を追加する):

`aws secretsmanager delete-secret --secret-id {{name|arn}}`

- シークレットテキストを除くシークレットの詳細を表示する:

`aws secretsmanager describe-secret --secret-id {{name|arn}}`

- シークレットの値を取得する (シークレットの最新バージョンを取得するには、`--version-stage` を省略する):

`aws secretsmanager get-secret-value --secret-id {{name|arn}} --version-stage {{version_of_secret}}`

- Lambda 関数を使用してシークレットをすぐにローテーションする:

`aws secretsmanager rotate-secret --secret-id {{name|arn}} --rotation-lambda-arn {{arn_of_lambda_function}}`

- Lambda 関数を使用して、シークレットを 30 日ごとに自動的にローテーションする:

`aws secretsmanager rotate-secret --secret-id {{name|arn}} --rotation-lambda-arn {{arn_of_lambda_function}} --rotation-rules AutomaticallyAfterDays={{30}}`
