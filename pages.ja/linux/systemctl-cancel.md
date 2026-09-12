# systemctl cancel

> システム マネージャーまたはユーザー マネージャーで 1 つ以上の保留中のジョブをキャンセルします。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#cancel%20JOB%E2%80%A6>。

- 数値 ID でジョブをキャンセルします:

`systemctl cancel {{job_id}}`

- 複数のジョブをキャンセルする:

`systemctl cancel {{job_id1 job_id2 ...}}`

- 保留中のジョブをすべてキャンセルします:

`systemctl cancel`

- ユーザーサービスマネージャーでジョブをキャンセルします:

`systemctl cancel {{job_id}} --user`
