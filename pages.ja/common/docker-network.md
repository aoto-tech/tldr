# docker network

> Docker ネットワークを作成および管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/network/>。

- Docker デーモン上で使用可能なすべての構成済みネットワークをリストします:

`docker network ls`

- ユーザー定義のネットワークを作成します:

`docker network create {{[-d|--driver]}} {{driver_name}} {{network_name}}`

- 1 つ以上のネットワークに関する詳細情報を表示します:

`docker network inspect {{network_name1 network_name2 ...}}`

- 名前または ID を使用してコンテナをネットワークに接続します:

`docker network connect {{network_name}} {{container_name|id}}`

- コンテナをネットワークから切断します:

`docker network disconnect {{network_name}} {{container_name|id}}`

- 未使用の (どのコンテナからも参照されていない) ネットワークをすべて削除します:

`docker network prune`

- 1 つ以上の未使用のネットワークを削除します:

`docker network rm {{network_name1 network_name2 ...}}`
