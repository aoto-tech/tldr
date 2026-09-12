# systemctl list-automounts

> 現在メモリ内にある自動マウント ユニットを一覧表示し、マウント パスとユニット名を表示します。
> 「`systemctl list-units`」、「`systemctl list-unit-files`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-automounts%20PATTERN%E2%80%A6>。

- 現在メモリ内にある自動マウント ユニットを一覧表示します:

`systemctl list-automounts`

- 非アクティブなものを含むすべての自動マウント ユニットをリストします:

`systemctl list-automounts {{[-a|--all]}}`

- 自動マウントユニットを状態別にフィルタリングします:

`systemctl list-automounts --state {{active|inactive|failed|...}}`

- 自動マウントユニットを名前パターンでフィルタリングします:

`systemctl list-automounts {{pattern1 pattern2 ...}}`
