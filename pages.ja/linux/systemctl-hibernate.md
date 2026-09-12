# systemctl hibernate

> 現在の状態をディスクに保存し、電源をオフにして、システムを休止状態にします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#hibernate>。

- システムをただちに休止状態にします:

`systemctl hibernate`

- インヒビターが存在する場合でも強制的に冬眠させます:

`systemctl hibernate {{[-f|--force]}}`

- ログインしているユーザーにメッセージを送信せずにシステムを休止状態にします:

`systemctl hibernate --no-wall`
