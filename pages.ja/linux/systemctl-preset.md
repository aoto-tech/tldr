# systemctl preset

> ユニット ファイルの有効化状態を、プリセット ポリシー ファイルで指定されたデフォルトにリセットします。
> 「`systemctl preset-all`」、「`systemctl list-unit-files`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#preset%20UNIT%E2%80%A6>。

- 有効化状態をプリセットのデフォルトにリセットします:

`systemctl preset {{unit1 unit2 ...}}`

- 事前設定ポリシーで有効としてマークされている場合にのみ有効にします:

`systemctl preset {{unit}} --preset-mode enable-only`

- プリセットポリシーで無効としてマークされている場合のみ無効にします:

`systemctl preset {{unit}} --preset-mode disable-only`

- 出力を抑制し、終了コードのみを返します:

`systemctl preset {{unit}} {{[-q|--quiet]}}`
