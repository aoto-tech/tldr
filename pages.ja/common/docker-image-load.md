# docker image load

> Docker イメージをファイルまたは `stdin` からロードします。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/image/load/>。

- `stdin` から Docker イメージをロードします:

`docker < {{path/to/image_file.tar}} {{[load|image load]}}`

- 特定のファイルから Docker イメージをロードします:

`docker {{[load|image load]}} {{[-i|--input]}} {{path/to/image_file.tar}}`

- Quiet モードで特定のファイルから Docker イメージをロードします:

`docker {{[load|image load]}} {{[-q|--quiet]}} {{[-i|--input]}} {{path/to/image_file.tar}}`
