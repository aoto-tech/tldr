# systemctl cat

> systemd が認識するユニット ファイルの完全な内容を表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#cat%20PATTERN%E2%80%A6>。

- ユニットファイルの内容と絶対パスを表示します:

`systemctl cat {{unit}}`

- 複数のユニット ファイルの内容を表示します:

`systemctl cat {{unit1 unit2 ...}}`

- テンプレートのユニット ファイルの内容を表示します:

`systemctl cat {{template@}}`

- ユーザーユニットファイルの内容を表示します:

`systemctl cat {{unit}} --user`
