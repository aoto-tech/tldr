# systemctl service-log-target

> サービスのログターゲットを取得または設定します。
> D-Bus 統合サービスでのみ機能します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#service-log-target%20SERVICE%20%5BTARGET%5D>。

- サービスの現在のログ ターゲットを表示します:

`systemctl service-log-target {{service_name}}`

- ログ ターゲットを `console` に設定します (ログを `stderr` に送信します):

`systemctl service-log-target {{service_name}} console`

- ログ ターゲットを `journal` に設定します (ログを `systemd-journald` に送信します):

`systemctl service-log-target {{service_name}} journal`

- ログ ターゲットを `syslog` に設定します (ログを `/dev/log` に送信します):

`systemctl service-log-target {{service_name}} syslog`

- systemd が適切なログ ターゲットを選択できるようにします:

`systemctl service-log-target {{service_name}} auto`

- すべてのログ出力を無効にします:

`systemctl service-log-target {{service_name}} null`
