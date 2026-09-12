# docker context

> コンテキストを切り替えて複数の Docker 環境を管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/context/>。

- 特定の Docker エンドポイントを使用してコンテキストを作成します:

`docker context create {{context_name}} --docker "host={{tcp://remote-host:2375}}"`

- `$DOCKER_HOST` 環境変数に基づいてコンテキストを作成します:

`docker context create {{context_name}}`

- コンテキストに切り替えます:

`docker context use {{context_name}}`

- すべてのコンテキストをリストします:

`docker context ls`
