# systemctl is-system-running

> システムの現在の状態を確認します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#is-system-running>。

- システムが動作しているかどうかを確認し、現在の状態を出力します:

`systemctl is-system-running`

- 現在の状態を静かにチェックして印刷します (出力なし、終了ステータスのみ):

`systemctl is-system-running {{[-q|--quiet]}}`

- 現在の状態を出力する前に、ブート プロセスが完了するまで待ちます:

`systemctl is-system-running --wait`
