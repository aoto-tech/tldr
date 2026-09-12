# systemctl reload-or-restart

> `systemd` ユニットをリロードするか、再起動します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#reload-or-restart%20PATTERN%E2%80%A6>。

- ユニットをリロードまたは再起動します:

`systemctl reload-or-restart {{unit}}`

- パターンに一致する複数のユニットをリロードまたは再起動します:

`systemctl reload-or-restart {{pattern}}`

- 操作が完了するのを待たずにコマンドを実行します:

`systemctl reload-or-restart {{unit}} --no-block`

- コマンドをユーザー ユニットにのみ適用します:

`systemctl reload-or-restart {{unit}} --user`
