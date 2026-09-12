# docker container stats

> コンテナーのリソース使用量統計のライブ ストリームを表示します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/stats/>。

- 実行中のすべてのコンテナーの統計のライブ ストリームを表示します:

`docker {{[stats|container stats]}}`

- 1 つ以上のコンテナの統計のライブ ストリームを表示します:

`docker {{[stats|container stats]}} {{container1 container2 ...}}`

- 列の形式を変更して、コンテナーの CPU 使用率を表示します:

`docker {{[stats|container stats]}} --format "{{.Name}}:\t{{.CPUPerc}}"`

- すべてのコンテナー (実行中と停止中の両方) の統計を表示します:

`docker {{[stats|container stats]}} {{[-a|--all]}}`

- ストリーミング統計を無効にし、現在の統計のみを取得します:

`docker {{[stats|container stats]}} --no-stream`
