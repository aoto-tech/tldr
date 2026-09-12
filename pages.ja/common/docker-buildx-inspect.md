# docker buildx inspect

> 現在のビルダー インスタンスまたは指定されたビルダー インスタンスを検査します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/inspect>。

- 現在のビルダー インスタンスに関する情報を表示します:

`docker buildx inspect`

- 特定のビルダー インスタンスを名前で検査します:

`docker buildx inspect {{builder_name}}`

- 以下を検査する前に、ビルダーが実行されていることを確認してください:

`docker buildx inspect --bootstrap`

- ビルダーのステータスをロードするためのデフォルトのタイムアウト (デフォルト: 20 秒) をオーバーライドします:

`docker buildx inspect --timeout {{seconds}}`
