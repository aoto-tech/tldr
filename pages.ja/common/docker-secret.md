# docker secret

> Docker swarm シークレットを管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/secret/>。

- `stdin` から新しいシークレットを作成します:

`{{command}} | docker secret create {{secret_name}} -`

- ファイルから新しいシークレットを作成します:

`docker secret create {{secret_name}} {{path/to/file}}`

- すべてのシークレットをリストします:

`docker secret ls`

- 1 つまたは複数のシークレットに関する詳細情報を人間に優しい形式で表示します:

`docker secret inspect --pretty {{secret_name1 secret_name2 ...}}`

- 1 つ以上のシークレットを削除します:

`docker secret rm {{secret_name1 secret_name2 ...}}`
