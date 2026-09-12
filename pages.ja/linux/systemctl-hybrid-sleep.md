# systemctl hybrid-sleep

> システムをハイブリッド スリープ状態にします。これは、RAM へのサスペンドと休止状態を組み合わせたものです。
> 詳細情報: <https://www.freedesktop.org/software/systemd/man/latest/systemctl.html#hybrid-sleep>。

- システムをただちにハイブリッド スリープ状態にします:

`systemctl hybrid-sleep`

- インヒビターが存在する場合でもハイブリッド スリープを強制します:

`systemctl hybrid-sleep {{[-f|--force]}}`

- ログインしているユーザーにウォール メッセージを送信せずにシステムをハイブリッド スリープにします:

`systemctl hybrid-sleep --no-wall`
