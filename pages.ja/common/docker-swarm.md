# docker swarm

> コンテナ オーケストレーション ツール。
> 詳細情報: <https://docs.docker.com/engine/swarm/>。

- swarm クラスターを初期化します:

`docker swarm init`

- マネージャーまたはワーカーに参加するためのトークンを表示します:

`docker swarm join-token {{worker|manager}}`

- 新しいノードをクラスターに参加させます:

`docker swarm join --token {{token}} {{manager_node_url:2377}}`

- swarm からワーカーを削除します (ワーカー ノード内で実行します):

`docker swarm leave`

- 現在の CA 証明書を PEM 形式で表示します:

`docker swarm ca`

- 現在の CA 証明書をローテーションして、新しい証明書を表示します:

`docker swarm ca --rotate`

- ノード証明書の有効期間を変更します:

`docker swarm update --cert-expiry {{hours}}h{{minutes}}m{{seconds}}s`
