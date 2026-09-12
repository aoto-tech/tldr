# docker buildx ls

> ビルダー インスタンスと関連ノードをリストします。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/ls/>。

- ビルダー インスタンスをリストします:

`docker buildx ls`

- Go テンプレートを使用して出力をフォーマットします:

`docker buildx ls --format "{{.NAME}}: {{.DriverEndpoint}}"`
