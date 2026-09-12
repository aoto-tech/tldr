# systemctl list-dependencies

> systemd でユニットの依存関係ツリーを表示します。
> `systemctl list-units` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-dependencies%20UNIT%E2%80%A6>。

- `default.target` の依存関係ツリーを表示します:

`systemctl list-dependencies`

- 特定のユニットの依存関係ツリーを表示します:

`systemctl list-dependencies {{unit}}`

- すべての依存関係タイプ (`Requires=` と `Wants=` だけでなく) を含めます:

`systemctl list-dependencies {{unit}} {{[-a|--all]}}`

- ツリーを特定のユニット タイプに制限します:

`systemctl list-dependencies {{unit}} {{[-t|--type]}} {{service|socket|target|mount|...}}`

- 方向を反転すると、指定した単位に依存する単位が表示されます:

`systemctl list-dependencies {{unit}} --reverse`

- ヘッダーまたはフッターなしで出力を印刷します (スクリプトの場合):

`systemctl list-dependencies {{unit}} --no-legend`
