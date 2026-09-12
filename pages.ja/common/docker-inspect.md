# docker inspect

> Docker オブジェクトに関する低レベルの情報を返します。
> 詳細情報: <https://docs.docker.com/reference/cli/docker/inspect/>。

- 名前または ID を使用して、コンテナー、イメージ、またはボリュームに関する情報を表示します:

`docker inspect {{container|image|id}}`

- コンテナの IP アドレスを表示します:

`docker inspect {{[-f|--format]}} '\{\{range.NetworkSettings.Networks\}\}\{\{.IPAddress\}\}\{\{end\}\}' {{container}}`

- コンテナのログ ファイルへのパスを表示します:

`docker inspect {{[-f|--format]}} '\{\{.LogPath\}\}' {{container}}`

- コンテナーのイメージ名を表示します:

`docker inspect {{[-f|--format]}} '\{\{.Config.Image\}\}' {{container}}`

- 構成情報を JSON として表示します:

`docker inspect {{[-f|--format]}} '\{\{json .Config\}\}' {{container}}`

- すべてのポート バインディングを表示します:

`docker inspect {{[-f|--format]}} '\{\{range $p, $conf := .NetworkSettings.Ports\}\} \{\{$p\}\} -> \{\{(index $conf 0).HostPort\}\} \{\{end\}\}' {{container}}`

- ヘルプを表示する:

`docker inspect`
