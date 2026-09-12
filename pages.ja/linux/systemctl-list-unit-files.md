# systemctl list-unit-files

> インストールされているユニット ファイルとその有効化状態を一覧表示します。
> `systemctl list-units` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-unit-files%20PATTERN%E2%80%A6>。

- インストールされているユニット ファイルとその状態を一覧表示します:

`systemctl list-unit-files`

- 状態でフィルターします:

`systemctl list-unit-files --state {{enabled|disabled|static|...}}`

- ユニットタイプでフィルタリングします:

`systemctl list-unit-files {{[-t|--type]}} {{service|socket|timer|...}}`

- 名前パターンでフィルターします:

`systemctl list-unit-files '{{sshd*}}'`

- 出力を `stdout` に直接印刷します:

`systemctl list-unit-files --no-pager`

- ヘッダーまたはフッターなしで出力を印刷します:

`systemctl list-unit-files --no-legend`
