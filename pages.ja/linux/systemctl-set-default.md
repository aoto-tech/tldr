# systemctl set-default

> `default.target` エイリアスを指定されたターゲット ユニットにシンボリックリンクします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#set-default%20TARGET>。

- `systemd` のデフォルトのブート モードを設定します:

`systemctl set-default {{target_name.target}}`

- デフォルトで GUI モードで起動するように `systemd` を設定します:

`systemctl set-default graphical.target`

- デフォルトで CLI モードで起動するように `systemd` を設定します:

`systemctl set-default multi-user.target`
