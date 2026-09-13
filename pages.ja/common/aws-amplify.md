# aws amplify

> 安全でスケーラブルなモバイルおよび Web アプリケーションを構築するための開発プラットフォーム。
> 詳細情報: <https://docs.aws.amazon.com/cli/latest/reference/amplify/>。

- 新しい Amplify アプリを作成する:

`aws amplify create-app --name {{app_name}} --description {{description}} --repository {{repo_url}} --platform {{platform}} --environment-variables {{env_vars}} --tags {{tags}}`

- 既存の Amplify アプリを削除する:

`aws amplify delete-app --app-id {{app_id}}`

- 特定の Amplify アプリの詳細を取得する:

`aws amplify get-app --app-id {{app_id}}`

- すべての Amplify アプリを一覧表示する:

`aws amplify list-apps`

- Amplify アプリの設定を更新する:

`aws amplify update-app --app-id {{app_id}} --name {{new_name}} --description {{new_description}} --repository {{new_repo_url}} --environment-variables {{new_env_vars}} --tags {{new_tags}}`

- 新しいバックエンド環境を Amplify アプリに追加する:

`aws amplify create-backend-environment --app-id {{app_id}} --environment-name {{env_name}} --deployment-artifacts {{artifacts}}`

- Amplify アプリからバックエンド環境を削除する:

`aws amplify delete-backend-environment --app-id {{app_id}} --environment-name {{env_name}}`

- Amplify アプリ内のすべてのバックエンド環境を一覧表示する:

`aws amplify list-backend-environments --app-id {{app_id}}`
