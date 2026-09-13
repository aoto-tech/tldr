# aws ecr

> コンテナイメージをプッシュ、プル、管理する。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/ecr/>。

- デフォルトのレジストリを使用して Docker を認証する (ユーザー名は AWS):

`aws ecr get-login-password --region {{region}} | {{docker login}} --username AWS --password-stdin {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com`

- リポジトリを作成する:

`aws ecr create-repository --repository-name {{repository}} --image-scanning-configuration scanOnPush={{true|false}} --region {{region}}`

- ローカルイメージに ECR のタグを付ける:

`docker tag {{container_name}}:{{tag}} {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}`

- イメージをリポジトリにプッシュする:

`docker push {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}`

- リポジトリからイメージをプルする:

`docker pull {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}`

- リポジトリからイメージを削除する:

`aws ecr batch-delete-image --repository-name {{repository}} --image-ids imageTag={{latest}}`

- リポジトリを削除する:

`aws ecr delete-repository --repository-name {{repository}} --force`

- リポジトリ内のイメージを一覧表示する:

`aws ecr list-images --repository-name {{repository}}`
