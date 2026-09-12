# systemctl reset-failed

> 1 つ以上のユニットの「障害」状態をリセットします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#reset-failed%20%5BPATTERN%E2%80%A6%5D>。

- すべてのユニットの障害状態をリセットします:

`systemctl reset-failed`

- 特定のユニットの障害状態をリセットします:

`systemctl reset-failed {{unit}}`

- 複数のユニットを一度にリセットします:

`systemctl reset-failed {{unit_1 unit_2 ...}}`
