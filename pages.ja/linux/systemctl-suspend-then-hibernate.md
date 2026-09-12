# systemctl suspend-then-hibernate

> システムを一時停止し、一定期間非アクティブ状態が続いた後、自動的に休止状態になります。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#suspend-then-hibernate>。

- システムを一時停止し、設定された遅延の後に休止状態にします:

`systemctl suspend-then-hibernate`

- 強制的にサスペンドしてから休止状態にします (インヒビター ロックをバイパス):

`systemctl suspend-then-hibernate {{[-f|--force]}}`
