# systemctl switch-root

> 新しいルート ファイルシステムに切り替えて、新しいシステム マネージャーを実行します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#switch-root%20ROOT%20INIT>。

- 新しいルート ファイルシステムに切り替えて、そのデフォルトの init システムを実行します:

`systemctl switch-root {{path/to/new_root}}`

- 新しいルート ファイルシステムに切り替えて、特定の init バイナリを実行します:

`systemctl switch-root {{path/to/new_root}} {{/sbin/init}}`

- 詳細な出力を含む新しいルート ファイルシステムに切り替えます:

`systemctl switch-root {{path/to/new_root}} {{[-v|--verbose]}}`
