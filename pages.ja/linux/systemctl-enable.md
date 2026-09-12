# systemctl enable

> systemd サービスを有効にします。
> `systemctl revert` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#enable%20UNIT%E2%80%A6>。

- 起動時にサービスを実行できるようにします:

`systemctl enable {{unit}}`

- 起動時にサービスを実行できるようにし、今すぐ開始します:

`systemctl enable {{unit}} --now`

- ユーザーユニットがログイン時に実行できるようにします:

`systemctl enable {{unit}} --user`
