# docker container update

> Dockerコンテナの構成を更新します。
> 注: このコマンドは Windows コンテナではサポートされていません。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/container/update/>。

- 特定のコンテナが終了したときに適用される再起動ポリシーを更新します:

`docker {{[update|container update]}} --restart {{always|no|on-failure|unless-stopped}} {{container_name}}`

- 特定のコンテナーがゼロ以外の終了ステータスで終了した場合に、そのコンテナーを最大 3 回再起動するようにポリシーを更新します:

`docker {{[update|container update]}} --restart on-failure:3 {{container_name}}`

- 特定のコンテナーで使用可能な CPU の数を更新します:

`docker {{[update|container update]}} --cpus {{count}} {{container_name}}`

- 特定のコンテナーのメモリ制限を [M] メガバイト単位で更新します:

`docker {{[update|container update]}} {{[-m|--memory]}} {{limit}}M {{container_name}}`

- 特定のコンテナ内で許可されるプロセス ID の最大数を更新します (無制限の場合は `-1` を使用します):

`docker {{[update|container update]}} --pids-limit {{count}} {{container_name}}`

- 特定のコンテナがディスクにスワップできるメモリ量を [M] メガバイト単位で更新します (無制限の場合は `-1` を使用します):

`docker {{[update|container update]}} --memory-swap {{limit}}M {{container_name}}`
