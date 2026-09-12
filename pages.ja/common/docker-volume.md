# docker volume

> Docker ボリュームを管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/volume/>。

- ボリュームを作成します:

`docker volume create {{volume_name}}`

- 特定のラベルを持つボリュームを作成します:

`docker volume create --label {{label}} {{volume_name}}`

- サイズ 100 MiB、uid 1000 の `tmpfs` ボリュームを作成します:

`docker volume create {{[-o|--opt]}} {{type}}={{tmpfs}} {{[-o|--opt]}} {{device}}={{tmpfs}} {{[-o|--opt]}} {{o}}={{size=100m,uid=1000}} {{volume_name}}`

- すべてのボリュームをリストします:

`docker volume ls`

- ボリュームを削除します:

`docker volume rm {{volume_name}}`

- ボリュームに関する情報を表示します:

`docker volume inspect {{volume_name}}`

- 未使用のローカル ボリュームをすべて削除します:

`docker volume prune`

- サブコマンドのヘルプを表示します:

`docker volume {{subcommand}} --help`
