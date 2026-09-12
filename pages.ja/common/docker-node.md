# docker node

> Docker Swarm ノードを管理します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/node/>。

- swarm 内のノードをリストします:

`docker node ls`

- 1 つ以上のノードで実行されているタスクをリストします。デフォルトは現在のノードです:

`docker node ps {{node1 node2 node3 ...}}`

- 1 つ以上のノードに関する詳細情報を表示します:

`docker node inspect {{node1 node2 node3 ...}}`

- swarm 内の 1 つ以上のノードをマネージャーに昇格します:

`docker node promote {{node1 node2 node3 ...}}`

- swarm 内のマネージャーから 1 つ以上のノードを降格します:

`docker node demote {{node1 node2 node3 ...}}`

- 1 つ以上のノードを swarm から削除します:

`docker node rm {{node1 node2 node3 ...}}`

- 可用性、ラベル、ロールなど、ノードに関するメタデータを更新します:

`docker node update --{{availability|role|label-add|...}} {{active|worker|...}} {{node1}}`
