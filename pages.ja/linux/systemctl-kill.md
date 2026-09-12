# systemctl kill

> ユニットの 1 つ以上のプロセスにシグナルを送信します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#kill%20PATTERN%E2%80%A6>。

- `SIGTERM` 信号をユニットに送信してユニットを終了します:

`systemctl kill {{unit}}`

- 特定の信号をユニットに送信します:

`systemctl kill {{[-s|--signal]}} {{signal_number|signal_name}} {{unit}}`

- `SIGHUP` シグナルをユニットのメインプロセスのみに送信します:

`systemctl kill {{[-s|--signal]}} {{[1|SIGHUP]}} --kill-whom main {{unit}}`

- 利用可能な信号をすべてリストします:

`systemctl kill {{[-s|--signal]}} help`
