# systemctl log-target

> systemd マネージャーのログ ターゲットを取得または設定します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#log-target%20%5BTARGET%5D>。

- systemd マネージャーの現在のログ ターゲットを表示します:

`systemctl log-target`

- マネージャーのログターゲットを設定します:

`systemctl log-target {{journal-or-kmsg|journal|kmsg|console|syslog|null|auto}}`
