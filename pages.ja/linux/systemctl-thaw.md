# systemctl thaw

> 1 つ以上の凍結ユニットを解凍 (再開) します。
> ユニットは `systemctl freeze` で凍結できます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#thaw%20PATTERN%E2%80%A6>。

- 特定のユニットを解凍します:

`systemctl thaw {{unit}}`

- 複数のユニットを解凍します:

`systemctl thaw {{unit1 unit2 ...}}`

- 現在凍結されているすべてのユニットを解凍します:

`systemctl thaw '*'`
