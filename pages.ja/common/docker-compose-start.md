# docker compose start

> サービス用の既存のコンテナを開始します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/compose/start/>。

- すべてのサービスの既存のコンテナを開始します:

`docker compose start`

- 1 つ以上のサービスの既存のコンテナを開始します:

`docker compose start {{service1 service2 ...}}`

- 既存のコンテナの起動をシミュレートします:

`docker compose start --dry-run`

- 既存のコンテナを起動し、サービスが実行されるか正常になるまで待ちます:

`docker compose start --wait`

- 既存のコンテナを起動し、指定された秒数まで待機します:

`docker compose start --wait --wait-timeout {{seconds}}`
