# systemctl is-failed

> 1 つ以上の systemd ユニットに障害が発生していないか確認してください。
> 「`systemctl is-active`」、「`systemctl status`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#is-failed%20PATTERN%E2%80%A6>。

- 障害が発生したユニットがあるかどうかを確認します:

`systemctl is-failed`

- 1 つまたは複数のユニットに障害が発生したかどうかを確認します:

`systemctl is-failed {{unit1 unit2 ...}}`

- 出力を抑制し、終了コードのみを返します:

`systemctl is-failed {{unit}} {{[-q|--quiet]}}`

- ユーザーユニットに障害が発生したかどうかを確認します:

`systemctl is-failed {{unit}} --user`
