# docker compose stop

> コンテナーを削除せずに実行を停止します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/compose/stop>。

- 実行中のサービスをすべて停止します:

`docker compose stop`

- 特定のサービスを停止します:

`docker compose stop {{service_1 service_2 ...}}`

- 秒単位のカスタム シャットダウン タイムアウトで停止します:

`docker compose stop {{[-t|--timeout]}} {{seconds}}`

- 特定の構成ファイルで定義されているサービスを停止します:

`docker compose {{[-f|--file]}} {{path/to/compose_file}} stop`

- ドライラン (実行せずに操作を表示):

`docker compose stop --dry-run`

- カスタム タイムアウトを使用して特定のサービスを停止します:

`docker compose stop {{[-t|--timeout]}} {{seconds}} {{service_1 service_2 ...}}`
