# systemctl link

> ユニットファイルの検索パス外にあるユニットファイルを検索パスにリンクします。
> `systemctl disable` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#link%20PATH%E2%80%A6>。

- ユニット ファイルをリンクして、systemd コマンドで使用できるようにします:

`systemctl link {{path/to/service}}`

- 複数のユニット ファイルを一度にリンクします:

`systemctl link {{path/to/service1 path/to/service2 ...}}`
