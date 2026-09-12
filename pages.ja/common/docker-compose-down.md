# docker compose down

> `docker compose up` によって作成されたコンテナー、ネットワーク、イメージ、およびボリュームを停止して削除します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/compose/down/>。

- すべてのコンテナとネットワークを停止して削除します:

`docker compose down`

- サービスで使用されるコンテナー、ネットワーク、およびすべてのイメージを停止して削除します:

`docker compose down --rmi all`

- コンテナ、ネットワーク、およびカスタム タグのないイメージのみを停止して削除します:

`docker compose down --rmi local`

- コンテナ、ネットワーク、およびすべてのボリュームを停止して削除します:

`docker compose down {{[-v|--volumes]}}`

- 孤立したコンテナを含むすべてを停止して削除します:

`docker compose down --remove-orphans`

- 代替構成ファイルを使用してコンテナを停止および削除します:

`docker compose {{[-f|--file]}} {{path/to/config}} down`

- 秒単位のカスタム タイムアウトを使用してコンテナを停止および削除します:

`docker compose down {{[-t|--timeout]}} {{timeout}}`

- Compose ファイルで定義されていないサービスのコンテナを削除します:

`docker compose down --remove-orphans {{[-v|--volumes]}}`
