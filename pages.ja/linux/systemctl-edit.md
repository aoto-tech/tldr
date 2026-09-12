# systemctl edit

> systemd ユニット ファイルを編集します。
> `systemctl revert` も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#edit%20UNIT%E2%80%A6>。

- ユニットファイルを非破壊的にオーバーレイします:

`sudo systemctl edit {{unit_file}}`

- ユニットファイルを編集します:

`sudo systemctl edit {{unit_file}} {{[-l|--full]}}`

- 新しいユニット ファイルを作成します:

`sudo systemctl edit {{unit_file}} {{[-lf|--full --force]}}`

- ユーザーユニットファイルをオーバーレイします:

`systemctl edit {{unit_file}} --user`
