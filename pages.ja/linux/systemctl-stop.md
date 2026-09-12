# systemctl stop

> systemd ユニットを停止します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#stop%20PATTERN%E2%80%A6>。

- ユニットを停止します:

`systemctl stop {{unit}}`

- サービスを停止し、警告を抑制します:

`systemctl stop {{unit}} --no-warn`

- ユーザーユニットを停止します:

`systemctl stop {{unit}} --user`
