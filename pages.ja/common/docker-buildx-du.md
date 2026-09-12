# docker buildx du

> ビルダーのディスク使用量を参照してください。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/du/>。

- ディスク使用量を表示:

`docker buildx du`

- 特定の条件に基づいて出力をフィルタリングします:

`docker buildx du --filter "{{description~=golang}}"`

- 詳細な出力を表示します:

`docker buildx du --verbose`

- Go テンプレートを使用して出力をフォーマットします:

`docker buildx du --format "table {{.ID}}    {{.Description}}"`

- `jq` コマンドを使用して、出力を JSON としてきれいに印刷します:

`docker buildx du --format json | jq .`

- 特定のビルダーのディスク使用量を検査します:

`docker buildx du --builder {{builder_name}}`
