# systemctl soft-reboot

> カーネルを実行したまま、ユーザー空間をシャットダウンして再起動します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#soft-reboot>。

- すぐにソフト再起動を実行します:

`systemctl soft-reboot`

- ソフトリブートを強制します:

`systemctl soft-reboot {{[-f|--force]}}`

- 特定の時間にソフト リブートをスケジュールします:

`systemctl soft-reboot --when "{{timestamp}}"`

- スケジュールされたソフト リブートをキャンセルします:

`systemctl soft-reboot --when cancel`
