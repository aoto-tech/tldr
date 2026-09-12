# docker service

> Docker デーモンでサービスを管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/service/>。

- Docker デーモン上のサービスを一覧表示します:

`docker service ls`

- 新しいサービスを作成します:

`docker service create --name {{service_name}} {{image}}:{{tag}}`

- 1 つ以上のサービスに関する詳細情報を表示します:

`docker service inspect {{service_name_or_id1 service_name_or_id2 ...}}`

- 1 つ以上のサービスのタスクをリストします:

`docker service ps {{service_name_or_id1 service_name_or_id2 ...}}`

- スペースで区切られたサービスのリストの特定の数のレプリカにスケールします:

`docker service scale {{service_name}}={{count_of_replicas}}`

- 1 つ以上のサービスを削除します:

`docker service rm {{service_name_or_id1 service_name_or_id2 ...}}`
