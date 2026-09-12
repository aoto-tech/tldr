# systemctl whoami

> プロセスが属するユニットを表示します。
> PID が指定されていない場合は、`systemctl` コマンド自体が呼び出されたユニットを表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#whoami%20%5BPID%E2%80%A6%5D>。

- 現在のシェル (`systemctl` が実行されている場所) のユニットを表示します:

`systemctl whoami`

- ユーザー サービス マネージャー (ログイン セッション用に管理されるサービス) で現在のシェルのユニットを表示します:

`systemctl whoami --user`

- 特定のプロセスが属するユニットを表示します:

`systemctl whoami {{process_id}}`

- 複数のプロセスの単位を表示します:

`systemctl whoami {{process_id1 process_id2 ...}}`
