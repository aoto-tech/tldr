# systemctl try-reload-or-restart

> 1 つ以上のユニットがサポートしている場合はリロードします。それ以外の場合は再起動してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#try-reload-or-restart%20PATTERN%E2%80%A6>。

- 特定のユニットをリロードまたは再起動します:

`systemctl try-reload-or-restart {{unit}}`

- 複数のユニットをリロードまたは再起動します:

`systemctl try-reload-or-restart {{unit1 unit2 ...}}`

- パターンに一致するすべてのユニットをリロードまたは再起動します:

`systemctl try-reload-or-restart '{{pattern}}'`
