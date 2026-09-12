# systemctl list-paths

> 現在メモリ内にあるパスユニットをパス順にリストします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-paths%20PATTERN%E2%80%A6>。

- 現在メモリ内にあるすべてのパス ユニットを表示します:

`systemctl list-paths`

- 特定のワイルドカード パターン (`shell-globbing`) に一致するパス ユニットをリストします:

`systemctl list-paths {{pattern}}`

- 複数のパターンに一致するパスユニットをリストします:

`systemctl list-paths {{pattern_1 pattern_2 ...}}`

- 非アクティブなものを含むすべてのパス ユニットを表示します:

`systemctl list-paths {{[-a|--all]}}`

- パスユニットを状態別にフィルタリングします:

`systemctl list-paths --state {{state}}`

- 出力に単位タイプも表示します:

`systemctl list-paths --show-types`
