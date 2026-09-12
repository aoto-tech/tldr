# systemctl set-environment

> 1 つ以上のサービス マネージャー環境変数を設定します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#set-environment%20VARIABLE=VALUE%E2%80%A6>。

- 単一の環境変数を設定します:

`systemctl set-environment {{var value}}`

- 複数の環境変数を一度に設定します:

`systemctl set-environment {{var1 value1 var2 value2 ...}}`

- ユーザー サービス マネージャーの環境変数を設定します:

`systemctl set-environment {{var value}} --user`
