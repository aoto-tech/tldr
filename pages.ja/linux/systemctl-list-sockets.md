# systemctl list-sockets

> 現在メモリ内にあるアクティブなソケット ユニットをリスニング アドレス順にリストします。
> 「`systemctl list-units`」、「`systemctl list-unit-files`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-sockets%20PATTERN%E2%80%A6>。

- 現在メモリ内にあるアクティブなソケット ユニットをリストします:

`systemctl list-sockets`

- アクティブなソケット ユニットとそのソケット タイプをリストします:

`systemctl list-sockets --show-types`

- 非アクティブなものや障害が発生したものを含む、すべてのソケット ユニットをリストします:

`systemctl list-sockets {{[-a|--all]}}`

- 状態別にフィルタリングされたソケットユニットをリストします:

`systemctl list-sockets --state {{active|inactive|failed|...}}`

- 名前パターンに一致するソケットユニットをリストします:

`systemctl list-sockets {{pattern1 pattern2 ...}}`
