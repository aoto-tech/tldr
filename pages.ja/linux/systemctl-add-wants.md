# systemctl add-wants

> `Wants` 依存関係を 1 つ以上のユニットのターゲットに追加します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#add-wants%20TARGET%20UNIT%E2%80%A6>。

- `Wants` 依存関係をターゲットからユニットに追加します:

`systemctl add-wants {{target}} {{unit}}`

- 複数の `Wants` 依存関係を一度に追加します:

`systemctl add-wants {{target}} {{unit1 unit2 ...}}`

- ユーザーレベルの `Wants` 依存関係を追加します:

`systemctl add-wants {{target}} {{unit}} --user`
