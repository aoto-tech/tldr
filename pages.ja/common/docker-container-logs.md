# docker container logs

> コンテナーのログを印刷します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/logs/>。

- コンテナからログを出力します:

`docker {{[logs|container logs]}} {{name|id}}`

- ログを印刷して追跡します:

`docker {{[logs|container logs]}} {{name|id}} {{[-f|--follow]}}`

- 最後の 5 行を出力します:

`docker {{[logs|container logs]}} {{name|id}} {{[-n|--tail]}} 5`

- ログを出力し、タイムスタンプを追加します:

`docker {{[logs|container logs]}} {{name|id}} {{[-t|--timestamps]}}`

- コンテナー実行の特定の時点 (つまり、23 分 10 秒、2013-01-02T13:23:37) からのログを出力します:

`docker {{[logs|container logs]}} {{name|id}} --until {{time}}`
