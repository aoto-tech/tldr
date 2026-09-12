# systemctl disable

> systemd サービスを無効にします。
> `systemctl revert` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#disable%20UNIT%E2%80%A6>。

- 起動時にサービスの実行を停止します:

`systemctl disable {{unit}}`

- 起動時にサービスの実行を停止し、現在の実行を停止します:

`systemctl disable {{unit}} --now`

- ログイン時に実行されるユーザー サービスを停止します:

`systemctl disable {{unit}} --user`
