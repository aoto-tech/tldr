# systemctl-halt

> システムをシャットダウンして停止します (OS カーネルを停止しますが、ハードウェアの電源はオンのままにします)。
> `halt` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#halt>。

- システムを停止します:

`systemctl halt`

- サービスに正常に停止するように要求せずに、システムをただちに停止します:

`systemctl halt {{[-f|--force]}}`

- ログインしているユーザーに通知を送信せずに、システムをただちに停止します:

`systemctl halt {{[-f|--force]}} --no-wall`

- プロセスを終了したり、ファイルシステムをアンマウントしたりせずに、ただちにシステムを停止します (危険、データ損失の可能性があります):

`systemctl halt {{[-ff|--force --force]}}`

- 特定の時間 (例: 23:00) に停止をスケジュールします:

`systemctl halt --when 23:00`

- 特定の期間 (例: 2 時間) の後に停止するようにスケジュールを設定します:

`systemctl halt --when +2h`

- スケジュールされた停止をキャンセルします:

`systemctl halt --when cancel`
