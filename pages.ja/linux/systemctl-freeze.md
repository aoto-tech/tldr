# systemctl freeze

> 1 つ以上のユニットを凍結します。
> 凍結されたユニットは、`systemctl thaw` で再開できます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#freeze%20PATTERN%E2%80%A6>。

- 特定のユニットをフリーズします:

`systemctl freeze {{unit}}`

- 複数のユニットをフリーズします:

`systemctl freeze {{unit1 unit2 ...}}`

- 実行中のすべてのユニットをフリーズします:

`systemctl freeze '*'`
