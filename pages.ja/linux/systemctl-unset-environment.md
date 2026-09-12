# systemctl unset-environment

> 1 つ以上のサービス マネージャー環境変数の設定を解除します。
> これにより、`systemctl set-environment` の効果が取り消されます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#unset-environment%20VARIABLE%E2%80%A6>。

- 単一の環境変数の設定を解除します:

`systemctl unset-environment {{var}}`

- 複数の環境変数の設定を一度に解除します:

`systemctl unset-environment {{var1 var2 ...}}`

- ユーザー サービス マネージャーで環境変数の設定を解除します:

`systemctl unset-environment {{var}} --user`
