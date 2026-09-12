# docker-machine

> Docker を実行するマシンを作成および管理します。
> 詳細情報: <https://github.com/docker-archive-public/docker.machine>。

- 現在実行中の Docker マシンをリストします:

`docker-machine ls`

- 特定の名前で新しい Docker マシンを作成します:

`docker-machine create {{name}}`

- マシンのステータスを取得します:

`docker-machine status {{name}}`

- マシンを起動します:

`docker-machine start {{name}}`

- マシンを停止します:

`docker-machine stop {{name}}`

- マシンに関する情報を検査します:

`docker-machine inspect {{name}}`
