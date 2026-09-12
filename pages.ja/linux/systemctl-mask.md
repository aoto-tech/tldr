# systemctl mask

> ユニットを起動できないように `/dev/null` にリンクします。
> `systemctl revert` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#mask%20UNIT%E2%80%A6>。

- サービスをマスクする:

`systemctl mask {{service_name}}`

- マスキング中にサービスがシャットダウンされていることを確認します:

`systemctl mask {{service_name}} --now`

- ユーザー サービスをマスクします:

`systemctl mask {{service_name}} --user`
