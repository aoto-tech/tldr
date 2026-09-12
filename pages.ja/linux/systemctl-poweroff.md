# systemctl-poweroff

> システムの電源を切ります。
> `poweroff` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#poweroff>。

- システムの電源を切ります:

`systemctl poweroff`

- サービスに正常な停止を要求せずに、すぐにシステムの電源をオフにします:

`systemctl poweroff {{[-f|--force]}}`

- ログインしているユーザーに通知を送信せずに、ただちにシステムの電源をオフにします:

`systemctl poweroff {{[-f|--force]}} --no-wall`
