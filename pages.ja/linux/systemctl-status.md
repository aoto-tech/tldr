# systemctl status

> systemd ユニットのステータスを表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#status%20PATTERN%E2%80%A6%7CPID%E2%80%A6%5D>。

- systemd ユニットのステータスを表示します:

`systemctl status {{unit}}.{{service|timer|socket|target|...}}`

- 障害が発生したユニットのステータスを表示します:

`systemctl status --failed`

- 実行中のすべてのサービスをリストします:

`systemctl status`

- システム内のすべてのユニットをリストします:

`systemctl status {{[-a|--all]}}`

- 特定のタイプのすべてのユニットをリストします:

`systemctl status {{[-t|--type]}} {{service|timer|socket|target|...}}`

- 特定の状態のすべてのユニットをリストします:

`systemctl status --state {{active|inactive|failed}}`

- ユーザーユニットのステータスを表示します:

`systemctl status {{unit}} --user`
