# systemctl list-jobs

> 現在キューに入れられている、またはシステム上で実行されているアクティブな systemd ジョブのリスト。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#list-jobs%20PATTERN%E2%80%A6>。

- すべてのアクティブなジョブをリストします:

`systemctl list-jobs`

- 特定のユニットのジョブをフィルタリングします:

`systemctl list-jobs {{unit}}`
