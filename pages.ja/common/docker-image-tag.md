# docker image tag

> 既存の Docker イメージにタグを割り当てます。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/tag/>。

- 特定のイメージ ID に名前とタグを割り当てます:

`docker {{[tag|image tag]}} {{id}} {{name}}:{{tag}}`

- 特定の画像にタグを割り当てます:

`docker {{[tag|image tag]}} {{image}}:{{current_tag}} {{image}}:{{new_tag}}`

- ヘルプを表示する:

`docker {{[tag|image tag]}}`
