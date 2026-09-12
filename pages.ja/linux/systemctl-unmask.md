# systemctl unmask

> ユニットのマスクを解除して、再び起動できるようにします。
> これにより、`systemctl mask` の効果が取り消されます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#unmask%20UNIT%E2%80%A6>。

- サービスのマスクを解除します:

`systemctl unmask {{service_name}}`

- マスクを解除してサービスをすぐに開始します:

`systemctl unmask {{service_name}} --now`

- ユーザー サービスのマスクを解除します:

`systemctl unmask {{service_name}} --user`
