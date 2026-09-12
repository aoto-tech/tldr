# systemctl list-machines

> ホストと、実行中のすべてのローカル仮想マシンまたはコンテナをその状態とともに一覧表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-machines%20PATTERN%E2%80%A6>。

- すべてのマシン (ホストおよび実行中のコンテナ/VM) を表示します:

`systemctl list-machines`

- 特定のマシンをリストします:

`systemctl list-machines {{machine}}`

- 複数の一致するマシンをリストします:

`systemctl list-machines {{machine_1 machine_2 ...}}`

- ワイルドカード パターン (`shell-globbing`) を使用してマシンをフィルタリングします:

`systemctl list-machines {{pattern}}`
