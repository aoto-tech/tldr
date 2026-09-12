# systemctl show

> ユニットまたは systemd 自体のプロパティを表示します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#show%20PATTERN%E2%80%A6%7CJOB%E2%80%A6>。

- システム サービス マネージャーのプロパティを表示します:

`systemctl show`

- ユーザー サービス マネージャーのプロパティを表示します:

`systemctl show --user`

- 特定のユニットのプロパティを表示します:

`systemctl show {{unit}}`

- 特定のユーザーユニットのプロパティを表示します:

`systemctl show {{unit}} --user`

- 空のプロパティをリストに含めます:

`systemctl show {{[-a|--all]}}`

- 指定されたプロパティのみを表示します:

`systemctl show {{unit}} {{[-p|--property]}} {{Wants,Conflicts,...}}`
