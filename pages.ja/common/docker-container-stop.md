# docker container stop

> 実行中の 1 つ以上のコンテナを停止します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/stop/>。

- Docker コンテナを停止します:

`docker {{[stop|container stop]}} {{container}}`

- コンテナを停止して、コンテナに特定のシグナルを送信します:

`docker {{[stop|container stop]}} {{[-s|--signal]}} {{signal}} {{container}}`

- コンテナを停止し、強制的に強制終了する前に特定の秒数待機します:

`docker {{[stop|container stop]}} {{[-t|--timeout]}} {{seconds}} {{container}}`

- 1 つ以上のコンテナを停止します:

`docker {{[stop|container stop]}} {{container1 container2 ...}}`

- ヘルプを表示する:

`docker {{[stop|container stop]}} --help`
