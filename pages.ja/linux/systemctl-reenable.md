# systemctl reenable

> 1 つ以上のユニットを再度有効にします。
> サービスの対象が変更される場合に使用されます。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#reenable%20UNIT%E2%80%A6>。

- ユニットを再度有効にして、デフォルトのシンボリックリンクを復元します:

`systemctl reenable {{unit}}`

- 複数のユニットを一度に再度有効にします:

`systemctl reenable {{unit1 unit2 ...}}`

- ユニットを再度有効にして、すぐに開始します:

`systemctl reenable {{unit}} --now`
