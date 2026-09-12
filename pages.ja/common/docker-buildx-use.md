# docker buildx use

> 現在のビルダー インスタンスを設定します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/use>。

- 特定のビルダー インスタンスを現在のインスタンスとして設定します:

`docker buildx use {{builder_name}}`

- 現在のコンテキストのデフォルトとしてビルダーを設定します:

`docker buildx use --default {{builder_name}}`

- ビルダーを設定し、コンテキスト間で変更を永続化します:

`docker buildx use --global {{builder_name}}`
