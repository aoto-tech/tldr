# systemctl suspend

> システムを一時停止します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#suspend>。

- システムを直ちに一時停止します:

`systemctl suspend`

- 5 分の遅延後に一時停止をスケジュールします:

`sleep 300 && systemctl suspend`

- システムを一時停止し、遅れて休止状態にします:

`systemctl hybrid-sleep`
