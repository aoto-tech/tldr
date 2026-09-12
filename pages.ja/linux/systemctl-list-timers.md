# systemctl list-timers

> すべてのアクティブな systemd タイマーをリストします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-timers%20PATTERN%E2%80%A6>。

- すべてのアクティブなタイマーをリストします:

`systemctl list-timers`

- 非アクティブなものを含むすべてのタイマーをリストします:

`systemctl list-timers {{[-a|--all]}}`

- パターンに一致するタイマーをリストします:

`systemctl list-timers {{pattern}}`

- 特定の状態に一致するタイマーをリストします:

`systemctl list-timers --state {{active|inactive|failed|...}}`
