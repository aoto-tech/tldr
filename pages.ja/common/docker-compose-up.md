# docker compose up

> Compose ファイルで定義された Docker サービスを開始して実行します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/compose/up/>。

- docker-compose ファイルで定義されているすべてのサービスを開始します:

`docker compose up`

- バックグラウンドでサービスを開始します (分離モード):

`docker compose up {{[-d|--detach]}}`

- サービスを開始し、開始する前にイメージを再構築します:

`docker compose up --build`

- 特定のサービスのみを開始します:

`docker compose up {{service1 service2 ...}}`

- カスタム構成ファイルを使用してサービスを開始します:

`docker compose {{[-f|--file]}} {{path/to/config}} up`

- サービスを開始し、孤立したコンテナを削除します:

`docker compose up --remove-orphans`

- スケーリングされたインスタンスでサービスを開始します:

`docker compose up --scale {{service}}={{count}}`

- サービスを開始し、タイムスタンプ付きのログを表示します:

`docker compose up --timestamps`
