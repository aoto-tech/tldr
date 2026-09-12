# systemctl help

> 1 つ以上のユニット、またはプロセスが属するユニット (PID 別) のマニュアル ページを表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#help%20PATTERN%E2%80%A6%7CPID%E2%80%A6>。

- 特定のユニットのマニュアル ページを表示します:

`systemctl help {{unit}}`

- 複数のユニットのマニュアル ページを表示します:

`systemctl help {{unit1 unit2 ...}}`

- ユーザーユニットのマニュアルページを表示します:

`systemctl help {{unit}} --user`

- ページャーを使用せずにマニュアル ページを表示します (一度に):

`systemctl help {{unit}} --no-pager`

- PID ごとにプロセス単位のマニュアル ページを表示します:

`systemctl help {{process_id}}`
