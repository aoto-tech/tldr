# docker buildx create

> 新しいビルダー インスタンスを作成します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/create/>。

- デフォルトの Docker コンテキストを使用して、新しいビルダー インスタンスを作成します:

`docker buildx create`

- 特定の名前で新しいビルダー インスタンスを作成します:

`docker buildx create --name {{builder_name}}`

- 新しいビルダー インスタンスを作成し、すぐにそれを現在のアクティブなビルダーとして設定します:

`docker buildx create --name {{builder_name}} --use`

- 特定のドライバーを使用して新しいビルダー インスタンスを作成します (デフォルトは `docker`):

`docker buildx create --driver {{docker-container|kubernetes|remote|...}}`

- サポートされている特定のプラットフォームで新しいビルダー インスタンスを作成します:

`docker buildx create --platform {{linux/amd64,linux/arm64,...}}`

- 新しいノードを既存のビルダーに追加します:

`docker buildx create --name {{builder_name}} --append {{context|endpoint}}`

- 特定の BuildKit デーモン フラグを使用して新しいビルダー インスタンスを作成します:

`docker buildx create --buildkitd-flags "{{--debug --debugaddr 0.0.0.0:6666}}"`

- 新しいビルダー インスタンスを作成し、すぐに起動します:

`docker buildx create --name {{builder_name}} --bootstrap`
