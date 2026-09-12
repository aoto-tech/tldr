# docker image rm

> Docker イメージを削除します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/rm/>。

- 名前を指定して 1 つ以上のイメージを削除します:

`docker {{[rmi|image rm]}} {{image1 image2 ...}}`

- 画像を強制的に削除します:

`docker {{[rmi|image rm]}} {{[-f|--force]}} {{image}}`

- タグ付けされていない親を削除せずに画像を削除します:

`docker {{[rmi|image rm]}} --no-prune {{image}}`

- ヘルプを表示する:

`docker {{[rmi|image rm]}} --help`
