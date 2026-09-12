# docker buildx prune

> ビルドキャッシュを削除します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/prune/>。

- 現在アクティブなビルダーのビルド キャッシュを削除します:

`docker buildx prune`

- 特定のフィルターに基づいてキャッシュ レコードを削除します:

`docker buildx prune --filter "{{type=source.local}}"`

- キャッシュ サイズが特定の制限を下回るまで、最も最近使用されていないキャッシュ レコードを削除します:

`docker buildx prune --max-used-space {{128mb}}`

- 特定の量の空きディスク領域が利用可能になるまで、最も最近使用されていないキャッシュ レコードを削除します:

`docker buildx prune --reserved-space {{2gb}}`
