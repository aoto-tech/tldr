# docker image pull

> レジストリから Docker イメージをダウンロードします。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/pull/>。

- 特定の Docker イメージをダウンロードします:

`docker {{[pull|image pull]}} {{image}}:{{tag}}`

- 特定の Docker イメージを Quiet モードでダウンロードします:

`docker {{[pull|image pull]}} {{[-q|--quiet]}} {{image}}:{{tag}}`

- 特定の Docker イメージのすべてのタグをダウンロードします:

`docker {{[pull|image pull]}} {{[-a|--all-tags]}} {{image}}`

- 特定のプラットフォーム用の Docker イメージをダウンロードします:

`docker {{[pull|image pull]}} --platform {{linux/amd64}} {{image}}:{{tag}}`

- ヘルプを表示する:

`docker {{[pull|image pull]}} --help`
