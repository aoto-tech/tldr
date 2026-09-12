# docker container exec

> すでに実行されている Docker コンテナ上でコマンドを実行します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/exec/>。

- すでに実行中のコンテナ上で対話型シェル セッションを開始します:

`docker {{[exec|container exec]}} {{[-it|--interactive --tty]}} {{container_name}} {{/bin/bash}}`

- 実行中のコンテナ上でバックグラウンド (切り離された状態) でコマンドを実行します:

`docker {{[exec|container exec]}} {{[-d|--detach]}} {{container_name}} {{command}}`

- 特定のコマンドを実行する作業ディレクトリを選択します:

`docker {{[exec|container exec]}} {{[-it|--interactive --tty]}} {{[-w|--workdir]}} {{path/to/directory}} {{container_name}} {{command}}`

- 既存のコンテナーでバックグラウンドでコマンドを実行しますが、`stdin` を開いたままにします:

`docker {{[exec|container exec]}} {{[-i|--interactive]}} {{[-d|--detach]}} {{container_name}} {{command}}`

- 実行中の Bash セッションで環境変数を設定します:

`docker {{[exec|container exec]}} {{[-it|--interactive --tty]}} {{[-e|--env]}} {{variable_name}}={{value}} {{container_name}} {{/bin/bash}}`

- 特定のユーザーとしてコマンドを実行します:

`docker {{[exec|container exec]}} {{[-u|--user]}} {{user}} {{container_name}} {{command}}`
