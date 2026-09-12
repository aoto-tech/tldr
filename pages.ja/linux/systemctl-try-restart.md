# systemctl try-restart

> 1 つ以上のユニットが現在実行中の場合にのみ再起動します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#try-restart%20PATTERN%E2%80%A6>。

- 特定のユニットが実行中の場合は再起動します:

`systemctl try-restart {{unit}}`

- 複数のユニットが実行中の場合は再起動します:

`systemctl try-restart {{unit1 unit2 ...}}`

- パターンに一致するすべてのユニットが実行中の場合は再起動します:

`systemctl try-restart '{{pattern}}'`
