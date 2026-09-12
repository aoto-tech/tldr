# systemctl list-units

> systemd が現在メモリ内に持っているユニットをリストします。
> `systemctl list-unit-files` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-units%20PATTERN%E2%80%A6>。

- アクティブなユニット、保留中のジョブがあるユニット、または失敗したユニットをリストします:

`systemctl list-units`

- 非アクティブなものを含むすべてのユニットをリストします:

`systemctl list-units {{[-a|--all]}}`

- ユニットタイプでフィルタリングします:

`systemctl list-units {{[-t|--type]}} {{service|socket|timer|...}}`

- 状態でフィルターします:

`systemctl list-units --state {{running|listening|dead|...}}`

- 名前パターンでフィルターします:

`systemctl list-units 'systemd*'`

- 出力を `stdout` に直接印刷します:

`systemctl list-units --no-pager`

- ヘッダーまたはフッターなしで出力を印刷します (スクリプトの場合):

`systemctl list-units --no-legend`
