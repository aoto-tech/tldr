# systemctl bind

> ファイルまたはディレクトリをホストからユニットのマウント名前空間に一時的にバインドマウントします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#bind%20UNIT%20PATH%20%5BPATH%5D>。

- ホスト パスをユニット内の同じ場所にバインドマウントします:

`systemctl bind {{unit}} /{{path/to/host_directory}}`

- ホスト パスをユニット内の別の場所にバインドマウントします:

`systemctl bind {{unit}} /{{path/to/host_directory}} /{{path/to/unit_directory}}`

- ユニット内でパスを読み取り専用としてバインドマウントします:

`systemctl bind {{unit}} /{{path/to/host_directory}} --read-only`

- バインドする前にユニット内に宛先パスを作成します:

`systemctl bind {{unit}} /{{path/to/host_directory}} /{{path/to/unit_directory}} --mkdir`
