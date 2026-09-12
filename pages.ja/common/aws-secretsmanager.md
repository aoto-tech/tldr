# aws secretsmanager

> シークレットを保存、管理、取得します。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/secretsmanager/>。

- 現在のアカウントのシークレット マネージャーによって保存されているシークレットを表示します:

`aws secretsmanager list-secrets`

- すべてのシークレットをリストしますが、シークレット名と ARN のみを表示します (簡単に表示できます):

`aws secretsmanager list-secrets --query 'SecretList[*].{Name: Name, ARN: ARN}'`

- シークレットを作成します:

`aws secretsmanager create-secret --name {{name}} --description "{{secret_description}}" --secret-string '{{secret}}'`

- シークレットを削除します (回復期間なしですぐに削除するには、`--force-delete-without-recovery` を追加します):

`aws secretsmanager delete-secret --secret-id {{name|arn}}`

- シークレット テキストを除くシークレットの詳細を表示します:

`aws secretsmanager describe-secret --secret-id {{name|arn}}`

- シークレットの値を取得します (シークレットの最新バージョンを取得するには、`--version-stage` を省略します):

`aws secretsmanager get-secret-value --secret-id {{name|arn}} --version-stage {{version_of_secret}}`

- Lambda 関数を使用してシークレットをすぐにローテーションします:

`aws secretsmanager rotate-secret --secret-id {{name|arn}} --rotation-lambda-arn {{arn_of_lambda_function}}`

- Lambda 関数を使用して、シークレットを 30 日ごとに自動的にローテーションします:

`aws secretsmanager rotate-secret --secret-id {{name|arn}} --rotation-lambda-arn {{arn_of_lambda_function}} --rotation-rules AutomaticallyAfterDays={{30}}`
