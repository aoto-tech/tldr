# systemctl log-level

> systemd マネージャーのログ レベルを取得または設定します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#log-level%20%5BLEVEL%5D>。

- systemd マネージャーの現在のログ レベルを表示します:

`systemctl log-level`

- マネージャーのログ レベルを設定します:

`systemctl log-level {{emerg|alert|crit|err|warning|notice|info|debug}}`
