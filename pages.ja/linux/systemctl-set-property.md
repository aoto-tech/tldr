# systemctl set-property

> 実行時に指定されたユニットのプロパティを設定します。
> `systemctl revert` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#set-property%20UNIT%20PROPERTY=VALUE%E2%80%A6>。

- 実行中のサービスのプロパティを設定します:

`systemctl set-property {{unit}} {{property}}={{value}}`

- 複数のプロパティを一度に設定します:

`systemctl set-property {{unit}} {{property_1=value_1 property_2=value_2 ...}}`

- 現在のランタイム セッションに対してのみプロパティを設定します (永続的ではありません):

`systemctl set-property {{unit}} {{property}}={{value}} --runtime`

- プロパティをデフォルト値にリセットします:

`systemctl set-property {{unit}} {{property}}=`

- 複数のプロパティをデフォルト値にリセットします:

`systemctl set-property {{unit}} {{property_1= property_2= ...}}`
