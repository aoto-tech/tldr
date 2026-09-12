# systemctl preset-all

> インストールされているすべてのユニットの有効化状態を、プリセット ポリシー ファイルで指定されているデフォルトにリセットします。
> 「`systemctl preset`」、「`systemctl list-unit-files`」も参照してください。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#preset-all>。

- インストールされているすべてのユニットの有効化状態をリセットします:

`sudo systemctl preset-all`

- 事前設定ポリシーで有効としてマークされている場合にのみ有効にします:

`sudo systemctl preset-all --preset-mode enable-only`

- プリセットポリシーで無効としてマークされている場合のみ無効にします:

`sudo systemctl preset-all --preset-mode disable-only`

- 出力を抑制し、終了コードのみを返します:

`sudo systemctl preset-all {{[-q|--quiet]}}`
