# systemctl reload

> サービスの構成を再起動せずに再読み込みします。
> これにより、systemd ユニット ファイルではなく、サービス自体 (Apache や `nginx` 構成など) がリロードされます。
> ユニット ファイルを再ロードするには、`systemctl daemon-reload` を使用します。

- サービスをリロードします:

`systemctl reload {{nginx}}`

- 複数のサービスをリロードします:

`systemctl reload {{unit1 unit2 ...}}`

- 現在のユーザーのサービスをリロードします:

`systemctl reload {{pipewire}} --user`
