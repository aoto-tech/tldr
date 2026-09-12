# systemctl is-enabled

> ユニットファイルが有効になっているか確認してください。
> 「`systemctl enable`」、「`systemctl disable`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#is-enabled%20UNIT%E2%80%A6>。

- 有効化状態を表示します:

`systemctl is-enabled {{unit1 unit2 ...}}`

- 出力を抑制し、終了コードのみを返します:

`systemctl is-enabled {{unit}} {{[-q|--quiet]}}`

- インストールターゲットとシンボリックリンクパスを表示します:

`systemctl is-enabled {{unit}} {{[-l|--full]}}`
