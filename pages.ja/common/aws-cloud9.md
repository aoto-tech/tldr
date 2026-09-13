# aws cloud9

> Cloud9 の管理 - クラウドでソフトウェアをコーディング、構築、実行、テスト、デバッグ、リリースするためのツールのコレクションです。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/cloud9/>。

- すべての Cloud9 開発環境識別子をリストします:

`aws cloud9 list-environments`

- Cloud9 開発環境を作成します:

`aws cloud9 create-environment-ec2 --name {{name}} --instance-type {{instance_type}}`

- Cloud9 開発環境に関する情報を表示します:

`aws cloud9 describe-environments --environment-ids {{environment_ids}}`

- 環境メンバーを Cloud9 開発環境に追加します:

`aws cloud9 create-environment-membership --environment-id {{environment_id}} --user-arn {{user_arn}} --permissions {{permissions}}`

- Cloud9 開発環境のステータス情報を表示します:

`aws cloud9 describe-environment-status --environment-id {{environment_id}}`

- Cloud9 環境を削除します:

`aws cloud9 delete-environment --environment-id {{environment_id}}`

- 開発環境から環境メンバーを削除します:

`aws cloud9 delete-environment-membership --environment-id {{environment_id}} --user-arn {{user_arn}}`
