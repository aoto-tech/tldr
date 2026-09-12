# systemctl is-active

> 1 つ以上の systemd ユニットがアクティブかどうかを確認します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#is-active%20PATTERN%E2%80%A6>。

- ユニットがアクティブかどうかを確認します:

`systemctl is-active {{unit}}`

- 複数のユニットがアクティブかどうかを確認します:

`systemctl is-active {{unit1 unit2 ...}}`

- 状態を `stdout` に出力せずに、ユニットがアクティブかどうかを確認します:

`systemctl is-active {{unit}} {{[-q|--quiet]}}`

- ユーザーユニットがアクティブかどうかを確認します:

`systemctl is-active {{unit}} --user`
