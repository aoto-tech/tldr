# docker compose logs

> Docker Compose アプリケーションのコンテナーからの出力を表示します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/compose/logs/>。

- すべてのサービスのログを表示します:

`docker compose logs`

- 特定のサービスのログを表示します:

`docker compose logs {{service_name}}`

- ログを表示し、新しい出力 (`tail --follow` など) を追跡します:

`docker compose logs {{[-f|--follow]}}`

- タイムスタンプ付きのログを表示します:

`docker compose logs {{[-t|--timestamps]}}`

- 各コンテナーのログの最後の `n` 行のみを表示します:

`docker compose logs {{[-n|--tail]}} {{n}}`

- 特定の時点以降のログを表示します:

`docker compose logs --since {{timestamp}}`

- 特定の時刻までのログを表示します:

`docker compose logs --until {{timestamp}}`

- 複数の特定のサービスのログを表示します:

`docker compose logs {{service1 service2 ...}}`
