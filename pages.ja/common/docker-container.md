# docker container

> Dockerコンテナを管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/>。

- 現在実行中の Docker コンテナを一覧表示します:

`docker {{[ps|container ls]}}`

- 1 つ以上の停止したコンテナを起動します:

`docker {{[start|container start]}} {{container1_name container2_name ...}}`

- 1 つ以上の実行中のコンテナを強制終了します:

`docker {{[kill|container kill]}} {{container1_name container2_name ...}}`

- 実行中の 1 つ以上のコンテナを停止します:

`docker {{[stop|container stop]}} {{container1_name container2_name ...}}`

- 1 つ以上のコンテナ内のすべてのプロセスを一時停止します:

`docker {{[pause|container pause]}} {{container1_name container2_name ...}}`

- 1 つ以上のコンテナに関する詳細情報を表示します:

`docker container inspect {{container1_name container2_name ...}}`

- コンテナのファイルシステムを `.tar` アーカイブとしてエクスポートします:

`docker {{[export|container export]}} {{container_name}}`

- コンテナの変更から新しいイメージを作成します:

`docker {{[commit|container commit]}} {{container_name}}`
