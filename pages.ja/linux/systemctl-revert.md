# systemctl revert

> ユニット ファイルをベンダー バージョンに戻します。
> `edit`、`enable`、`disable`、`set-property`、および `mask` の効果を元に戻します。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#revert%20UNIT%E2%80%A6>。

- ユニットファイルをデフォルト設定に戻します:

`systemctl revert {{unit1 unit2 ...}}`

- ユーザーユニットファイルを元に戻します:

`systemctl revert {{unit}} --user`
