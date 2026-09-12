# docker buildx rm

> 1 つ以上のビルダー インスタンスを削除します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/buildx/rm/>。

- ビルダー インスタンスを削除します:

`docker buildx rm {{builder_name}}`

- 非アクティブなビルダーをすべて削除します:

`docker buildx rm --all-inactive`

- 確認を求めるプロンプトを表示せずに、非アクティブなビルダーをすべて削除します:

`docker buildx rm --all-inactive {{[-f|--force]}}`
