# systemctl service-log-level

> D-Bus 経由でサービスのランタイム ログ レベルを取得または設定します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#service-log-level%20SERVICE%20%5BLEVEL%5D>。

- サービスの現在のログ レベルを表示します:

`systemctl service-log-level {{service_name}}`

- サービスのログ レベルを設定します (レベル名は 0 ～ 7 の数字に置き換えることができます):

`systemctl service-log-level {{service_name}} {{emerg|alert|crit|err|warning|notice|info|debug}}`
