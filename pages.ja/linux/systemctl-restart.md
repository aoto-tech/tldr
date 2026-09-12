# systemctl restart

> 1 つ以上の systemd ユニットを停止してから起動します。
> 停止したユニットで `systemctl start` の代わりに使用できますが、実行中のユニットが誤って再起動されないように、`start` の方が安全です。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#restart%20PATTERN%E2%80%A6>。

- ユニットを再起動します:

`systemctl restart {{unit}}`

- 複数のユニットを再起動します:

`systemctl restart {{unit1 unit2 ...}}`

- ユーザーユニットを再起動します:

`systemctl restart {{unit}} --user`
